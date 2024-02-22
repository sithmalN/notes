- move HEAD pointer to a specific commit
- three types:
	- soft
	- mixed
	- hard

### Soft 
- moved HEAD pointer
- does not change staging index
- Does not change working directory
- usage `git reset --soft <tree-ish>`

### Mixed
- Moves HEAD pointer
- changes staging index to match repository
- Does not change working directory
- usage `git reset --mixed <tree-ish>`
- default choice

### Hard
- Moves HEAD pointer
- changes staging index to match repository
- change working directory to match repository
- usage `git reset --hard <tree-ish>`