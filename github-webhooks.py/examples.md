```bash
$ cd path/to/repo
$ python -m github_webhooks.create "push" https://xxx.execute-api.us-east-1.amazonaws.com/run
$ python -m github_webhooks.names
web
$ python -m github_webhooks.urls
https://xxx.execute-api.us-east-1.amazonaws.com/run
$ python -m github_webhooks.delete "web"
```

`~/.github-webhooks.ini`
```
[name]
  url = https://xxx.execute-api.us-east-1.amazonaws.com/run
  events = push
```

```
$ python -m github_webhooks.init "name"
```
