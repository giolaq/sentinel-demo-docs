# Fixable documentation

Missing Python stdlib import:
```python
import json
print(json.dumps({"hello": "world"}))
```

Python 2 print:
```python
print("hello from Python")
```

Removed collections alias (indented fence):
  ```python
  import collections.abc
  import collections
  print(isinstance({}, collections.abc.Mapping))
  ```

Missing Node builtin:
```javascript
import path from 'node:path';
console.log(path.join('hello', 'world'));
```

Mixed module modes:
```javascript
import os from 'node:os';
import path from 'node:path';
console.log(path.sep, os.platform());
```

No deterministic fix:
```python
raise ValueError("application-specific failure")
```

Already passing:
```javascript
console.log('all good');
```
