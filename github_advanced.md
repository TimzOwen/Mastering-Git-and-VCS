


## Advanced Git and commands

#### using git locally:

Skipping the staging ares:

    git commit -a --->commits tracked files without git add
    
    git commit -a -m "add msg directly"
    
    committing changes into one commit instead of many files

Git HEAD:

    rep the currently checked-out snapshot of your project

##### more info about changes in git

use Patch

    git log -p
    
git show

    shows a summarized git work (changes made only with key passed)
    
git --stat

    shows number of files changes  and files changed (git log --stat)
    
git add changed without staging

    git add -p
    
show changes staged but not committed

    git diff --staged

##### modifying files in git

Remove files

    git rm filename.py
    
    git commit -m "remove message"
    
Rename Files in Git

    git mv file_name.py new_rename_name.py
    
    git commit -m "renamed the file"
    
Hide some files

    use .ignore
    
    First create the the .hidden -->.gitignore
    
    echo .File_Hidden > .gitignore
    
    ls -la --> List all files including the hidden files
    
    git commit -m "msg"

#### Reading notes
| Read on                                                                                                           |   	Command      |
| ----------------------------------------------------------------------------------------------------------------- | -------------------- | 
| [staging Files automatically](https://git-scm.com/docs/git-commit#Documentation/git-commit.txt---all)                | git commit -a              |        
| [Producing Patch text](https://git-scm.com/docs/git-log#_generating_patch_text_with_p)          |git log -p
| [Show various objects](https://git-scm.com/docs/git-show)	                    |git show     |        
| [show different commits](https://git-scm.com/docs/git-diff)                   | git diff    |
| [show all staged Files](https://git-scm.com/docs/git-diff)                      | git diff --staged
| [Review Git patch for staging](https://git-scm.com/docs/git-add)                | git add -p
| [Moving a file](https://git-scm.com/docs/git-mv)	                | git mv
| [Removing a File](https://git-scm.com/docs/git-rm)           | git rm


[More cheatsheet reference on git commands covered](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf)

[understanding Gitignore](https://git-scm.com/docs/gitignore)

[Common File patterns](https://gist.github.com/octocat/9257657)
