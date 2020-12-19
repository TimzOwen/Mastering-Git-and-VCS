
### Remote Collaboration with Github

Github-->Distributed. @Dev has a copy of the repository

### Creating a repo.

create a new repo after creating a github account

initialize it with read me.

choose if private or public

Clone into your editor to start working on the Repo

cd into the branch or Markdown and edit

stage the changes for the commit

Push  the changed------->git push

##### password request each time avoidance

    use SSH Key-pair
    
    or Credential Helper

    git config --global credential.helper cache

#### interaction cheatsheet

create a new account 

[create new user account](https://github.com/join)

[create new branch ](https://help.github.com/articles/create-a-repo/)

Remote hosting site

[Github](http://github.com/)

[BitBucket](http://github.com/)

[Gitlab](https://gitlab.com/)

| Read on Liks                                                                                                           |   	Command      |
| ----------------------------------------------------------------------------------------------------------------- | -------------------- |
| [Cloning a remote repo](https://git-scm.com/docs/git-clone)                | git clone            |
| [pushing changes to remote ](https://git-scm.com/docs/git-push)          |git push
| [Fetch newest update from a repo](https://git-scm.com/docs/git-pull)	                    |git pull    |

Generate one password

[using caching](https://help.github.com/en/articles/caching-your-github-password-in-git)

[using ssh](https://help.github.com/en/articles/generating-an-ssh-key)

### Using Remote Repository

check for git configuration

    git remote -v

        1. fetch-uses HTTP

        2. push -uses HTTPS / SSH

    git remote show origin -- > get more details about remote repo

    git branch -r ---->check for remote branches

Fetching new changes

    git fetch ----> get all changes made from a repo

    git log origin/master ----> check the changes made

    git merge ---> Combine code if there a re changes behind the master branch

Updating Local Repository

| Read on Links                                                                                                           |   	Command      |
| ----------------------------------------------------------------------------------------------------------------- | -------------------- |
| [List Remote repos](https://git-scm.com/docs/git-remote)                | git remote            |
| [List remote repos verbosely ](https://git-scm.com/docs/git-remote#Documentation/git-remote.txt--v)          |git remote -v
| [describe single remote](https://git-scm.com/docs/git-remote#Documentation/git-remote.txt-emshowem)	                    |git remote show <name>   |
| [Get most up-to date commits ](https://git-scm.com/docs/git-remote#Documentation/git-remote.txt-emupdateem)          |git remote update
| [Download specific objects-](https://git-scm.com/docs/git-fetch)	                    |git fetch    |
