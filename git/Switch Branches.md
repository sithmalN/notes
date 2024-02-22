 - `git checkout branch_name`
## Create and Switch branches

- `git checkout -b new_branch_name` - create and checkout
- `git switch` also used to switch between branches. but checkout can also perform different actions such as switching branches, checking out specific commits(detached HEAD state), or working with files.

## Switch branches with uncommitted changes

- cannot switch if changes in working directory conflict
- can switch if changes in working directory could be applied without conflict
- can switch if files are not being tracked
### How to Do : 
- commit the changes to the current branch
- Remove the changes, checkout the file again
- Stash the changes