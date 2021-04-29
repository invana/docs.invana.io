# Python API User Guide

### Installing Python SDK for Invana Engine

```
$ pip3 install invana-engine
```

{% hint style="info" %}
Supports Python 3.8 only  
{% endhint %}

### Connecting to Invana Engine

```python
from invana_engine.gremlin.client import InvanaEngineClient

gremlin_server_url = "ws://127.0.0.1:8182/gremlin"
client = InvanaEngineClient(gremlin_server_url=gremlin_server_url)
```

### Operations on Vertex

#### client.vertex.create\(label=None, properties=None\)

| param name | param description |
| :--- | :--- |
| label | Vertex label |
| properties | key, value pairs of properties data |

```python
earth_label = "Planet"
earth_properties = {
    "name": "Earth",
    "radius_in_kms": 6378,
}

earth_data = client.vertex.create(
    label=earth_label,
    properties=earth_properties
)
```

#### client.vertex.get\_or\_created\(label=None, properties=None\)

| param name | param description |
| :--- | :--- |
| label | Vertex label |
| properties | key, value pairs of properties data |

```python
earth_label = "Planet"
earth_properties = {
    "name": "Earth",
    "radius_in_kms": 6378,
}

earth_data_get_or_created = client.vertex.get_or_create(
    label=earth_label,
    properties=earth_properties
)
```

#### client.vertex.read\_one\(element\_id\)

| param name | param description |
| :--- | :--- |
| element\_id | vertex id |

```text
earth_data = client.vertex.read_one(earth_data.id)
```

