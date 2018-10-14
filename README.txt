CRITICALLY IMPORTANT NOTES FROM ROBERT CUNNINGHAM

the issue was that you had the file in github instantiated with a readme file, however, at the same time you were creating a local file on your computer called tower of hanoi, that didn't have the readme file. Because the components of code in the local and on github didn't match up you could push the tower of hanoi to github because they didn't make. 

in summary: 
make sure the code in the local and github match up and praise the following code: 


other notes:

add origin is referring to adding the code from github and connecting it to the code on the computer 

there are three stages of files:
1. unaccounted for files - when you do status it gets put in red
2. staged files - when it's green and ready to be committed files
3. committed - when it's committed and is uploaded to github 


jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects (master)
$ cd C:/Users/jdavi/IdeaProjects/TowersOfHanoi/src

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git init
Initialized empty Git repository in C:/Users/jdavi/IdeaProjects/TowersOfHanoi/src/.git/

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git remote add origin https://github.com/jdlonergan08/github-upload.git

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git add .

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git push -u origin master
error: src refspec master does not match any.
error: failed to push some refs to 'https://github.com/jdlonergan08/github-upload.git'

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git commit -m "initializing repository"
[master (root-commit) 248c0aa] initializing repository
 2 files changed, 115 insertions(+)
 create mode 100644 .gitignore.gitignore
 create mode 100644 TowerOfHanoi.java

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git push -u origin master
To https://github.com/jdlonergan08/github-upload.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://github.com/jdlonergan08/github-upload.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git pull
warning: no common commits
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
From https://github.com/jdlonergan08/github-upload
 * [new branch]      master     -> origin/master
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> master


jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git push -u origin master
To https://github.com/jdlonergan08/github-upload.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'https://github.com/jdlonergan08/github-upload.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git pull
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> master


jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git pull
fatal: refusing to merge unrelated histories

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git init
Initialized empty Git repository in C:/Users/jdavi/IdeaProjects/TowersOfHanoi/src/.git/

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        .gitignore.gitignore
        TowerOfHanoi.java

nothing added to commit but untracked files present (use "git add" to track)

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git add TowerOfHanoi.java

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   TowerOfHanoi.java

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        .gitignore.gitignore


jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git commit -m "first commit"
[master (root-commit) 87d490f] first commit
 1 file changed, 92 insertions(+)
 create mode 100644 TowerOfHanoi.java

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git remote add origin https://github.com/jdlonergan08/upload-test2.git

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 1.00 KiB | 1.00 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
remote:
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/jdlonergan08/upload-test2/pull/new/master
remote:
To https://github.com/jdlonergan08/upload-test2.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

jdavi@LAPTOP-EK9OD4HA MINGW64 ~/IdeaProjects/TowersOfHanoi/src (master)
$

at the bottom here is a test to write code on github and pull it to git 
