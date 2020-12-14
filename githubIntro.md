### Version Control System (VCS)

#### Git
[Git system Control Manager](https://git-scm.com/doc)

[mercurial](https://www.mercurial-scm.org/)

[Apache subversion](https://subversion.apache.org/)

[Wikipedia version Control ReadOn](https://en.wikipedia.org/wiki/Version_control)


### Installing Git on Windows

check for the version with

        git --version

[Download page](https://git-scm.com/downloads)

[installation Instructions](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

### Working with Git.
Configuration:
    we user the flag - to set to all repositories
    git config --global user.email "timzowen@gmail.com"
    git config --global user.name "Timz Owen"

### create using simple project
    mkdir gitChecks-------> creates a new file on your system
    cd into the project file
    git init----->creates a new repository
    ls -la --->checks if file exits, list all starting with .
    ls -l .git --->check the contents in the file

    #staging area (File maintained by Git containing all the files and changes to the next commit)
    git add filename.py------->keep track of all file changes (staging area)
    git status------> check the current working tree and pending changes made
    git commit----->committing the changes made (you can write a commit message)

=============================================================================================================Latest commit
### Tracking File changes

Modified

    Changes made but not committed to the staging area
stage

    changes are ready to be committed

commit

    changes made are pushed

##### Example.

make changes to the code and run git status.

    cd gitchecks
    
    ls -l
    
    git status  # before making changes
    
    git status #after making changes to your code(not staged)
    
    git add gitcheks.py --> adds the changes made
    
    git status ---->check again and note the difference(staged)
    
    git commit -m "commit message" --->commit with message
    
    git status--->check, you'll note that it indicates nothing to commit as changes been staged

### Git workflow

##### check configuration:

    git config -l
    
create a new file and follow the initial steps above.

Rem, if no commit message , the changes are untracked

    git add filecreated.py ----->track the file
    
    git commit -m "message here"---> Failure to add -m launches a default editor where you'll type your commit message

##### Make changes to the existing file created--->"filecreated.py"

    git status----->check status and you'll see untracked changes
    
    git add filecreated.py--------->stage the changes
    
    git status----------->turn green meaning changes have been staged
    
    git commit -m "message"------>store changed to git Directory

##### Writing useful commit messages

Always write short desc first then long in commit messages later

Display commit messages:

    git log

More READ ONs:

[Linux Kernel Documentaion](https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/tree/Documentation/process/submitting-patches.rst?id=HEAD)

[impassioned opinions](http://stopwritingramblingcommitmessages.com/)

[Developers story and opinion on Git](https://robots.thoughtbot.com/5-useful-tips-for-a-better-commit-message)

[setting your email in git](https://help.github.com/articles/setting-your-email-in-git/)

[make your git mail private](https://help.github.com/articles/keeping-your-email-address-private/)
