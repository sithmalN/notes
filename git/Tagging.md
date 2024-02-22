- Tags allow marking points in history as important.
- A named reference to a commit
- Frequently used to mark software release versions (v1.0, v1.1, v2.0)

### Lightweight tag

- `git tag <tag_name> <commit_hash>`

### Annotated tag (most common)

- `git tag -am "Version 1.0" v1.0 <commit_hash>`

### Delete a tag

- `git tag -d v1.0/git tag --delete v1.0` - delete tag not the references commit by the tag.

### List tags

- `git tag -l/git tag --list` - list all
- `git tag -l "v2*` - list tags beginning with "v2"
- `git tag -n` - show annotated tags

### Push Tags to a Remote

- git push does not transfer tags
- `git push origin <tag_name>`
- `git push origin --tags` - push all tags to remote
- `git feth` - fetch tags and commits
- `git fetch --tags` - Fetch only tags
-  `git push -d origin <tag_name>` - delete remote tag
- 