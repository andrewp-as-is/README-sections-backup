```python
>>> import webloc
>>> webloc.write("path.webloc","https://www.google.com/")
>>> webloc.read("path.webloc")
'https://www.google.com/'
```

```bash
$ python -m webloc "path.webloc" "https://www.github.com/"
$ python -m webloc "path.webloc"
https://www.github.com/
```

```bash
$ webloc file.webloc https://github.com/
$ webloc file.webloc
https://github.com/
```
