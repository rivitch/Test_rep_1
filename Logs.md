PS D:\GB\TASKS\Hello_Git> cd Test_rep_1
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git remote add origin https://github.com/rivitch/Test_Rep2.git
error: remote origin already exists.
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git remote remove origin
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git remote add origin https://github.com/rivitch/Test_Rep2.git
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git remote -v
origin  https://github.com/rivitch/Test_Rep2.git (fetch)
origin  https://github.com/rivitch/Test_Rep2.git (push)
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git branch
* main
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git push -u origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (6/6), 1.21 KiB | 1.21 MiB/s, done.
Total 6 (delta 0), reused 6 (delta 0), pack-reused 0
To https://github.com/rivitch/Test_Rep2.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git remote add source https://github.com/rivitch/Test_rep_1.git
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git remote -v
origin  https://github.com/rivitch/Test_Rep2.git (fetch)
origin  https://github.com/rivitch/Test_Rep2.git (push)
source  https://github.com/rivitch/Test_rep_1.git (fetch)
source  https://github.com/rivitch/Test_rep_1.git (push)
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git add README.md
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git commit -m "Add Line"
 1 file changed, 1 insertion(+)
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/rivitch/Test_Rep2.git
   d2f1c13..4bde925  main -> main
branch 'main' set up to track 'origin/main'.
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git push -u sourse main 
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git remote -v
origin  https://github.com/rivitch/Test_Rep2.git (fetch)
origin  https://github.com/rivitch/Test_Rep2.git (push)
source  https://github.com/rivitch/Test_rep_1.git (fetch)
source  https://github.com/rivitch/Test_rep_1.git (push)
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git push -u sourse main
fatal: 'sourse' does not appear to be a git repository
fatal: Could not read from remote repository.
and the repository exists.
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git log
commit 4bde925a439ea5fbb0a2624153326d9fc5580ea6 (HEAD -> main, origin/main)
Author: rivitch <rivitch@rambler.ru>
    Add Line

Author: rivitch <136101600+rivitch@users.noreply.github.com>
Date:   Tue Dec 19 07:45:04 2023 +0400

    Update README.md

Author: rivitch <136101600+rivitch@users.noreply.github.com>
Date:   Tue Dec 19 07:40:11 2023 +0400

    Initial commit
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git add .
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git commit -m "1"
On branch main
Your branch is up to date with 'origin/main'.
nothing to commit, working tree clean
PS D:\GB\TASKS\Hello_Git\Test_rep_1>
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git push -u origin main
Everything up-to-date
branch 'main' set up to track 'origin/main'.
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git push -u sourse main
fatal: 'sourse' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git push -u source main
To https://github.com/rivitch/Test_rep_1.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/rivitch/Test_rep_1.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS D:\GB\TASKS\Hello_Git\Test_rep_1> git push -u source https://github.com/rivitch/Test_rep_1.git
fatal: invalid refspec 'https://github.com/rivitch/Test_rep_1.git'
PS D:\GB\TASKS\Hello_Git\Test_rep_1>
