---
description: Deploy Invana infrastructure using docker compose
---

# Setup Invana

Invana Graph Analytics System can be deployed in your local or cloud using [docker compose](https://docs.docker.com/compose/).

## Install and Setup Invana System

You can use the following templates to setup Invana with supported graph databases as graph processing engine.

{% tabs %}
{% tab title="Using JanusGraph" %}
```text
git clone git@github.com:invanalabs/docker-templates.git
cd docker-templates/invana-with-janusgraph
docker-compose up
```
{% endtab %}

{% tab title="Using Neo4j" %}
```text
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

| service name | service available at |
| :--- | :--- |
| Invana Engine | http://&lt;ip-address&gt;:8200 |
| Invana Studio | http://&lt;ip-address&gt;:8300 |
| Apache TinkerPop Server | http://&lt;ip-address&gt;:8182 |

Docker compose will expose the following services, that lets you visualise and browse through the graph data.

Let's start with a story of graph.

{% page-ref page="build-your-first-graph.md" %}

