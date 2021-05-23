```python
import task.setup
from task.classes import Task

class Stand_up(Task):
    def todo(self):
        return not self.elapsed or self.elapsed >= 30*60
```

```bash
$ python -m task.scan
$ python -m task.update
```
