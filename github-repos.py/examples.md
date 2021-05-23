delete orphaned repos (if basename = repo name)

```bash
$ cd ~/git/owner
$ python -m github_repos | awk -F '/' '{print $2}' | grep -v -iF "$(ls -1)" | xargs python -m github_delete
```
