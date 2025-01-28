# GitHub - Remove Commit History

```bash
git clone <link>
git checkout --orphan TEMP
git add -A
git commit -am "Initial commit"
git branch -D main
git branch -m main
git push -f origin main
```

```bash
#!/usr/bin/env bash
echo "Link: "
read link
git clone $link && cd $(basename $_ .git)
git checkout --orphan TEMP
git add -A
git commit -am "Initial commit"
git branch -D main
git branch -m main
git push -f origin main
$SHELL
```
