```python
import launchctl

for job in launchctl.jobs():
    print("%s %s %s" % (job.pid if job.pid else "", job.status, job.label))

launchctl.job("com.apple.Finder")
{...}
```
