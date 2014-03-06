# git-cheatsheet

## git & svn

### Clone svn repository

  git svn clone https://path/to/your/repository --stdlayout
  
`stdlayout` specifies, that `trunk`, `tags` and `branches` are being cloned. 

**Note that this operation takes some time (hours)**

### Get new branches from svn

    git svn fetch
  
### Get latest changes from svn

    git svn rebase
  
### Commit to svn

    git svn dcommit

## git

### Restore to a previous point

    git reflog
    git reset --hard <hash>
    
### Create patch

    git format-patch master --stdout > my-patch.patch
  
### Change commit message after commit

    git commit --amend -m "new message"

### Stash specific files

    git add <file>
    git stash

