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
### exercise 2

```bash

PS C:\Users\TheGym\Desktop\Git exercises> git init      
Reinitialized existing Git repository in C:/Users/TheGym/Desktop/Git exercises/.git/
PS C:\Users\TheGym\Desktop\Git exercises> git stash clear
PS C:\Users\TheGym\Desktop\Git exercises> echo "hdhhf" >"home.html" 

PS C:\Users\TheGym\Desktop\Git exercises> git add home.html
d24 main: manuputated files
PS C:\Users\TheGym\Desktop\Git exercises> echo "this is 
d24 main: manuputated files
PS C:\Users\TheGym\Desktop\Git exercises> git stash list
stash@{1}: WIP on dev: f533d24 main: manuputated files  
PS C:\Users\TheGym\Desktop\Git exercises> echo "this is 
the teams page" > "teams.html"
PS C:\Users\TheGym\Desktop\Git exercises> git stash     
Saved working directory and index state WIP on dev: f533d24 main: manuputated files
PS C:\Users\TheGym\Desktop\Git exercises> git stash list

stash@{0}: WIP on dev: f533d24 main: manuputated files  
stash@{1}: WIP on dev: f533d24 main: manuputated files  
stash@{2}: WIP on dev: f533d24 main: manuputated files  
PS C:\Users\TheGym\Desktop\Git exercises> git checkout  
stash@{1} about.html
error: unknown switch `e'
usage: git checkout [<options>] <branch>
   or: git checkout [<options>] [<branch>] -- <file>... 

    -b <branch>           create and checkout a new branch
    -B <branch>           create/reset and checkout a branch
    -l                    create reflog for new branch  
    --guess               second guess 'git checkout <no-such-branch>' (default)
    --overlay             use overlay mode (default)    
    -q, --quiet           suppress progress reporting   
    --recurse-submodules[=<checkout>]
                          control recursive updating of 
submodules
    --progress            force progress reporting      
    -m, --merge           perform a 3-way merge with the new branch
    --conflict <style>    conflict style (merge, diff3, 
or zdiff3)
    -d, --detach          detach HEAD at named commit   
    -t, --track[=(direct|inherit)]
                          set branch tracking configuration
    -f, --force           force checkout (throw away local modifications)
    --orphan <new-branch>
                          new unparented branch
    --overwrite-ignore    update ignored files (default)    --ignore-other-worktrees
                          do not check if another worktree is holding the given ref
    -2, --ours            checkout our version for unmerged files
    -3, --theirs          checkout their version for unm    --ignore-skip-worktree-bits
                          do not limit pathspecs to sparse entries only
    --pathspec-file-nul   with --pathspec-from-file, pathspec elements are separated with NUL character

PS C:\Users\TheGym\Desktop\Git exercises> git stash list

stash@{0}: WIP on dev: f533d24 main: manuputated files  
stash@{1}: WIP on dev: f533d24 main: manuputated files  
stash@{2}: WIP on dev: f533d24 main: manuputated files  

PS C:\Users\TheGym\Desktop\Git exercises> git stash list

stash@{0}: WIP on dev: f533d24 main: manuputated files  
stash@{1}: WIP on dev: f533d24 main: manuputated files  
stash@{2}: WIP on dev: f533d24 main: manuputated files  
PS C:\Users\TheGym\Desktop\Git exercises> git stash pop 
PS C:\Users\TheGym\Desktop\Git exercises> git stash pop 
 stash@{0}    
error: unknown switch `e'
usage: git stash pop [--index] [-q|--quiet] [<stash>]   

    -q, --quiet           be quiet, only report errors  
    --index               attempt to recreate the index 
1
On branch dev
        new file:   about.html

Dropped refs/stash@{1} (bb7d051a451edb7afc8ce1ede56c34ca15382f26)
PS C:\Users\TheGym\Desktop\Git exercises> git stash list

stash@{0}: WIP on dev: f533d24 main: manuputated files  
stash@{1}: WIP on dev: f533d24 main: manuputated files  
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)     
        new file:   about.html
Dropped refs/stash@{1} (0a2f674cebe3e4bdf3e1bfe42885bd4a7557b62f)
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m 
"dev: did the stashing and unstashing"
[dev 0a3c229] dev: did the stashing and unstashing      
 2 files changed, 0 insertions(+), 0 deletions(-)       
 create mode 100644 about.html
 create mode 100644 home.html
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 921 bytes | 307.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0    
iting:
remote:
To https://github.com/serapieTuyishime/Git-exercise-1.gi * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.
PS C:\Users\TheGym\Desktop\Git exercises> git stash list

stash@{0}: WIP on dev: f533d24 main: manuputated files  
PS C:\Users\TheGym\Desktop\Git exercises> git stash pop 
o
error: o is not a valid reference
PS C:\Users\TheGym\Desktop\Git exercises> git stash pop 
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)     
        new file:   teams.html

Dropped refs/stash@{0} (aab78323e4346404e68533e4c48053804a9859cc)
PS C:\Users\TheGym\Desktop\Git exercises> git reset     
PS C:\Users\TheGym\Desktop\Git exercises> git reset 
```
## bundle 2
### exercise one
```bash
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
PS C:\Users\TheGym\Desktop\Git exercises> git add .     
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m 
"ft/bundle-2 created new services" 
[ft/bundle-2 461f146] ft/bundle-2 created new services  
 2 files changed, 13 insertions(+)
 create mode 100644 services.html
 create mode 100644 teams.html
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin ft/bundle-2
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 894 bytes | 894.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0    
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/serapieTuyishime/Git-exercise-1/pull/new/ft/bundle-2
remote:
To https://github.com/serapieTuyishime/Git-exercise-1.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
PS C:\Users\TheGym\Desktop\Git exercises>          
```
