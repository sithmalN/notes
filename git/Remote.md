![[Pasted image 20240216204634.png]]


- `git init`
- `git remote add origin <url>` - setup remote
- `git remote` - show remotes
- `git remote -v` - show remotes
- `cat .git/config`
- `git remote rm <remote_name>` - delete remote
- `git push -u origin <remote_branch>`  - recommend to use `u` when first creating remote
- `git branch -r` - show remote branches
- `git branch -a` - show all the branches
- `git clone <url> <directory_name(optional)>` - clone remote repository
- `git fetch` - sync the remote
- TIP : fetch before work, fetch before push
- `git fetch + git merge = git pull`
- `git branch <branch> <origin_branch>` - checkout remote branches
- if git reject the push - fetch, merge and push again
- `git push origin :<remote_branch>` - delete remote branch(old method)
- `git push origin --delete <remote_branch>` - delete remote branch


### Best practices (Example)

- my point of view

![[Pasted image 20240216214808.png]]

- collaborator point of view

![[Pasted image 20240216215104.png]]

- my point of view

![[Pasted image 20240216215248.png]]

