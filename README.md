# learning-git

<svg class="octicon octicon-mark-github v-align-middle" height="32" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>

This repo was used to learn git from amigoscode.
https://amigoscode.com/

git --version
git --help
git config --global user.name "xxxx"
git config --global user.email "xxx_xxx@xxx.com"
git config --global color.ui auto
git config -l
cd ~/Desktop/
ls
mkdir learning-git
cd learning-git/
-----init--------
git init .
ls -a
rm -rf .git
git add
git init .
git add
-----git add ------
touch index.html
touch index.js
touch main.css
ls
git status
git add index.html
git rm --cached index.html
git status
git add index.html
git add index.js
git status
git add .
git status
git rm -r --cached .
git status
mkdir test
cd test
touch test.js
git status
ls
git add .
git status
git add -A
git status
----- commits ------
cd ..
git commit -m "bootstrap project"
git status
git log
git show 1bdfc0fa7837e41d9793e0eb333209a818c40c3b
q
vi index.js
i
console.log("hello");
esc : wq
cat index.js
git status
git diff
git add .
git status
git commit -m "added console.log"
git log
git show 0a5cb1fe65bc15969f9294ee09859977b5ef5974
vi index.js
i -> delete conosle.log
esc :wq
git diff
git status
git restore index.js
--------- Amend commits -----------------
ls
vi main.css
i -> body{}
esc :wq 
git status
git add .
git commit -m "jfisdrwert"
git log
git commit --amend -m "added body{} in main.css"
--------- git hub push -----------------
create reoisitory on gihub.com
git remote add origin https://github.com/xxxx/learning-git.git
git branch
git branch -M main

-------- SSH Keys Setup ------------

ssh-keygen -t ed25519-sk -C "xxx_xx@yaxxo.com"

vi main.go
git status
git commit -m "added main.go with empty main function"
git log
git push 
--------- git pull --------------------
add readme on github web
git log
ls
git pull
ls
change main.go in github web
cat main.go
git pull
cat main.go
-------- branches ----------
git branch
git branch -r
git branch -a
git branch feature-a
git branch -a
git checkout feature-a
git checkout -
vi utils.js
git status
git add .
git commit -m "utils.js with todo"
git log
git checkout -
git log
git checkout -
git push
git push -u origin feature-a
git checkout main
git checkout -b to-delete
git branch -a
git checkout -
git branch -d to-delete
------------- merging pr ------------
git log --oneline
git pull
git log --oneline
git branch -d feature-a
git branch -a
------- dealing with conflicts -------
git checkout -b feature-xyz
ls
cat index.html
add some html
git add .
git commit -m "add some html"
git push
git push --set-upstream origin feature-xyz
git add .
git commit -m "added another p tag"
------- merging conflicts --------------
git pull
git status
git add .
git status
git commit -m "resolved conflicts"
git status
git push
----------- rebase ---------------------
gi pull -r origin main
git add .
git rebase --continue
git push -f
---------- git pod ----------------
