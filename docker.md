<!-- TITLE: Docker -->
<!-- SUBTITLE: A quick summary of Docker -->

# Header

<!-- TITLE: Docker -->
<!-- SUBTITLE: A quick summary of Docker -->

# Context

Docker is installed on rp3.redpelicans.com and rp4.redpelicans.com
rp3 and rp4 are managers, init swarm on rp3, ask rp4 to join it as manager.

```
rp3:~# docker swarm init --advertise-addr 10.254.254.1

To add a worker to this swarm, run the following command:

    docker swarm join --token SWMTKN-1-3bk9ehvl35pq9rpraf3vcb4wdg86aea6fvfwzhb49ois30758h-4lekrafjk567scfdoqkaxaq3x 10.254.254.1:2377

To add a manager to this swarm, run 'docker swarm join-token manager' and follow the instructions.

root@rp4:~# docker node ls
ID                            HOSTNAME            STATUS              AVAILABILITY        MANAGER STATUS
s4lt9uzo9szl8z9vnx7nx70yo     rp3                 Ready               Active              Leader
f2c1hjlonmbxv5b2x9jkitpm1 *   rp4                 Ready               Active              Reachable


rp3:~# docker info 
...

```

# Launch Docker containers

## MongoProd

`mongoprod` needs a mount of /opt/mongoprod folder, so it must start on rp4:
mongo data are saved in /opt/mongoprod/dump via crontab and copy to rp3:/opt/bkp

```
rp4:~# docker run --restart=always --name mongoprod -v /opt/mongoprod:/data/db --net=swarm --replicas 1 --constraint 'node.hostname==rp4' -d mongo
```
## website

website is accessible directly via port 8282 or via proxy

```
# docker service create --name website --replicas 2 --publish 8282:80 --network net1 -d redpelicans/website

```

## Proxy

/opt/proxy are installed on both rp3 and rp4 so we can run proxy like this:

``` 
# docker service create --name=proxy  --replicas 2 --network net1  -p 80:80 --mount type=bind,src=/opt/proxy,target=/opt -w /opt -d node sh run
```


## peep

```
# docker service create --replicas 1 --name=peep --network net1 --constraint 'node.hostname==rp4' -p 8383:80 --mount type=bind,src=/opt/peep/params.js,dst=/peep/params/production.js -d  redpelicans/peep
```

## ghost

```
# docker service create -d  --name=ghost --network net1 --constraint 'node.hostname==rp4' --mount type=bind,src=/opt/ghost,dst=/ghost-override redpelicans/ghost
```

## wiki

```
# docker service create -d --name=wiki --network net1 --constraint 'node.hostname==rp4' --replicas 1 -e "WIKI_ADMIN_EMAIL=admin@redpelicans.com" --mount type=bind,src=/opt/wiki/config.yml,dst=/var/wiki/config.yml --mount type=bind,src=/opt/wiki/github,dst=/var/wiki/github -p 8181:3000 requarks/wiki
```

