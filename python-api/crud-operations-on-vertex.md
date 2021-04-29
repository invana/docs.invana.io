# CRUD Operations on Vertex

### client.vertex.create\(label=None, properties=None\)



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

### client.vertex.get\_or\_created\(label=None, properties=None\)

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

### client.vertex.read\_one\(element\_id\)

| param name | data type | param description |
| :--- | :--- | :--- |
| element\_id | str or int | vertex id |

```python
earth_data = client.vertex.read_one(earth_data.id)
```

### client.vertex.read\_many\(label=None, query=None, limit=None, skip=None\)

| param name | data type | param description |
| :--- | :--- | :--- |
| label | string | Vertex label |
| query | dict | key, value pairs of properties |
| limit | int | number of items to limit |
| skip | int | number of items to skip |

```python
planets_data = client.vertex.read_many(label="Planet", query={"name": "Earth"}, limit=10, skip=1)
```

### client.vertex.update\(element\_id, properties=None\)

| param name | data type | param description |
| :--- | :--- | :--- |
| element\_id | str or int | vertex id |
| properties | dict | key, value pairs of properties |

```python
earth_new_properties = {
    "average_orbital_speed_in_kms": 29.78
}
earth_data_updated = client.vertex.update(earth_data.id, properties=earth_new_properties)
```

### client.vertex.delete\_one\(vertex\_id\)

| param name | data type | param description |
| :--- | :--- | :--- |
| vertex\_id | str or int | vertex id |

### client.vertex.delete\_many\(label=None, query=None\)

| param name | data type | param description |
| :--- | :--- | :--- |
| label | str | vertex name |
| query | dict | key, value pairs of properties |

```text
client.vertex.delete_many(query={"name": "Earth"})
```

### client.vertex.read\_in\_edges\_and\_vertices\(vertex\_id, label=None, query=None, limit=None, skip=None\)

| param name | data type | param description |
| :--- | :--- | :--- |
| vertex\_id | str or int | vertex id |
| label | str | vertex name |
| query | dict | key, value pairs of properties |
| limit | init | how many nodes data should be returned in the response |
| skip | int | how many nodes should be skipped in the returned response |

```text
client.vertex.read_in_edges_and_vertices(earth_data.id, limit=0, skip=0)
```

#### 

