```
folder
├── __init__.py
├── module1.py
├── module2.py
└── module3.py
```

`__init__.py`
```python
import import_submodules

import_submodules.import_submodules()           # import moduleX
```
```python
import import_submodules

import_submodules.import_all_from_submodules()  # from moduleX import *
```
