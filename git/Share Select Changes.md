
- Apply the changes from one or more existing commits
- Each commit targeted will become a new commit on the current branch
- Conceptually similar to copy and paste
- New commits have different SHAs


- `git cherry-pick <SHA>`/ `git cherry-pick <SHA>..<SHA>`
- Use `--edit` , `-e` to edit the commit message.

## Resolve cherry picking conflicts

- cherry-pick, then resolve conflicts, then add changed files using `git add <file_name>`, then `git cherry-pick --continue`

## Create diff patches

- Share changes via files
- Useful when changes are not ready for a public
- Useful when collaborators do not share a remote
- Discussion, review, approval process
- `git diff <SHA_BEFORE_THE_REQUIRED_RANGE>..<TO_SHA> > output.diff`- create a diff patch

## Apply Diff Patches

- `git switch <branch_name> <from_commit(sha)>` - create a branch
- `git apply <output.diff`

## Create formatted patches

- `git format-patch <from_hash>..<to_hash>` - Export all commit in the range
-  `git format-patch main`/ `git format-patch main..HEAD` - Export all commits on current branch or that are not in main branch
- `git format-patch -1 <commit_hash>`
- `git format-patch <from_hash>..<to_hash> -o ~/feature_patches` - Put patches file into a directory. if not directory in there it will create a one
- `git format-patch <from_hash>..<to_hash> --stdout > feature.patch` - Output patches as a single file

## Apply formatted patches

- Extract author, commit message, and changes from a mailbox message and apply them to the current branch
- Similar to cherry-picking: same changes, different SHAs
- `git am <patch_file>` - Apply single patch
- `git am <*.patch>` - Apply all patches in a directory
