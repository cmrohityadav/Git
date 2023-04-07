# Basics commands
 git --version

 git config

 git config --get user.name

 git config --global user.name 

 git config --global user.name "cmrohityadav"

 git config --global user.email

 git config --global user.email "cmrohityadav23@gmail.com"

git config --global core.editor "code --wait"

git init

ls

ls -a

cd .git

cd ..

git add index.html

git add . //for all files to tract ......//files gai stage area me

git commit -m "my first commit"

git status

.gitignore

git branch

git branch rahul

git checkout rahul

git  checkout -b yadav

git checkout master

git merge rahul




cmroh@Rohit MINGW64 /d/Web Development/Git
$ mkdir gitInitCommit

cmroh@Rohit MINGW64 /d/Web Development/Git
$ cd gitInitCommit

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit
$ code .

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit
$ ls
index.html

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ ls -a
./  ../  .git/  index.html

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ cd .git

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit/.git (GIT_DIR!)
$ ls
FETCH_HEAD  HEAD  config  description  hooks/  info/  objects/  refs/

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit/.git (GIT_DIR!)
$ cd ..

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ ls
index.html

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ ls
index.html

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git add index.html

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ ^C

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html


cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ ls
footer.html  index.html

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        footer.html


cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git add footer.html

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   footer.html
        new file:   index.html


cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ ^[[200~git commit -m "my first commit"
bash: $'\E[200~git': command not found

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git commit -m "my first commit"
[master (root-commit) d186fff] my first commit
 2 files changed, 24 insertions(+)
 create mode 100644 footer.html
 create mode 100644 index.html

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git status
On branch master
nothing to commit, working tree clean

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git add index.html

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   index.html


cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git commit -m "added home page as header"
[master eff85e9] added home page as header
 1 file changed, 1 insertion(+), 1 deletion(-)

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git status
On branch master
nothing to commit, working tree clean

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   footer.html
        modified:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

no changes added to commit (use "git add" and/or "git commit -a")

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git add .

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ ls
footer.html  index.html  passwords.js

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        modified:   footer.html
        modified:   index.html


cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git branch
* master

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git branch rahul

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git branch
* master
  rahul

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git checkout rahul
Switched to branch 'rahul'
A       .gitignore
M       footer.html
M       index.html

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (rahul)
$ git branch
  master
* rahul

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (rahul)
$ git checkout -b yadav
Switched to a new branch 'yadav'

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (yadav)
$ git branch
  master
  rahul
* yadav

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (yadav)
$ git checkout master
Switched to branch 'master'
A       .gitignore
M       footer.html
M       index.html

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git branch
* master
  rahul
  yadav

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        modified:   footer.html
        modified:   index.html


cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git add .

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git commit - m "add new files"
error: pathspec '-' did not match any file(s) known to git
error: pathspec 'm' did not match any file(s) known to git
error: pathspec 'add new files' did not match any file(s) known to git

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git commit -m "added"
[master 0d385b1] added
 3 files changed, 3 insertions(+)
 create mode 100644 .gitignore

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git status
On branch master
nothing to commit, working tree clean

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git branch
* master
  rahul
  yadav

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git checkout rahul
Switched to branch 'rahul'

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (rahul)
$ git add .

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (rahul)
$ git commit -m "navbar by rahul"
[rahul fc92dbb] navbar by rahul
 2 files changed, 15 insertions(+)
 create mode 100644 navbar.html
 create mode 100644 passwords.js

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (rahul)
$ git status
On branch rahul
nothing to commit, working tree clean

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (rahul)
$ git checkout master
Switched to branch 'master'

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git branch
* master
  rahul
  yadav

cmroh@Rohit MINGW64 /d/Web Development/Git/gitInitCommit (master)
$ git merge rahul
Merge made by the 'ort' strategy.
 navbar.html  | 13 +++++++++++++
 passwords.js |  2 ++
 2 files changed, 15 insertions(+)
 create mode 100644 navbar.html
 create mode 100644 passwords.js





