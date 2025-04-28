List of commands that I used

stray@Serch24 MINGW64 ~/bootcamp
$ git clone https://github.com/Serch24-Hub/getting-git-1.git
Cloning into 'getting-git-1'...
remote: Enumerating objects: 11, done.
remote: Counting objects: 100% (11/11), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 11 (delta 1), reused 9 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (11/11), done.
Resolving deltas: 100% (1/1), done.

stray@Serch24 MINGW64 ~/bootcamp
$ ls
getting-git-1/  git-flow-ttpr-001/  html-album-cover-ttpr-002/

stray@Serch24 MINGW64 ~/bootcamp
$ cd getting-git-1

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1 (main)     
$ ls
day1.txt  lesson1.txt  README.md

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1 (main)     
$ code .

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1 (main)     
$ mkdir first-git-lab

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1 (main)     
$ ls
day1.txt  first-git-lab/  lesson1.txt  README.md

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1 (main)     
$ cd first-git-lab

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (main)
$ git init
Initialized empty Git repository in C:/Users/stray/bootcamp/getting-git-1/first-git-lab/.git/

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ echo "Hello Git!" > hello.txt

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        hello.txt

nothing added to commit but untracked files present (use "git add" to track)

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git add hello.txt
warning: in the working copy of 'hello.txt', LF will be replaced by CRLF the next time Git touches it

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git status
On branch master

No commits yet
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   hello.txt


stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git commit -m "First commit, hello there"
[master (root-commit) 991d1d4] First commit, hello there  
 1 file changed, 1 insertion(+)
 create mode 100644 hello.txt

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git log
commit 991d1d496e2c72a26ccff61ed698d690e1018394 (HEAD -> master)
Author: Serch24-Hub <sergio_lozano2002@hotmail.com>       
Date:   Mon Apr 28 09:04:17 2025 -0400

    First commit, hello there

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ tree .git
bash: tree: command not found

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ dir /s .git
dir: cannot access '/s': No such file or directory
.git:
COMMIT_EDITMSG  description  hooks  info  objects
config          HEAD         index  logs  refs

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ echo "I have never used git before, but I am still getting it.\nGithub is a really good platform to work in teams.\nI will get more into it, because I want to learn more of
 it and how to use it" > REFLECTION.md

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ ls
hello.txt  REFLECTION.md

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        REFLECTION.md

nothing added to commit but untracked files present (use "git add" to track)

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git add REFELCTION.md
fatal: pathspec 'REFELCTION.md' did not match any files

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git add REFLECTION.md
warning: in the working copy of 'REFLECTION.md', LF will be replaced by CRLF the next time Git touches it

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)       
        new file:   REFLECTION.md


stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git commit -m "Reflection for Assignment #1"
[master 91a205a] Reflection for Assignment #1
 1 file changed, 1 insertion(+)
 create mode 100644 REFLECTION.md

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git push
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>


stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git log
commit 91a205acb94f3f8dd2f35213208ecf2533ad6e88 (HEAD -> master)
Author: Serch24-Hub <sergio_lozano2002@hotmail.com>       
Date:   Mon Apr 28 09:27:32 2025 -0400

    Reflection for Assignment #1

commit 991d1d496e2c72a26ccff61ed698d690e1018394
Author: Serch24-Hub <sergio_lozano2002@hotmail.com>       
Date:   Mon Apr 28 09:04:17 2025 -0400

    First commit, hello there

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git remote add origin https://github.com/Serch24-Hub/getting-git.git

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (master)
$ git branch -M main

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (main)
$ git push u- origin main
error: src refspec origin does not match any
error: failed to push some refs to 'u-'

stray@Serch24 MINGW64 ~/bootcamp/getting-git-1/first-git-lab (main)
$ git push -u origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 16 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 643 bytes | 321.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Serch24-Hub/getting-git.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
