- SHA-1 Hash
	- 40 character string
	- `git show de14` - show commit reference
	- must use minimum 4 chars
- Head Pointer
	- .git/HEAD
	- `git show HEAD`
	- `git log`
- Ancestry
	- go to the parent
		1. method 1 : - use `^`
			 ex:  `git show HEAD^` (show parent)
				`git show HEAD^^` (show grand parent)
		2. method 2: use `~`
			ex: `git show HEAD~1` (show parent)
				`git show HEAD~2` (show great parent)\
- Tree list
	- usage `git ls-tree <tree-ish>` 
		- got list contains blog(binary large object/files and tree(directory))
- commit log
	- `git log --since=2023-01-01` or `git log --until="3 days ago"` or `git log --after=2.weeks --before=3.days`
	- `git log --grep="Initial"`
	- `git log --author="nimthaka"`
	- `git log a3lkjslkj..HEAD` - from that commit to HEAD
	- `git log filename
- format the commit log
	- `git log -p` 
	- `git log --stat`
	- `git log --format= `
		- `oneline/short/medium(default)/full/fuller/email/raw`
	- `git log --graph`
	- tip : `git log --graph --all --oneline --decorate`