# Linux Commands Cheat Sheet

## Find file in filesystem
Finds file in the whole filesystem

```bash
find / -type f -name "*.ext"
find / -name file.txt -path '*/dir-name/*' 2>/dev/null
```

- `2>/dev/null`: Redirects error messages to /dev/null to suppress permission denied messages.
