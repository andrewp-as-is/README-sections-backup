```bash
$ find . "*.app" | xargs python -m mac_app_env .env
```

paths with spaces:
```bash
$ find . "*.app" -exec python -m mac_app_env .env {} \;
```
