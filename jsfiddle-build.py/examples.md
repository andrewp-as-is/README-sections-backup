```bash
$ find . -name "*.html" ! -name "build.*" | xargs python -m jsfiddle_build
```

---
paths with spaces:

OS|speed|command
-|-|-
any|slow|`find . -name "*.html" ! -name "build.*" -exec python -m jsfiddle_build {} \;`
Linux|fast|`find . -name "*.html" ! -name "build.*" -print0 \| xargs -d '\n' python -m jsfiddle_build`
macOS|fast|`find . -name "*.html" ! -name "build.*" -print0 \| xargs -0 python -m jsfiddle_build`
