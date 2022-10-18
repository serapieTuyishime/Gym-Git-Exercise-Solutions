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
PS C:\Users\TheGym\Desktop\Git exercises> touch draft.txt
touch : The term 'touch' is not recognized as the name of a cmdlet, function, script file,    
or operable program. Check the spelling of the name, or if a path was included, verify that   
the path is correct and try again.
At line:1 char:1
+ touch draft.txt
+ ~~~~~
    + CategoryInfo          : ObjectNotFound: (touch:String) [], CommandNotFoundException     
    + FullyQualifiedErrorId : CommandNotFoundException
 
PS C:\Users\TheGym\Desktop\Git exercises> echo "This is text filecreated in command line" > draft.txt
PS C:\Users\TheGym\Desktop\Git exercises> echo "this file will be deleted!" > to delete.txt   
At line:1 char:1
+ del to delete.txt
+ ~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidArgument: (:) [Remove-Item], ParameterBindingException   
    + FullyQualifiedErrorId : PositionalParameterNotFound,Microsoft.PowerShell.Commands.Remo  
   veItemCommand
 
PS C:\Users\TheGym\Desktop\Git exercises> del C:\Users\TheGym\Desktop\Git exercises\to delete.txt
Remove-Item : A positional parameter cannot be found that accepts argument 'exercises\to'.    
+ del C:\Users\TheGym\Desktop\Git exercises\to delete.txt
+ ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidArgument: (:) [Remove-Item], ParameterBindingException   
    + FullyQualifiedErrorId : PositionalParameterNotFound,Microsoft.PowerShell.Commands.Remo  
   veItemCommand
 
PS C:\Users\TheGym\Desktop\Git exercises> del "to delete.txt"
del : Cannot find path 'C:\Users\TheGym\Desktop\Git exercises\to delete.txt' because it does  
not exist.
+ del "to delete.txt"
+ ~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (C:\Users\TheGym...s\to delete.txt:String) [Re  
   move-Item], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Commands.RemoveItemCommand    
 
PS C:\Users\TheGym\Desktop\Git exercises> echo "this file will be deleted!" > "to delete.txt" 
PS C:\Users\TheGym\Desktop\Git exercises> del "to delete.txt"
PS C:\Users\TheGym\Desktop\Git exercises> dir



Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/18/2022   5:04 PM             88 draft.txt


PS C:\Users\TheGym\Desktop\Git exercises> ren "draft.txt" ??? "draft Renamed.txt"
Rename-Item : A positional parameter cannot be found that accepts argument 'draft 
Renamed.txt'.
+ ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidArgument: (:) [Rename-Item], ParameterBindingException   
    + FullyQualifiedErrorId : PositionalParameterNotFound,Microsoft.PowerShell.Commands.Rena  
   meItemCommand
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
PS C:\Users\TheGym\Desktop\Git exercises> git add remote origin https://github.com/serapieTuyishime/Git-exercise-1.git
fatal: pathspec 'remote' did not match any files
PS C:\Users\TheGym\Desktop\Git exercises> git add origin https://github.com/serapieTuyishime/Git-exercise-1.git
fatal: pathspec 'origin' did not match any files
PS C:\Users\TheGym\Desktop\Git exercises> git remote add origin https://github.com/serapieTuyishime/Git-exercise-1.git
PS C:\Users\TheGym\Desktop\Git exercises> git push 
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\TheGym\Desktop\Git exercises> git push --u origin main
error: unknown option `u'
usage: git push [<options>] [<repository> [<refspec>...]]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --repo <repository>   repository
    --mirror              mirror all refs
    -d, --delete          delete refs
    --tags                push tags (can't be used with --all or --mirror)
    -n, --dry-run         dry run
    --porcelain           machine-readable output
    -f, --force           force updates
    --force-with-lease[=<refname>:<expect>]
                          require old value of ref to be at this value
    --recurse-submodules (check|on-demand|no)
                          control recursive pushing of submodules
    --thin                use thin pack
    --receive-pack <receive-pack>
                          receive pack program
    --exec <receive-pack>
                          receive pack program
    -u, --set-upstream    set upstream for git pull/status
    --progress            force progress reporting
    --prune               prune locally removed refs
    --no-verify           bypass pre-push hook
    --follow-tags         push missing but relevant tags
    --signed[=(yes|no|if-asked)]
                          GPG sign the push
    --atomic              request atomic transaction on remote side
    -o, --push-option <server-specific>
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only

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
PS C:\Users\TheGym\Desktop\Git exercises> git pull ...
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream  origin main
To https://github.com/serapieTuyishime/Git-exercise-1.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/serapieTuyishime/Git-exercise-1.git'   
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.








On branch main
nothing to commit, working tree clean
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
