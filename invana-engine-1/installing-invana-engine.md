# Installing Invana Engine

## Using Docker

```
$ docker run -p 8200:8200 -d  -e GREMLIN_SERVER_URL=ws://xx.xx.xx.xx:8182/gremlin --name invana-engine invanalabs/invana-engine 
```

Following Docker environment variables are supported

* **GREMLIN\_SERVER\_URL**: http or ws gremlin url. ex: ws://xx.xx.xx.xx:8182/gremlin or [http://xx.xx.xx.xx:8182/gremlin](http://xx.xx.xx.xx:8182/gremlin)
* **GREMLIN\_TRAVERSAL\_SOURCE**\(optional\): defaults: 'g'
* **GREMLIN\_SERVER\_USERNAME**\(optional\): gremlin username. ex: myusername
* **GREMLIN\_SERVER\_PASSWORD**\(optional\): gremlin password. ex: mypassword
* **SERVER\_PORT**\(optional, available in standalone python mode only\): port on which invana engine server is available: defaults to 8200

