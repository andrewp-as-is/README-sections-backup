`README.md.sh`
```bash
#!/usr/bin/env bash

[ -e setup.py ] && echo "badges ..." && cat <<EOF
### Installation
pip install name
EOF

readme-section ".readme/pros.md"
readme-section ".readme/how.md" "How it works"
readme-section ".readme/examples.md"
readme-section ".readme/links.md"               # optional. empty if file not exists
```

```bash
$ bash -l README.md.sh > README.md
```
```markdown
badges ...

### Installation
pip install name

### Features
features.md content ...

### How it works
how.md content ...
```
