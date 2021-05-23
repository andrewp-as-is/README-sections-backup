```bash
$ travis-exec travis status -r {}
$ travis-exec python -m travis_cron.add {} master daily no
$ travis-exec python -m travis_env.set {} WEBHOOK_URL "$WEBHOOK_URL"
```
