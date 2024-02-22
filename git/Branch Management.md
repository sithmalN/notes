
## Force Push

- force push = replace remote

## Identify the merged branches

- `git branch --merged`
- `git branch --no-merged`
- `git branch -r --merged`

## Prune Stale Branches

- Delete all stale branches
- Stale branch: a remote-tracking branch that no longer tracks anything because the actual branch in the remote repository has been deleted
- 3 types of branches - 
	- Branch on the remote repo(bugfix)
	- Local snapshot of the remote branch (origin/bugfix)
	- Local branch, tracking the remote branch (bugfix)
- `git remote prune origin --dry-run` - dry run
- `git remote prune origin` - prune
- short cuts: (prune, then fetch)
	- `git fetch -p/git fetch --prune`
- edit config for always prune before fetch
	- `git config --global fetch.prune true`