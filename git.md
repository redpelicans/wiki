<!-- TITLE: Git -->
<!-- SUBTITLE: A quick summary of Git -->

# Git workflow

The workflow heavily relies on branches. It assigns very specific roles to these branches and defines how and when they should interact. Branches are used for preparing, maintaining and keep track of releases.

This workflow allows isolated experiments and a more efficient collaboration.

## Basics

All developpers work locally and push branches to a central repo. The central repo is seen as the communication hub for all developpers.

**Everything in master is always deployable**
### Required branches
The master branch stores official release history and all its commits should be tagged with semver convention.
The staging branch is used as an integration branch for features.

### Feature branches
Each new feature should resides in its own branch. This branch could be pushed to the hub for backup or collaboration.
A feature branch is branching off staging and not master.
When a feature is complete, the concerned branch is merged back in staging.

**Features should never interact directly with master**

### Release branches

Once staging is ready for a release, a release branch is created by forking staging. New feature could not be added anymore back to staging during the life of a release branch.

**Only release-oriented tasks should go in a release branch (bug, fixes, documentation, etc…)**
Once ready, release branch is merged into master with a version tag and in parallel merged back in staging.

This kind of branch allows part of the team to double-check the release while the rest continues to work on features for the next releases.

### Hotfix branches
Hotfix branches are used to patch releases. This is the only branch that is forked directly from master. Once the fix is complete, branch is merged back into master with a hotfix tag (ie: v1.0.0 becomes v1.0.1) and in parallel merged into staging or in the current release branch if exists (in this case, the hotfix will be merged into staging when the release branch will merged back in staging).

## Lifecycle
We assumed the central repository exists (with a branch master).

Only if not set yet:

create the staging branch locally
```
$ git branch staging
```
push staging branch to origin (-u will add tracking reference, used by pull/push)
```
$ git push -u origin staging
```

### For any new developer:
get the project
```
$ git clone https://github.com/CodeRedInc/Cockpit.git 
```

create a local staging branch based on the one on origin and will set it as the current one 
(git branch staging && git checkout staging will do the same while on origin/master)
```
$ git checkout -b staging origin/staging
```

### Pull requests (to use for feature, release & hotfix):
Instead of allowing everybody to be able to merge (into staging or master), we use pull requests.
They provide a way to notify project manager (or lead dev maybe) changes to be considered and monitoring them.

When a feature/release/hotfix is done in its branch, the developer creates a pull request of the branch.
The project manager is notified and is able to see precisely what changes are made and he could measure the impact on the whole project. 
If everything is ok, the pull request is accepted and the merge is automatically done.

Github offers a great interface around pull requests that allows to track them (and see what feature/hotfix is in the pipe) and discuss about them (thanks to a markdown commentary interface).

### Make a fix with a pull request:
```
$ git checkout -b hotfix master
#fix the bug in hotfix
$ git checkout master
$ git pull
$ git checkout hotfix
$ git merge master
#fix conflicts if needed
$ git push -u origin hotfix
#on github, click on the green button, compare, review or pull request, then click on create a pull request after checking if everything was right.
#on github, click on merge pull request when reviewing is done.
```