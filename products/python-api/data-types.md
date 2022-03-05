# Data Types

### StringProperty

```python
// Some code

class Project(VertexModel):
    graph = graph
    properties = {
        'name': StringProperty(min_length=1, max_length=10, trim_whitespaces=True)
    }
```

### **IntegerProperty**

```python
// Some code
from invana.ogm import fields  
class Project(VertexModel):
    graph = graph
    properties = {
        'age': fields.IntegerProperty(min_value=1, max_value=100)
    }
```

### FloatProperty

```python
// Some code
from invana.ogm import fields  
class Project(VertexModel):
    graph = graph
    properties = {
        'rating': fields.FloatProperty(min_value=1, max_value=100)
    }
```

### BooleanProperty

```python
// Some code
from invana.ogm import fields  
class Project(VertexModel):
    graph = graph
    properties = {
        'is_active': fields.BooleanProperty(default=True)
    }
```

### DateTimeProperty

```python
// Some code
from invana.ogm import fields  
class Project(VertexModel):
    graph = graph
    properties = {
        'created_at': fields.DateTimeProperty(default=lambda: datetime.now())
    }
```
