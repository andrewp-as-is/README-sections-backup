download to current folder
```bash
$ pypi-download Django
$ pypi-download Django 3.0.0
```

download to temp folder and get filenames
```bash
$ filenames="$(cd "$(mktemp -d)" && pypi-download Django && find . -type f)"
```
