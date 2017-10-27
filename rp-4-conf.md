<!-- TITLE: Rp 4 Conf -->
<!-- SUBTITLE: A quick summary of Rp 4 Conf -->

# Header

```
	$ docker run --name swarm_agent --restart=always -d swarm join --addr=10.254.254.2:2375 etcd://10.254.254.2:2379,10.254.254.1:2379/nodes
```

$ docker run --name swarm_manager --restart=always -p 10.254.254.2:4000:4000 -d swarm manage -H :4000 --replication --advertise 10.254.254.2:4000 etcd://10.254.254.2:2379/nodes

$ docker run --restart=always --name mongoprod -v /opt/mongoprod:/data/db --net=swarm --env="constraint:node==rp4" -d mongo

$  docker run -d --restart=always --name=timetrack2 -h timetrack2  --net=swarm -e constraint:node==rp4 -v /opt/timetrack:/config redpelicans/timetrack

$  docker run -d --restart=always --name=proxy2 -h proxy2 --net=swarm --env="constraint:node==rp4" -p 80:80 -v "/opt/proxy":/opt -w /opt  node sh run

$ docker run -d --restart=always --name=website2 -h website2 --net=swarm --env="constraint:node==rp4"   redpelicans/website

$ docker run -d --restart=always -h ghost --name=ghost2 --net=swarm --env="constraint:node==rp4"  -v /opt/ghost:/ghost-override redpelicans/ghost

$ docker run -d --restart=always --name=etcd22 --env="constraint:node==rp4" -v /opt/etcd:/data -p 10.254.254.2:12380:2380 -p 10.254.254.2:12379:2379 quay.io/coreos/etcd  --heartbeat-interval 1000 --election-timeout 5000 -name etcd22 -data-dir /data -listen-client-urls http://0.0.0.0:2379 -advertise-client-urls http://10.254.254.2:12379  -listen-peer-urls http://0.0.0.0:2380 -initial-advertise-peer-urls http://10.254.245.2:12380 -initial-cluster-state existing -initial-cluster etcd1=http://10.254.254.1:2380,etcd2=http://10.254.254.2:2380,etcd11=http://10.254.254.1:12380,etcd22=http://10.254.254.2:12380 


$ docker run -d --restart=always --name=peep -h peep --net=swarm --env="constraint:node==rp4"  -v /opt/peep/params.js:/peep/params/production.js redpelicans/peep
