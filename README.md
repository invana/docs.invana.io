---
description: An open source Graph Analytics and Reasoning Engine.
---

# Invana

Any data, that is well modelled and has knowledge about all the relationships and weights with in the entities of the system can give better insights for making **Informed Decision**.

Invana let's you model the data as connected Graph of entities and relationships. You can extract insights from data by applying models like reasoning and graph algorithms. These models help you with learning relationships, predicting patterns and perform advanced analytics on connected data.

{% hint style="info" %}
Invana provides solutions for Graph Powered Analytics And Machine Learning.
{% endhint %}

### Features

* [x] &#x20;Object Mapper - Models, PropertyTypes, and Form validation
* [x] &#x20;Execute gremlin queries
* [x] &#x20;Built in QuerySets for performing standard CRUD operations on graph.
* [x] &#x20;Utilities for logging queries and performance.
* [x] &#x20;Django-ORM like search when using OGM(ex: has\_\_id\_\_within=\[200752, 82032, 4320], has\_\_name\_\_startingWith="Per")( Refer [search-usage.md](https://github.com/invanalabs/invana/blob/master/search-usage.md) for more)
* [x] &#x20;Index support
* [ ] &#x20;Query caching support
* [ ] &#x20;Asynchronous Python API.

### Architecture

![Invana architecture](<.gitbook/assets/image (1).png>)

### How Invana works

1. **Model your system** with the labels of entities and relationships.
2. **Import data** using python SDK or GraphQL API.
3. **Setup Functions** on Entities and Relationships to teach and learn patterns with in the Graph.
4. **Query and Visualise** inferences, reasoning and analytics data as force directed graphs.

Setup your first Knowledge Graph & Graph Powered Analytics Engine  with Invana in just few minutes, get started [here](setup-invana.md)
