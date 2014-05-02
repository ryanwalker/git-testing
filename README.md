Get Started
===========

1. Download Git - http://git-scm.com/downloads
2. Signup at github.com
3. Turn on 2-factor Authentication - https://github.com/blog/1614-two-factor-authentication
4. Setup SSH key to be able to clone, push, etc. to GitHub - https://help.github.com/articles/generating-ssh-keys 
5. Excellent Git Tutorial - https://www.atlassian.com/git/tutorial/git-basics
6. (optional) Download a git gui client such as http://www.sourcetreeapp.com/ 

//Clone a repository (this is a public repo I have created)
git clone git@github.com:ryanwalker/git-testing.git
 
//View branches branches
git branch //local branches, branches created locally that don't exist on the remote repository.
git branch -r //remote branches, or branches that already exist from the remote repository we just cloned
git branch -a //all branches
 
//Checkout a remote branch
git checkout <remoteBranchName>
 
//Create and checkout a local branch
git checkout -b <myFeatureBranchName>
 
//add un-versioned files or stage files for commit
git add <fileName>
git add . //stages all files for commit
 
//View staged, changed and untrcked files
git status
 
//commit
git commit //Commits all staged files
git commit -m 'Commit Message Here'
git commit -a //Commits all changed files
 
//View your remote repository connections so we can push our changes up there
//Normally you will only have one remote, the origin
git remote
gite remote -v //shows the repository url next to the name of the remote
 
//push your committed changes from your local repository up to the remote repository
//origin is an alias of the remote repository, <branchName> is the branch to push to.
git push origin <branchName>
 
//Go to github and see your feature branch up there
 
//pull request
//Log into GitHub and go to the repo, you should see
 
 
//branch commands
git branch //show local branches, * will be next to your current active branch
git branch -r //show remote branches
git branch -a //show all branches
git branch <branchName> //create a local branch
git branch -d <localBranch> //delete local
git push origin :<remoteBranch> //delete remote branch
 
//Merge changes from one branch into the current branch
git merge <branch> //Changes from <branch> will be merged into the branch you are working on. 
