=========== frontend-practice % git
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone             Clone a repository into a new directory
   init              Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add               Add file contents to the index
   mv                Move or rename a file, a directory, or a symlink
   restore           Restore working tree files
   rm                Remove files from the working tree and from the index
   sparse-checkout   Initialize and modify the sparse-checkout

examine the history and state (see also: git help revisions)
   bisect            Use binary search to find the commit that introduced a bug
   diff              Show changes between commits, commit and working tree, etc
   grep              Print lines matching a pattern
   log               Show commit logs
   show              Show various types of objects
   status            Show the working tree status

grow, mark and tweak your common history
   branch            List, create, or delete branches
   commit            Record changes to the repository
   merge             Join two or more development histories together
   rebase            Reapply commits on top of another base tip
   reset             Reset current HEAD to the specified state
   switch            Switch branches
   tag               Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch             Download objects and refs from another repository
   pull              Fetch from and integrate with another repository or a local branch
   push              Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.


=========== frontend-practice % git branch
* master


=========== frontend-practice % git branch corrections


=========== frontend-practice % git branch corrections
* master


=========== frontend-practice % git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   PoweredbyTech/Poweredbytech.css
        modified:   PoweredbyTech/Poweredbytech.html
        modified:   PoweredbyTech/Responsive.css
        deleted:    PoweredbyTech/magnifying-glass (1).png

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        PoweredbyTech/magnifying-glass.png

no changes added to commit (use "git add" and/or "git commit -a")


=========== frontend-practice % git add .


=========== frontend-practice % git commit -m "fixed tablet screen styles"
[master d4ab333] fixed tablet screen styles
 4 files changed, 94 insertions(+), 25 deletions(-)
 rename PoweredbyTech/{magnifying-glass (1).png => magnifying-glass.png} (100%)


=========== frontend-practice % git branch corrections
* master


=========== frontend-practice % git checkout corrections
Switched to branch 'corrections'


=========== frontend-practice % git branch
* corrections
  master


=========== frontend-practice % git status
On branch corrections
nothing to commit, working tree clean


=========== frontend-practice % git chechout master
git: 'chechout' is not a git command. See 'git --help'.

The most similar command is
        checkout


=========== frontend-practice % git checkout master
Switched to branch 'master'
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)


=========== frontend-practice % git reser --soft
 HEAD~1
git: 'reser' is not a git command. See 'git --help'.

The most similar commands are
        reset
        restore


=========== frontend-practice % git reset --soft HEAD~1


=========== frontend-practice % git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   PoweredbyTech/Poweredbytech.css
        modified:   PoweredbyTech/Poweredbytech.html
        modified:   PoweredbyTech/Responsive.css
        renamed:    PoweredbyTech/magnifying-glass (1).png -> PoweredbyTech/magnifying-glass.png



=========== frontend-practice % git restore --staged .


=========== frontend-practice % git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   PoweredbyTech/Poweredbytech.css
        modified:   PoweredbyTech/Poweredbytech.html
        modified:   PoweredbyTech/Responsive.css
        deleted:    PoweredbyTech/magnifying-glass (1).png

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        PoweredbyTech/magnifying-glass.png

no changes added to commit (use "git add" and/or "git commit -a")


=========== frontend-practice % git checkout corrections
M       PoweredbyTech/Poweredbytech.css
M       PoweredbyTech/Poweredbytech.html
M       PoweredbyTech/Responsive.css
D       PoweredbyTech/magnifying-glass (1).png
Switched to branch 'corrections'


=========== frontend-practice % git status
On branch corrections
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   PoweredbyTech/Poweredbytech.css
        modified:   PoweredbyTech/Poweredbytech.html
        modified:   PoweredbyTech/Responsive.css
        deleted:    PoweredbyTech/magnifying-glass (1).png

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        PoweredbyTech/magnifying-glass.png

no changes added to commit (use "git add" and/or "git commit -a")


=========== frontend-practice % git branch
* corrections
  master


=========== frontend-practice % git add .


=========== frontend-practice % git commit -m "fixed tablet screen styles"
[corrections cf0c053] fixed tablet screen styles
 4 files changed, 94 insertions(+), 25 deletions(-)
 rename PoweredbyTech/{magnifying-glass (1).png => magnifying-glass.png} (100%)


=========== frontend-practice % git status
On branch corrections
nothing to commit, working tree clean


=========== frontend-practice % git push
fatal: The current branch corrections has no upstream branch.
To push the current branch and set the remote as upstream, use "git push --set-upstream origin corrections"


=========== frontend-practice % git remote set-url origin corrections https://ghp_Pk2ExVivOn270jS19BceyGzcPWaGW33dV7Hf@github.com/devgemmy/frontend-practice.git
fatal: No such URL found: https://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@github.com/devgemmy/frontend-practice.git


=========== frontend-practice % git remote set-url origin https://ghp_Pk2ExVivOn270jS19BceyGzcPWaGW33dV7Hf@github.com/devgemmy/frontend-practice.git 


=========== frontend-practice % git push --set-upstream origin corrections
remote: Repository not found.
fatal: repository 'https://github.com/devgemmy/frontend-practice.git/' not found


=========== frontend-practice % git remote set-url origin https://ghp_Pk2ExVivOn270jS19BceyGzcPWaGW33dV7Hf@github.com/b3tcee/frontend-practice.git


=========== frontend-practice % git push --set-upstream origin corrections
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 2 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 1.11 KiB | 378.00 KiB/s, done.
Total 6 (delta 5), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (5/5), completed with 5 local objects.
remote: 
remote: Create a pull request for 'corrections' on GitHub by visiting:
remote:      https://github.com/b3tcee/frontend-practice/pull/new/corrections
remote: 
To https://github.com/b3tcee/frontend-practice.git
 * [new branch]      corrections -> corrections
Branch 'corrections' set up to track remote branch 'corrections' from 'origin'.


=========== frontend-practice % git status
On branch corrections
Your branch is up to date with 'origin/corrections'.

nothing to commit, working tree clean


=========== frontend-practice %   