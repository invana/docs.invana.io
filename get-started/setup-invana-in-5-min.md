---
description: Get started with Invana and build a knowledge graph with in minutes.
---

# Setup Invana in 5 minutes

Invana Graph Analytics System can be deployed in your local or cloud using docker.

### Invana Architecture

To ease the development and maintainability of the product, Invana System is built as four main services:

| Service Name | Service Description |
| :--- | :--- |
| Invana Engine | Python and GraphQL API for Apache TinkerPop supported graph databases.  |
| Invana Studio | Web based GUI and management app for graph data.  |
| Apache TinkerPop | _Apache TinkerPop_™ is an open source, vendor-agnostic, graph computing framework. |
| Graph Database |  Any graph database that supports Apache TinkerPop as graph processor. |



### Install and Setup Invana System

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
{% endtabs %}

{% hint style="info" %}
In theory, you can run any Apache TinkerPop supported graph database as graph processing engine with Invana.
{% endhint %}







