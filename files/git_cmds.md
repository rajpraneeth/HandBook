# Github

>>## General commands

    git init <project folder name>
        -> This command is for creating repository by <project folder name>
#
    git status
        -> This is for showing the status of git repository, about staging file,
         updated files deleted file and all file manipulations.
#
    git add <file name>
    　　-> This will add the file to the staging area Or it brings the changes into staging area.
    　　We can add file by one by one Or recursively. This is for one by one
#
    git add .
    　　-> This for recursively adding.
#
    git commit
    　　-> This is for saving the changes to git repository by doing comment to the changes.
#
    git commit -m “ text info “
    　　-> This is for doing comment in inline.
#
    git commit -am 
    　　-> This is for adding changes to staging and commenting in single command.
#
    git ls-files
    　　-> This is for tacking the git directory files.
#
    git log --oneline --graph --all
    　　-> This will show all the commit in one line formats with the respective branch’s.

>># Pull, Push and Clone commands

    git clone <URL>
    　　-> This will download the repository from remote repository.
#
    git pull origin master
    　　-> This is for maintaining the synchronization between local repository and remote repository.
#
    git push origin master   
    　　-> This is for update the changes to remote repository.

>>#    Discard the change

    git reset HEAD <filename> 
    　　-> This is for discarding changes form staging area and revert back to working directory.
#
    git checkout --<filename>
    　　-> This is for discarding the changes from working directory. 
#
    git checkout <branch name>
    　　-> This will help to switch one branch to another branch.

>>#    Difference and Compare

    git diff
    　　-> This will show the changes or difference between staging area and working directory.
#
    git diff  Head
    　　-> This will show the changes or difference between working directory and git repository/last commit.
#
    git diff -staged
    　　-> This will show the changes or difference between staging area and git repository/last commit.
#
    git diff master origin/master  
    　　-> This will show the changes or difference between local git repository and remote repository.
#
    git diff  <commit_id1> <commit_id2> 
    　　-> This will show the changes or difference between two commits.

>>#    Branch's
    　　
    git branch -a
    　　-> This will list all the branches created.
#
    git branch <branch_name>
    　　-> This will create new branch.
#
    git checkout <branch_name>
    　　-> This will help to switch between the branch.
#
    git checkout -b <branch_name>
    　　-> This will create the branch and switch the branch to branch_name 
#
    git diff -d <branch_name>
    　　-> This will delete the branch only after merging it with master.
#
    git diff -D <branch_name>
    　　-> This will delete the branch irrespective of merging it with master.
    
>>#    Merge

>##  This command is used if you are on master branch

    git merge <branch_name>
    　　-> This will fast foreword merge the branch changes on the master branch.
#
    git merge <branch_name> --no-ff
    　　-> This will Not fast foreword merge the branch changes on the master branch.

 we have a Scenario where we have merge conflicts, we have to resolve by logic or selecting the changes and after resolve conflicts merge with master branch.

>>#    Rebase

>## This commands is used if you are on branch

    git rebase master
    　　-> This will merge the changes in master on the branch.

> we have a Scenario where we have Rebase conflicts, we have to resolve by logic or selecting the changes and after resolve conflicts rebase with branch. 
#
    git rebase --abort
    　　-> This will abort the conflicts, so we can resolve it later.
    　　
>>#    *__Stash__*

>## This commands is used if you are on master branch

    git stash
    　　-> This will take all the file for stash.
#
    git stash apply
    　　-> This will take back all the file that we stashed.

>There is a scenario where we want to hide or working on that file, it is in stage area or working directory you need to commit some other changes. In this case we use stash.
This will hide the file which we are working on and un-hide them when we want, during this we cane commit other changes
　　
---
# *__Reference__*

>URL

* [Atlassian](https://www.atlassian.com/git/tutorials/what-is-version-control)

