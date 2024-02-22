- Take commits from a branch and replay them at another point, most often at the end of another branch
- Useful to integrate recent commits without merging
- Maintains a cleaner, more linear project history
- Ensures topic branch commits apply cleanly

### Before Rebase

![[Pasted image 20240220203121.png]]

### After Rebase

![[Pasted image 20240220203201.png]]


#### Usage

- `git rebase main` - Rebase current branch to tip of main
- `git rebase main <branch_name>` - Rebase branch to tip of main

- `git rebase --onto newbase upstream branch`
	- ex: `git rebase --onto ecommerce main new_feature`
		Telling git to rewind `new_feature` branch until it gets to the point  were it merges with the main branch and replay the commits on the ecommerce branch.
- `git merge-base main new_feature` - Return commit where topic branch diverges

## Merging Vs. Rebasing[[Merging Vs. Rebasing]]


### Interactive Rebase

- pick, drop
- reword, edit
- squash, fixup [[Squash commits]]
- exec

`git rebase -i main` - interactive mode

### Pull Rebase

- `git pull -r`
- `git pull --rebase`
- `git pull -rebase=preserve`
- `git pull--rebase=interactive`