## Git and GitHub

Git -> version control system
meaning we can switch between the
versions of our created projects

GitHub -> a free open source for using
git software

Uses: sharing the source code,
deployment,
version control.
necessary tool every programmer shoud know!

## git repositories:

Its like folders in the local maching
but repo(shor for repositories) are at the global cloud
meaning we can access it from anywhere with our credentials

## create a git repository:

1. go to github website, sign it to your account
2. you can see a create repository button
3. by clicking it, you can name your repo, set its visibility.
4. congrats! a new repo has been created.

## upload files from local machine to github repo:

1. initialize an empty .git file in the local mechine folders
   whose contents must be pushed to the github repo

_git init_

2. add the necessary files

_git add file_name_
_git add ._ (to add everything from your folder)

3. commit the changes to the stagging area

_git commit -m "commit message"_

4. create the main branch

_git branch -M main_

5. connect the local .git file to the github repository

_git remote add origin your_repo_url_

6. push the changes to the repo

_git push -u origin main_

7. congrats! you have moved/pushed your first file to github

NOTE: if you made any changes or updates to the folder (like adding a new file,
changing the contents of it), these changes are tracked by the .git file
and you have to push the changes to the repo, so that it remain upto date.

_git add ._
_git commit -m "commit message"_
_git push_

## cloning and pull request

if you need to get the files of other repositories, you can clone them to your
local machine

_git clone repo_url_

by this command the entire repo can be cloned down to your local machine
once you cloned the repo, the changes in that folder can be pulled to your local device

_git pull_

this command updates the code in your local device

## git branch and merging

branch : the branch 'main' is the root branch
if any changes in the project we are
currently working we need to create a
new branch.

command for creating branch:
_git branch branch_name_

switch to the created branch:
_git checkout branch_name_

alternative for the above command
_git switch branch_name_

shortcut for creating and switch to the new branch
_get checkout -b branch_name_

after creating a new branch (make some changes)
push the changes to the new branch

_git add ._
_git commit -m "commit message"_
_git push origin branch_name_

now you can see the created branch in the git hub repo

after making changes, we have to merge with the main branch

first switch to the main branch
_git switch main_
_git checkout main_

merge with the main branch
_git merge branch_name_

push the changes to the main branch
_git push -u origin main_

now the work of the new branch is finished
we can delete it from the local and from the repo

_git branch -d branch_name_ -> delete from local machine
_git push origin --delete branch_name_ -> delete from the cloud repo
