| Merging | Rebasing |
| ---- | ---- |
| Adds a merge commit | No additional merge commit |
| Nondestructive | Destructive: SHA changes, commits are rewritten |
| complete record of what happened and when | No longer a complete record of what happened and when |
| Easy to undo | Tricky to undo |
| Logs can become cluttered and nonlinear | Logs are linear and cleaner |


- **Thou shalt not rebase a public branch** 

### How to Choose

- Merge to allow commits to stand out or to be clearly grouped
- Merge to bring large topic branches back into main
- Rebase to add minor commits in main to a topic branch
- Rebase to move commits from one branch to another