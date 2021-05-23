```python
>>> import mac_comment
>>> mac_comment.write(__file__,"comment")
>>> mac_comment.read(__file__)
'comment'
```

```bash
$ python -m mac_comment ~ "CLI works too"
$ python -m mac_comment ~
CLI works too
```
