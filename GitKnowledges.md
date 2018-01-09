

Git knowledges:

Git Workflow

Proposed routine for working on features.
1. Clone code from master with a new local branch name according to feature. git clone https://github.com/lwrnczeng/GitDrill.git GitdrillFeature
2. Make changes. 
3. Commit 
4. Push to a branch named according to the feature.



==
make pull request
rebase


git pull --rebase origin master
Rebasing works by transferring each local commit to the updated master branch one at a time. This means that you catch merge conflicts on a commit-by-commit basis rather than resolving all of them in one massive merge commit.




Github

git checkout vs pull vs clone.

Git clone is the equivalent of these three commands:
git init
git remote add origin [url]
git pull origin master

Git pull is the equivalent of these commands:
git fetch
git merge origin/master

The 'origin' here is the name of a 'remote'
=====


To add a new branch remotely:
git push <remote-name> <local-branch-name>:<remote-branch-name>  e.g.
git push origin master:myRemotelySpecifiedBranchName  // it worked on Github


https://www.youtube.com/watch?v=0fKg7e37bQE
git pull/ git status / git add / git commit / git push   // set mac keychain access information
common steps in normal work:   git pull/ make changes / git add -A  / git commit  / git push
! For push a new local project, refer to https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/ It worked!
(…or create a new repository on the command line
echo "# SwiftDrilling" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/lwrnczeng/SwiftDrilling.git
git push -u origin master
…or push an existing repository from the command line
git remote add origin https://github.com/lwrnczeng/SwiftDrilling.git
git push -u origin master)