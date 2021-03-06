# GitHub Tutorial

 _by Jayden Weston_

---
## Git vs. GitHub
Git is a tool used by many professionals to take snapshots/take a picture of their projects. Git is seperate from Github. Github is similar to Git but you can save changes/snapshots of projects to the cloud/internet. This makes it easier for people to collaborate on files with other professionals. 

---
## Initial Setup
_Your not teaching commandline, Your teaching git and GitHub Assume they already know it_
Git init is used when you first create a repository using Git. To initialize Git in your newly made repository.
To use git init, you:
1. Create a repository and go into your new repository
2. Use `git init` to initialize your repository

---
## Repository Setup
When working on a repository it is **extremely** important to make sure it is connected to a local repository. Without doing this, it will be **incredibly** difficult to do any work on github whatsoever. The steps for creating a repository in github are:
* Go to github and log in 
* Click on **your profile** then click on **repositories**
* In the top right corner, click on **new**
* Create a name for yor repository, then click **create repository**
* On the top of the screen there is an option for https or ssh, make sure you have ssh selected for the link
* Go to **push an existing repository from the command line**
* Copy and paste `git remote add origin git@github.com:your-name-here/repo-name.git`

---
## Workflow & Commands
1. Whenever you are working on git, the main commands you would to edit are:
* `git add file.md` will add the files you edited to the stage to be committed
* `git add.` will add all files changed to your current/entire repository, while `git add --all` will include all changes made, including deleted files
* `git commit -m "message"`will take a snapshot of the files(which should be green) on stage. The message should describe what you did/ what you changed in the snapshot 
* `git push -u origin master` is used to push your commits onto your repo in github
* If you ever initialize in the wrong repository/folder, use `rm -rf .git` to remove the hidden folder

2. While coding in a repository here are some commands used in order to keep track of your work:
* `git status` shows which files are staged to be committed
* `git log` shows a list of all previous commits to keep track of your work
* `git diff` is used for you to see the difference between your current code and all of your previous commits

3. When forking and cloning a repository, the steps to do it are:
* Use `git remote -v` to show which remote repos are attached/connected to your local repo
* If you are looking at someone's repo, press the button in the top-right corner that says `fork`
* Once you fork the repo, press **clone or downlaod** and copy the ssh key
* Go to your workspace and put `git clone` then paste the ssh key link

4. However, you won't be able to push or pull because the repository isn't yours, just a copy to someone else's. To solve that you have to send a pull request. Yo do that by:
* Commiting your change to a file
*   After that, got to github and click on **new pull request** 
*   When you click on new pull request, it should show what your were going to commit, make sure its there or you made a mistake
*   Finally, press **create pull request** then the owner of the repo can decide whether to accept or deny the pull request
*   If you accept a pull request, use `git pull` which brings changes from your remote repo to the local repo

---
## Rolling Back Changes
When coding using git, it is extremely diifficult to undo and add or commit. But luckily there are some commands you can ue to undo such as:
* `git reset HEAD filename` allows you to unstage a file if you add a broken file
* `git reset HEAD~1` is used to undo a commit a file but keep the changes 
* `git reset --soft HEAD~1` means to undo commits but leaves your files alone **and** your index
* `git reset --hard HEAD~1` deletes your adds, commits, and edits and takes you back to your previous commit. Note: This is a **very dangerous command**, so it should be used wisely and when you are the only person using the repository
* `git checkout --filename` allows you to revert/return to a previous commit 
* `git push -force origin` will "force" push to a previous commit, deleting your previous git push. Make sure you are the only user/owner of your repository. If someone else has pulled it, that repository will become corrupted
