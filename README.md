# tipsAndTricks

## Bash

### Trim trailing whitespaces

detection
```bash
find . -type f -exec egrep -l " +$" {} \;
```

removal
```bash
find . -name "*.java" -type f -print0 | xargs -0 sed -i 's/[[:space:]]*$//' 
```
