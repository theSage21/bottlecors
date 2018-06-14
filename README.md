BottleCors
===========


`pip install bottlecors` and then

```python
from bottle import Bottle
from bottlecors import wide_open_cors, abort


app = Bottle()
app = wide_open_cors(app)

@app.get('/')
def home():
    abort(404, 'msg')
```
