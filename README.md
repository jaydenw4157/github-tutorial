# GitHub Tutorial

##### _by Jayden Weston_

---
## Git vs. GitHub
Git is a tool used by many people to take snapshots/take a picture of thier code and doesn't require github to be usable. Github is simialr to git but you can save changes/snapshots to your cloud and be able to see and track your changes on git. Also, github makes it easier for people to collaborate/work on files with opther programmers.

---
## Initial Setup
Git init is used when your first create a repository using git to initialize git in your newly made repository.
To use git init, you:
1. Create a repository using `mkdir repo-name`
2. Use `cd repo-name` to go into your new repository
3. Use `git init` to initialize your repository

---
## Repository Setup
When working on a repository it is **extremely** important to make sure it is connected to a local repository. Without doing this, it will be **incredibly** difficult to do any work on github whatsoever. The steps for creating a repository in github are:
* Go to github and log in 
* Click on **your profile** then click on **repositories**
* In the top right corner, click on **new**
* Create a name for yor repository, then click **create repository**
* Go to _push an existing repository from the command line_
* Copy and paste `git remote add origin git@github.com:your-name-here/repo-name.git`

---
## Workflow & Commands
Whenever you are working on git, the main commands you would to edit are:
* `git add file.md` will add the file you edited to the stage to be committed
* `git add.` will add all files changed to your current/entire repository, while `git add --all` will include all changes made, including deleted files
* `git commit -m "message"`will take a snapshot of the files on stage. The message should describe what you did/ whqt you changed in the snapshot 
* ` 



---
## Rolling Back Changes