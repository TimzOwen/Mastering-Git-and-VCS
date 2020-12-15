


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




##### Undoing changes

revert changes back to original stage:

    git checkout filename.py
    
revert  individual lines

    git checkout -p
    
unstage changes

    git reset
    
    steps:
    
    let's ammend some changes and unstage:
    
    ./pythonSctipts.py > output.txt
    
    git add *
    
    git status
    
    git reset HEAD output.txt
    
    git status
    
    git commit -m "ammend the changes made
    
specific changes

    git reset -p

#### Amending commits

involves committing messages on files or missing tasks staged andd pushed

git commit --amend   --->replaces the git history with new one


#### Git Rollbacks

Going back tto your previous  stable working version

    git revert head
    
    git -p 2 ---> check for the changes made in the last 2 heads

#### Identifying a commit

uses Hashing to identify

    generated using SHA1 algorithm
    
    git log -1 ---> latest commit

#### more read on

[git checkout](https://git-scm.com/docs/git-checkout)

[More on git reset](https://git-scm.com/docs/git-reset#_examples)

[Reset your Repo](https://jwiegley.github.io/git-from-the-bottom-up/3-Reset/4-doing-a-hard-reset.html)

[Amending your repo](https://git-scm.com/docs/git-commit#Documentation/git-commit.txt---amend)

[Revert your  Repo](https://git-scm.com/docs/git-revert)

[Rollback your repo](https://git-scm.com/book/en/v2/Git-Basics-Undoing-Things)

[SHA-1 Algorithm](https://en.wikipedia.org/wiki/SHA-1)

[Blog on collision](https://github.blog/2017-03-20-sha-1-collision-detection-on-github-com/)

### Branching and Merging

branch -->Pointer to a particular commit

check branch

    git branch
    
create a new branch

    git branch new_feature

switching branches

    git checkout new_feature_branch
    
    git branch ------>shows we are at new branch
    
    git checkout -b new_branch --->create and switch direct
    
Delete a branch

    git branch -d branch_to_be_deleted

### Merging

Combining branched data and History together

merge

    git merge
    
    git merge branch_to_be_merged
    
    git log -----------> to see the changes made
    
Algorithms used to merge

    fast-forward
    
    three-way merge
    
### Merge Conflicts

