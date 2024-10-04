### Docker in Coder Workspace

A quick start run Coder on a local desktop and to run Docker within container-based Coder workspace. The different options are described [here](https://coder.com/docs/templates/docker-in-workspaces).


#### 1) Prequisites for Mac

* Running Docker Desktop 
* Coder Binary [Installed](https://coder.com/docs/install)
* Clone this repo

Verify Coder CLI installed:
```
coder version
```

#### 2) Start Coder server 

To start Coder server on local mac (foreground):
```
coder server
```

#### 3) Launch the Coder UI

When coder server starts, the logs will show a public access url that was automatically created. If you choose not to use the public access url you can also connect to the localhost:3000. 

```
Coder v2.16.0+683a720 - Your Self-Hosted Remote Development Platform
Started HTTP listener at http://127.0.0.1:3000
Using built-in PostgreSQL (/Users/roger/Library/Application Support/coderv2/postgres)
Opening tunnel so workspaces can connect to your deployment. For production scenarios, specify an external access URL
╔═══════════════════════════════════════════════╗
║               View the Web UI:                ║
║   https://adfasfdasdf.pit-1.try.coder.app   ║
╚═══════════════════════════════════════════════╝
```

#### 4) Create first Admin account Login to UI 


#### 5) Coder CLI Login

```
unset CODER_SESSION_TOKEN
```
```
coder login http(s)://<access url>
```

#### 6) Coder Push Templates & Deploy Workspaces

There are three different template options for Privileged docker sidecar. Feel free to try one or all.
```
coder template push
```
