# Modelling using OGM

### Create Vertex Model

```
from invana.ogm import models, fields


graph = InvanaGraph("ws://megamind-ws:8182/gremlin", traversal_source="g")


class Project(models.VertexModel):
    graph = graph
    properties = {
        'name': fields.StringProperty(max_length=10, trim_whitespaces=True),
        'description': fields.StringProperty(allow_null=True, min_length=10),
        'rating': fields.FloatProperty(allow_null=True),
        'is_active': fields.BooleanProperty(default=True),
        'created_at': fields.DateTimeProperty(default=lambda: datetime.now())
    }
 
```
