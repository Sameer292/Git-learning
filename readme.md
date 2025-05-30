# Git commands

## Initializing git and basic commands

- **`git init`** Initializing a repo
- **`git status`** Status of the repo
- **`git branch`** Display branches
- **`git switch <branch-name>`** Switch branches
- **`git switch -c <branch-name>`** Create and switch branch
- **`git add <file>`** Stage an changed/modified file
- **`git add .`** Staged all modified files
- **`git commit -m 'message'`** Commit changes with a message
- **`git commit -am 'message'`** Stage and commit changes

## Reset, Revert and Restore

- **`git reset --soft <commit-hash>`** Softly resets branch to a specific commit & Keeps changes staged
- **`git reset --mixed <commit-hash>`** Resets branch to the commit & keeps changes unstaged
- **`git reset --hard <commit-hash>`** Resets branch to the commit and loses all changes after the commit
- **`git revert <commit-hash>`** Creates a new commit undoing the changes done in <commit-hash>
- **`git restore <file-name>`** Unstage a file and discard current changes to the file in current commit
- **`git restore .`** Unstage all changes in current commit

## Stashing

- **`git stash`** Save current changes in an temporary stack (stash). Can be reapplied/popped later.
- **`git stash apply`** Bring back the uncommited changes but don't remove from the stash.
- **`git stash pop`** Bring back the uncommitted changes and drop the stash from the stack.
- **`git stash list`** List current stashed items.

## Cherry-Picking

- **`git cherry-pick <commit-hash>`** Bring specific commit(changes) from other branch to current one.
- **`git cherry-pick --abort`** Abort current cherry-picking process.
- **`git cherry-pick --continue`** continue current cherry-picking process.
- **`git cherry-pick --quit`** Forget about the current operation in progress.
- **`git cherry-pick --skip`** Skip the current commit and continue with the rest of the sequence.
- **`git cherry-pick -n | --no-commit`** Stops automatically creating a new commit. Keeps changes staged and allows users to make custom commits.


- **`git rebase <branch-name>`** set the current branch's base to the tip of the <branch-name> branch.
- **`git rebase -i HEAD~<n>`** **Squashing** This allows us to merge the commits into one. <n> refers to the previous commits. Then change pick to squash of the commits you want to combine to one, then provide a commit message
- **`git rebase <branch-name>`** set the current branch's base to the tip of the <branch-name> branch.
- **`git remote add <alias> <url>`** Add remote repo
- **`git fetch`** Fetches any changes in the remote branch and keeps the changes uncommited to the local branch
- **`git merge`** Updates the Head pointer to reference the latest commit
- **`git pull`** fetches and merges the changes to the local branch
- **`git clone <url> `** Clone a remote repo
- **`git push <alias> <branch-name>`** Push to the remote repo
- **`git push --all <alias>`** Push all branches to the remote repo
- **`git branch -d <branch-name> `** Delete a local branch
- **`git push <alias> --delete <branch-name>`** Delete a remote repo
- **`git merge <branch-name> `** Merge a branch to the current one
- **`git remote -v`** List current remote
- **`ssh-keygen -t ed25519 -C "your_email@example.com"`** Generate ssh key
- **`git remote set-url origin <SSH-url>`** Update remote branch
- **`git checkout <commit-hash>`** Take a look at previous commits
- **`git checkout <current_branch-name>`** Go to the latest commit

