# notes

these are rough notes about devops 

## how to generate pdf

use pandoc (and all its dependencies)

run command to generate pdf file:

```bash
pandoc --pdf-engine=xelatex --highligh-style zenburn --table-of-contents -s devops.md -o devops.pdf
```