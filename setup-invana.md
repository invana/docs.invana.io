---
description: Deploy Invana infrastructure using docker compose
---

# Getting Started

Invana Graph Analytics System can be deployed in your local or cloud using [docker compose](https://docs.docker.com/compose/).

### Features

1.

### Install using Docker

You can use the following templates to setup Invana with supported graph databases as graph processing engine.

{% tabs %}
{% tab title="Using JanusGraph" %}
```
git clone git@github.com:invanalabs/docker-templates.git
cd docker-templates/invana-with-janusgraph
docker-compose up
```
{% endtab %}

{% tab title="Using Neo4j" %}
```
git clone git@github.com:invanalabs/docker-templates.git
cd docker-templates/invana-with-neo4j
docker-compose up
```
{% endtab %}

{% tab title="Using ArcadeDB" %}
```
git clone git@github.com:invanalabs/docker-templates.git
cd docker-templates/invana-with-arcadedb
docker-compose up
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
In theory, you can run any Apache TinkerPop supported graph database as graph processing engine with Invana.
{% endhint %}

| Invana Engine           | http://\<ip-address>:8200 |
| ----------------------- | ------------------------- |
| Invana Studio           | http://\<ip-address>:8300 |
| Apache TinkerPop Server | http://\<ip-address>:8182 |

Docker compose will expose the following services, that lets you visualise and browse through the graph data.

### Graph databases

1. [JanusGraph](https://janusgraph.org)

### Usage&#x20;

* [x] Python API&#x20;
* [ ] GraphQL API&#x20;
* [ ] REST API

Let's start with a story of graph.

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}
