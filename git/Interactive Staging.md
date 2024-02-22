- `git add -i` - interactive mode


### Patch mode

- allows staging portion of change file
- "Hunk": an are where two files differ
- Hunks can be staged, skipped, or split into small hunks

- `git add --patch/ git add -p`
- `git stacs -p`
- `git reset -p`
- `git restore -p`
- `git commit -p`

### Split a Hunk

- Hunks can contains multiple changes
- Tell Git to try to split a hunk further
- Require one or more unchanged lines between changes
