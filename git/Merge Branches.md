- `git merge <target_branch>`
- `git branh --merged`
- tip : all ways checkout the receiving branch


### Resolve merge conflicts

#### useful commands

- `git merge --abort`
- `git diff --color-words <branch>..<compaired_branch>`
- `git show --color-words` - show differences in the current branch
- `<<<<HEAD` - one we want to keep
- `==============` - separator
- `>>>>>><branch_name>` (ending marker)


### Strategies to reduce conflicts

- keep lines short
- keep commits small and focused
- Beware stray edits to whitespaces
- merge often
- track changes to masters