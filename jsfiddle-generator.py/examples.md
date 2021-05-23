create `demo.css`, `demo.js`, `demo.details` in every dir with `demo.html`:
```bash
$ find . -name "demo.html" -exec python -m jsfiddle_generator.repo {} \;
```

---
create jsfiddle repo files in every empty dir:

`find . -not -path '*/\.*' -type d -links 2 -exec python -m jsfiddle_generator.repo {} \;`

---
paths with spaces:

OS|speed|command
-|-|-
any|slow|`find ... -exec python -m jsfiddle_generator.repo {} \;`
Linux|fast|`find ... -print0 \| xargs -d '\n' python -m jsfiddle_generator.repo`
macOS|fast|`find ... -print0 \| xargs -0 python -m jsfiddle_generator.repo`
