
### Logging Option

- Log is the primary interface to Git
- Log has many option
- Sorting, filtering, output formatting
- use `git help log`

Useful commands:
- `git log filename.txt` - List commits that changed filename.txt
- `git log -p`/`git log --patch` - list commits as patches (diffs)
- `git log -L 100,150:filename.txt`/`git log -L 100,_50:filename.txt` - List changes to lines 100-150 in file name


- hit h for help in log mode
### Blame

- browse annotated file
- `git blame -L 100,150 filename.txt
- `git blame filename.txt`
- `git blame -w filename.txt` - Ignore whitespace
- `git annotate` - similar to blame but different output format

### Bisect
- Find the commit that introduced a bug or regression
- Mark last good revision and first bad revision
- Reset code to midpoint
- mark as good or bad revision
- repeat

- `git bisect start`
- `git bisect good <treeish>`
- `git bisect bad <treeish>`
- `git bisect reset` - quit


