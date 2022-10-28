# DemoRepoLiz
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git checkout -b feature/login
Switched to a new branch 'feature/login'
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git branch
* feature/login
  main
  myNewBranchLiz
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git add .
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git commit -m "Add 'not' into 'this is not a test'"
[feature/login f39163d] Add 'not' into 'this is not a test'
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git log -oneline
fatal: unrecognized argument: -oneline
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git log --oneline
f39163d (HEAD -> feature/login) Add 'not' into 'this is not a test'
bd2b4a3 (origin/main, origin/HEAD, myNewBranchLiz, main) Added word 'world' and commented 'this is a test'
fb03fb9 Add file2.js and file3.js and index.html
bf7de6a Add file1.js
32fcc4d Initial commit
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git log --oneline --all
f39163d (HEAD -> feature/login) Add 'not' into 'this is not a test'
bd2b4a3 (origin/main, origin/HEAD, myNewBranchLiz, main) Added word 'world' and commented 'this is a test'
fb03fb9 Add file2.js and file3.js and index.html
bf7de6a Add file1.js
32fcc4d Initial commit
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git log main..feature/login
commit f39163d676a823fff4cd463348cffdbfcdc24ec5 (feature/login)
Author: caliz83 <lizg1308@gmail.com>
Date:   Thu Oct 27 19:42:52 2022 -0700

    Add 'not' into 'this is not a test'
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git log --oneline
bd2b4a3 (HEAD -> main, origin/main, origin/HEAD, myNewBranchLiz) Added word 'world' and commented 'this is a test'
fb03fb9 Add file2.js and file3.js and index.html
bf7de6a Add file1.js
32fcc4d Initial commit
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git diff
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git diff feature/login
diff --git a/file1.js b/file1.js
index a635ee4..d55d456 100644
--- a/file1.js
+++ b/file1.js
@@ -1,3 +1,3 @@
 Hello
 world
-//this is not a test
\ No newline at end of file
+//this is a test
\ No newline at end of file
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git branch
  feature/login
* main
  myNewBranchLiz
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git merge feature/login
Updating bd2b4a3..f39163d
Fast-forward
 file1.js | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git branch --merged
  feature/login
* main
  myNewBranchLiz
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git branch --no-merged
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git checkout feature/login

Switched to branch 'feature/login'
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git branch -d feature/login
error: Cannot delete branch 'feature/login' checked out at 'C:/Users/lizg1/DemoRepoLiz/DemoRepoLiz'
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git branch -D feature.login
error: branch 'feature.login' not found.
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git branch -d feature/login
Deleted branch feature/login (was f39163d).
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 298 bytes | 298.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object. 
To https://github.com/caliz83/DemoRepoLiz.git
   bd2b4a3..f39163d  main -> main
PS C:\Users\lizg1\DemoRepoLiz\DemoRepoLiz> 