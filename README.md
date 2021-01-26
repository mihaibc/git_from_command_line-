# Git from command line

## Bellow you can find list with useful commands and solutions for common problems that developers encounter working with git from the command line

- **Remove untraced files that are not added to the staging area**.
  
        git clean -fdx

- **Pull commits and rebase your changes on top**
  
         git pull --rebase --autostash

- **List all the commands that were executed**

        git reflog

- **Reset unpushed commits**

        git reset HEAD~1 --soft   // keep changes
        git reset HEAD~1 --hard   // don't keep changes
   *commit hash can be used instead of HEAD~1 if we want to reset to a specific commit*

- **Make some changes to an unpushed commit**

        git commit --amend  // add staged files to the last commit
        git commit --amend -m "New message" // change the last commit message