# Installation

Invana Engine is served over GraphQL, so it can be used without Invana Studio. For any such use cases, below are the docker-based and standalone installation methods.

Invana Engine connects to the Apache TinkerPop's Gremlin Server's for communicating with the Graph Database. Below is the simple representation of how Invana Engine connects to a Graph Database.

![](../../.gitbook/assets/invana-engine-graph-db-setup.svg)

### Running using Docker

```
$ docker run -p 8200:8200 -d  -e GREMLIN_SERVER_URL=ws://xx.xx.xx.xx:8182/gremlin --name invana-engine invanalabs/invana-engine 
```

Invana Engine will be available at http://\<ip-address:8200>. Following Docker environment variables are supported:

* **GREMLIN\_SERVER\_URL**: http or ws gremlin url. ex: ws://xx.xx.xx.xx:8182/gremlin or [http://xx.xx.xx.xx:8182/gremlin](http://xx.xx.xx.xx:8182/gremlin)
* **GREMLIN\_TRAVERSAL\_SOURCE**(optional): defaults: 'g'
* **GREMLIN\_SERVER\_USERNAME**(optional): gremlin username. ex: myusername
* **GREMLIN\_SERVER\_PASSWORD**(optional): gremlin password. ex: mypassword
* **SERVER\_PORT**(optional, available in standalone python mode only): port on which invana engine server is available: defaults to 8200

{% hint style="info" %}
You can explore docker compose templates from [here](https://github.com/invanalabs/invana-engine/tree/develop/docker-templates) to deploy Invana Engine with Analytics Infrastructure with any of Invana supported Graph databases.
{% endhint %}

### Running using Python server (standalone)

```
pip3 install invana-engine

export GREMLIN_SERVER_URL=ws://xx.xx.xx.xx:8182/gremlin
invana-engine-start
```

{% hint style="warning" %}
Running python server via this implementation is not designed for production setup.&#x20;
{% endhint %}
