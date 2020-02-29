# HelloWorld


Things to pratice:
1) Clone the repository to your local directory
2) Start a new branch and start making commits on this branch (all this is done LOCALLY. Use git branch and git commit)
3) Try to push this branch to the remote repo using the git push command.
4) Submit a pull request to merge this branch into the main one (use github instead of git for a pull request)

Please try to use git to accomplish these tasks using git.

Useful git commands:

git clone <url of project> : creates local copy of project
git branch <branch name> : Creates new branch. Note that this only creates a new branch but does
  NOT automatically move the HEAD pointer to the new branch (see git checkout)
git checkout <branch name> : moves the HEAD pointer to the branch
git status : Shows what branch you're on and all the staged and unstaged files/changes. Note that ONLY staged
  files/changes will be saved in a commit
git log --oneline --decorate --graph --all : prints out a graph of all the commits in the repo and shows their respective
  branches.
git add <filename as specified in git status> : adds a file/modification to the stage
git add -A : adds ALL files to the stage
git commit -m "<insert commit message here>" : commits all staged files
git push <remote> <branch name> : pushes the branch from the local repo to the remote repo (i.e. your local
  branch is now on the internet)
git fetch <remote> : copy all new branches and commits from the remote repo to your local repo
git remote -v : view the names and urls of all github projects you saved.
git merge <branch name> : merges the branch with the current branch (to change current branch, use git checkout)
  
Steps from creating a branch to submitting a pull request:
-first use git fetch to incorporate all new changes in your local repo
-use git log to get a sense of the structure of the repo
-use git checkout to go the branch you want to work on
-create new branch using git branch and shift to that branch using git checkout
-use git status constantly to make sure you're on the right branch
-now, start making changes to your files. 
-use git status again to look for staged files and unstaged files.
-add all the files you want to be staged using git add. If you want to all files, use git add -A.
-Once you're satisfied with the changes, use git commit to save those changes.
-Once you're satisfied with your branch, push the branch to the remote repo using git push.
 If you don't know what your remote's name is, use git remote -v.
-Use git push to push your local branch to the remote repo
-Submit a pull request to merge this branch with another branch
