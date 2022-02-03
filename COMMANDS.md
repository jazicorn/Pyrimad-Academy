## Commands

### About
Commands for navigating and updating submodules

> ⚠️ ***!!!Remember!!!*** 
> 
> ⚠️ I choose to **not** update submodules *directly*.
> 
> ⚠️ Do **not** use this repository to update or edit submodule files.

### Add Submodule
```bash
# 💡 *clones submodule repo, and creates folder*
git submodule add <remote_url> <destination_folder>
```
```bash
# 🚨 For Cloned Repositories:
git submodule update --init --recursive
```
```markdown
💡 **Edit .gitmodules file:** *add branch of submodule for Pyramid Academy to pull from*
[submodule "<submodule>"]
    path = <destination_folder>
    url = <remote_url>
    branch = main
```
```bash
# 🚨 *Make sure to git add, commit, and push after submodule commands*
git add .

git commit -m "project <submodule> added"

git push
``` 

### Update Submodule (No Merge)
```bash
# 💡 *updates project from most current remote submodule commit*
git submodule update --init --recursive --remote <submodule>
```
```bash
# 🚨 *Make sure to git add, commit, and push after submodule commands*
git add .

git commit -m "<submodule> updated"

git push
```

### Refs
- [Cheatsheet](https://codex.so/git-submodules-cheatsheet)
- [git-scm Docs: Submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules)
- [Article: devconnected](https://devconnected.com/how-to-add-and-update-git-submodules/)
- [Article: Vogella](https://www.vogella.com/tutorials/GitSubmodules/article.html)
