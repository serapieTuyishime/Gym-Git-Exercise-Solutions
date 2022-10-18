# Gym-Git-Exercise-Solutions

## bundle one
### exercise 1
```bash
Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.
Try the new cross-platform PowerShell https://aka.ms/pscore6

PS C:\Users\TheGym\Desktop\Git exercises> git init
Initialized empty Git repository in C:/Users/TheGym/Desktop/Git exercises/.git/
PS C:\Users\TheGym\Desktop\Git exercises>
PS C:\Users\TheGym\Desktop\Git exercises> git branch -M main
PS C:\Users\TheGym\Desktop\Git exercises> echo "This is text filecreated in command line" > draft.txt
PS C:\Users\TheGym\Desktop\Git exercises> echo "this file will be deleted!" > "to delete.txt" 
PS C:\Users\TheGym\Desktop\Git exercises> del "to delete.txt"
PS C:\Users\TheGym\Desktop\Git exercises> dir



Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/18/2022   5:04 PM             88 draft.txt

PS C:\Users\TheGym\Desktop\Git exercises> dir

    Directory: C:\Users\TheGym\Desktop\Git exercises

----                 -------------         ------ ----
-a----        10/18/2022   5:04 PM             88 draft.txt


PS C:\Users\TheGym\Desktop\Git exercises> ren "draft.txt" "draft Renamed.txt"    
PS C:\Users\TheGym\Desktop\Git exercises> dir




Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/18/2022   5:04 PM             88 draft Renamed.txt


PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "main: manuputated files"
[main (root-commit) f533d24] main: manuputated files
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 draft Renamed.txt
PS C:\Users\TheGym\Desktop\Git exercises> git remote add origin https://github.com/serapieTuyishime/Git-exercise-1.git
PS C:\Users\TheGym\Desktop\Git exercises> git push 
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream  origin main
To https://github.com/serapieTuyishime/Git-exercise-1.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/serapieTuyishime/Git-exercise-1.git'   
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\TheGym\Desktop\Git exercises> git pull
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 604 bytes | 23.00 KiB/s, done.
From https://github.com/serapieTuyishime/Git-exercise-1
 * [new branch]      main       -> origin/main
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
error: failed to push some refs to 'https://github.com/serapieTuyishime/Git-exercise-1.git'   
hint: Updates were rejected because the tip of your current branch is behind
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "main: connected remote and local"    
On branch main
nothing to commit, working tree clean
PS C:\Users\TheGym\Desktop\Git exercises> git remote add origin 
usage: git remote add [<options>] <name> <url>

    --tags                import all tags and associated objects when fetching
    -t, --track <branch>  branch(es) to track
                          master branch
                          set up remote as a mirror to push to or fetch from
PS C:\Users\TheGym\Desktop\Git exercises> git remote add origin https://github.com/serapieTuyierror: remote origin already exists.
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin main
To https://github.com/serapieTuyishime/Git-exercise-1.git
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

PS C:\Users\TheGym\Desktop\Git exercises> git push --force --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 293 bytes | 146.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/serapieTuyishime/Git-exercise-1.git
 + 13004b3...f533d24 main -> main (forced update)
branch 'main' set up to track 'origin/main'.

PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b dev
Switched to a new branch 'dev'
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b test
Switched to a new branch 'test'
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b  dev
fatal: a branch named 'dev' already exists
PS C:\Users\TheGym\Desktop\Git exercises> git switch dev
Switched to branch 'dev'
PS C:\Users\TheGym\Desktop\Git exercises> git branch --delete test 
Deleted branch test (was f533d24).
PS C:\Users\TheGym\Desktop\Git exercises> git branch -a
* dev
  main
  remotes/origin/main
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "exercise one done bundle1 done"      
On branch dev
nothing to commit, working tree clean
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin main
Everything up-to-date
branch 'main' set up to track 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> 
```
