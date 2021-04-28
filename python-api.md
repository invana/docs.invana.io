# Python API User Guide

### Installing Python SDK for Invana Engine

```
$ pip install invana-engine
```

### Connecting to Invana Engine

```python
from invana_engine.gremlin.client import InvanaEngineClient

gremlin_server_url = "ws://127.0.0.1:8182/gremlin"
client = InvanaEngineClient(gremlin_server_url=gremlin_server_url)
```

### Creating Vertex

```python
earth_label = "Planet"
earth_properties = {
   "name": "Earth",
   "radius_in_kms": 6378,
   "average_orbital_speed_in_kms": 29.78
}

created_data = client.vertex.create(
                label=earth_label,
                properties=earth_properties
)
```



