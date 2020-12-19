
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
    
    
    
 ### Pull-Merge-Push Conflicts and Workflow

check for all the branches

    git log --graph --oneline --all

Three-way-merge

    git log -p  origin/master

Pushing Remote branches

    git push -u origin <branch>

    git checkout -b <branch name>

    git add repoName -a -m "commit message"

Rebasing your changes

Rebasing is combining sequences of commits

check all graph changes.

    git git rebase master

    After merge and rebase delete the branch for testing

[About merge Conflicts](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-merge-conflicts)

[PRs using Command-line](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/resolving-a-merge-conflict-using-the-command-line)

[Rebasing Github ](https://git-scm.com/book/en/v2/Git-Branching-Rebasing)




### Pull Requests

Forking:

    creating a copy of a given repository so that it belongs to our user

Pull Request:

    commit/series of commits that you send to the owner of the repository so that they incorporate into their tree

Steps:

    Fork the project

    find the error to fix

    propose File changes

    create a pull request

add a file

    git push -u origin add-readme


Squashing Changes in Commits.

    Rebase -i:
    git rebase -i master
        a repo with more changes details
    git push -f:
        Force Git to push current snapshot

[Learn more about pull Request](https://help.github.com/en/articles/about-pull-request-merges)

### Code Reviews

Code Review:

    Going through one's code to make sure it all makes sense.

[Style Guide Github](http://google.github.io/styleguide/)

[Pull Request Review](https://help.github.com/en/articles/about-pull-request-reviews)

[Code Review Process](https://medium.com/osedea/the-perfect-code-review-process-845e6ba5c31)

[What is Code Review](https://smartbear.com/learn/code-review/what-is-code-review/)

### Managing Collaboration & Integration

Continuos Integration (CI):

    Testing and running Code automatically using CI

Continuos Deployment/Delivery (CD):

    New Code deployed online/ to Production

CI/CD: example use case is JenKins

    :   Travis for Integration

Pipelines:

    steps you need to run to get to your end Result

artifacts:

    Files generated as part of the pipeline


#### Final tools readOns

[Dit Arp242](https://arp242.net/diy.html)

[Closing Issues](https://help.github.com/en/articles/closing-issues-using-keywords)

[Repo Contribution](https://help.github.com/en/articles/setting-guidelines-for-repository-contributors)

[CI/CD integrations](https://www.infoworld.com/article/3271126/what-is-cicd-continuous-integration-and-continuous-delivery-explained.html)

[Get started CI/CD](https://stackify.com/what-is-cicd-whats-important-and-how-to-get-it-right/)

[Get started Travis](https://docs.travis-ci.com/user/tutorial/)

[Travis Building stages](https://docs.travis-ci.com/user/build-stages/)
