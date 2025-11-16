## Exercise 1

...bash
Creating repo:
mkdir advanceGit
cd advanceGit
git init
...

### Part 1: Refining Git History (10 Challenges)

...bash
//Missing File Fix:
$ git status : to see file that haven't been commited

//Editing Commit History:
$ git rebase -i HEAD~2 : Take you back to the last two commits
squash: To combine two or more commit.
edit: To edit your commit message.

$ git rebase --continue : To continue the rebase state after using $ git add .
$ git rebase --abort : To leave the rebase state, if something is worng.
$ git rebase --reset : To undo all changes.

//Dropping a Commit:
$ git reset --hard HEAD~1 :If the commit had'nt been push; This will discards or remove all working changes and move HEAD back to the previous commit before.

$ git reset --hard <sha1-commit-id> : This command is use to delete up to specific commit, but first run git log to get the hash id from the commit history.

$ git push origin HEAD --force : If you have already push your commit and you want to push again.

//Reordering Commits:

$ git rebase -i : Set the stage for interactive rebasing or editing your commit. And just change the positions.

//Cherry-Picking Commits:

$ git cherry-pick <sha1-commit-id> : First run $ git reflog and check the commit history, then pick the hash id, after checkout the branch that you want to apply the commit to.

$ git add .
$ git cherry-pick --continue: To continue the state of cherry-picking.

$ git cherry-pick --abort : To leave the state of cherry-picking.

$ git log --graph : If you want to see the visual history of the commmit.

$ git reflog : If you want to show the reference of all the commit.
...

### Part 2: Branching Basics (10 Challenges)

...bash

$ git branch <branch-name> : If you want to create a new branch.

$ git checkout <branch-name>: If you want to switch to another branch.

$ git checkout -b <branch-name>: If you want to create and switch to a new branch.


...
