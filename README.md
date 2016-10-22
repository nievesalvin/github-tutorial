# GitHub Tutorial

_by Alvin Nieves_

---
## Git vs. GitHub
 Git is a version control software that takes "snapshots" of a programmers code  
 and keeps track of changes and modifications that have been made to the project   
 itself, while Github is a website where a programmer can send code to the cloud  
 so that the code itself lives elsewhere instead of locally. Github is also at the enter  
 of social coding, where a pethora of programmers can use eachothers' code as a  
 starting point to start their own project.  
 
 In order to work Github needs git, where as Git does not need GitHub to work  
 hence why "Git" can be found in the word "GitHub" and why "Github" is  
 not found in "Git."


---
## Initial Setup
When using Git, a programmer uses `git push` to move their code from 
a local directory to a remote repository. In order to do this, a 
programmer has to have a Github account.  

To set up a github account:
* Go to [Github](www.github.com)
* Click "Sign Up" and after filling out ones information click "Create Account"  
![](start-github.png)  

After making a Github account and a repository 





---
## Repository Setup



---
## Workflow & Commands
When using Git one must know all of the commands and what those 
commands tell the computer to do. Every command does
something different, and there is almost always a way to reverse what one did.  

##### Git Commands:
1. `git init`: creates a new repository and begins to track changes and modifications in files and folders.   
```bash
nievesalvin:~/workspace/practice $ git init
Initialized empty Git repository in /home/ubuntu/workspace/practice/.git/
```
2. `git status`: allows programmer to see what files have been modified since the last commit.  
```bash
nievesalvin:~/workspace/github-tutorial (master) $ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   README.md
        modified:   directions.md
        new file:   git-log-img.png
```
3. `git commit <filename> -m "message"`:this is used in order to keep a record of the changes that a programmer has made to a file. When one uses
git commit, it takes a "snapshot" and it sets a digital checkpoint, where 
it shows, when your code last worked.  
```bash
nievesalvin:~/workspace/github-tutorial (master) $ git commit -m "add image to git log"
[master 8329a3c] add image to git log
 3 files changed, 21 insertions(+), 6 deletions(-)
 create mode 100644 git-log-img.png
```  
4. `git add`: adds files to the "stage" so that the programmer can use `git init` in order to record changes. One 
can not commit before adding the files to the "stage."  
```bash
nievesalvin:~/workspace/github-tutorial (master) $ git add .
```
5. `git push`: is used to send commits from the local directory to a remote 
repository that lives on the cloud.  
```bash
nievesalvin:~/workspace/github-tutorial (master) $ git push
Warning: Permanently added 'github.com,192.30.253.112' (RSA) to the list of known hosts.
Counting objects: 5, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 48.27 KiB | 0 bytes/s, done.
Total 5 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:nievesalvin/github-tutorial.git
   b0663d4..8329a3c  master -> master
```  
6. `git clone`: is used by programmers to copy files from a remote repository
to a local one.  
7. `git diff`: is used so that a programmer can see what specific lines of 
code have been changed in a file.
```bash
nievesalvin:~/workspace/github-tutorial (master) $ git diff
diff --git a/README.md b/README.md
index 7d064c2..2a1d90e 100644
--- a/README.md
+++ b/README.md
@@ -59,5 +59,5 @@ to a local one.
 `git diff`: is used so that a programmer can see what specific lines of 
 code have been changed in a file.  
 `git log`: is used to see the number commits, author, message, and time 
-stamp. In order to get out of git log one must simply press 'q'
+stamp. In order to get out of git log one must simply press 'q'  
 ![](git-log-img.png)
\ No newline at end of file
```  
8. `git log`: is used to see the number commits, author, message, and time 
stamp. In order to get out of git log one must simply press 'q'  
```bash
nievesalvin:~/workspace/github-tutorial (master) $ git log
commit b0663d40a55bb4f2c75dc90ed9292f59a1b9809f
Author: nievesalvin <alvinn4392@hstat.org>
Date:   Fri Oct 21 16:02:30 2016 +0000

    add image
```  
##### Command Line Commands
* _ls_: is short for list, and list all of the files in a directory  
![](ls-img.png)
* _cd -directoryname-_: cd is short for change directory and essentially it is used to 
transfer a programmer from one folder to the next.  
![](cd-img.png)  
* _touch -filename-_: touch allows the programmer to create a new file   
![](touch-img.png)
* _mkdir_: used to make a new directory  
![](mkdir-img.png)