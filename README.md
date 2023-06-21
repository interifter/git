# git command favorites

## Use Cases

```bash
### Check Out Branch From Remote

# Use this if you want to check out a branch that already exists in one, or more, remotes.
# Typically more useful for multi-remote setups
# https://stackoverflow.com/a/1783426
# git > 2.23
git remote -v # to list your current remotes, and their names
git fetch <remote name>
# optional, if you want the list
# git branch -v a
git switch -c <branch name> <remote name>/<branch name>

### Check Out Branch Without History
# Use this if you want a clean branch and have nothing clean in your local env
git checkout --orphan <branch name>

### Push to different remote
# Good if you are using a fork/merge model
# Note: The remote branch name can be new/not exist on remote
git push <remote name> <local branch name>:<remote branch name>
```
