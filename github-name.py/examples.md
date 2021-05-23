```bash
$ git remote add github git@github.com:owner/repo.git
$ python -m github_name .
owner/repo
$ python -m github_name . | awk -F"/" '{print $1}'
owner
$ python -m github_name . | awk -F"/" '{print $2}'
repo
```

```python
>>> import github_name
>>> github_name.get()
'owner/repo'
```

print repo name for every repo:
```bash
$ find ~/git -type d -mindepth 1 -maxdepth 1 -exec python -m github_name {} \;
```
