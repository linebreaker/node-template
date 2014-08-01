# node-template

A template for nodejs project with easy git deployment.

TODO: Documentation.

# Deployment installation

```bash

# 1. On server, ssh git@<host>:
> mkdir <project name>
> cd <project name>
> git init
> git config receive.denyCurrentBranch ignore

# 2. On client: 
> git remote add prod git@<host>:<project name>
> git push prod master

# 3. On server:
> git checkout master
> cp .env.sample .env
> nano .env # Edit env variables as needed.
> config/restart

# 4. After installation, deploy is performed as (on client):
> git push prod

```


