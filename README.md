# DevOps Progress

## _Version Control with Git_

- [Git] is a version control system, it helps us to systematically store and manage the code we write not only on our own device but also on a remote server.
- It allows us to monitor the status (editing, deleting, adding new files) of the files in our project (except the ones we add to .gitignore), and to develop our project safely without breaking our core code.
- Ideally committing in our project allows us to both see the changes in a healthier way by creating follow-up points and to go to any moment in our project in a possible case.

 _In the simplest terms, Git is a version control system that helps us develop our project systematically and securely._

- [GitHub], on the other hand, is a kind of project storage system where the git system is integrated, where we can see the projects of other developers in the world. We can see our projects that we have integrated git, and the actions we have done with git commands on GitHub.

_It is kind of a social network for developers._

[Git]: <https://git-scm.com>
[GitHub]: <https://github.com/elifsezin>

>###Basic Git Commands:
> 
> ***git init***: it helps us to install git in our project. now our project becomes a git repository in our local.
> 
> ***git add***: We add the files we want git to follow by specifying them with the git add command. 'git add .' we can add our files other than the files specified in .gitignore.
> 
> ***git commit***: we commit the changes of the project to our local repo
> 
> ***it pull***: we pull changes from remote server to our local. 
> 
> ***git push***: we push our local changes to the remote server.
> 
> ***git fetch***: pull branch information from remote server
> 
> ***git status***: allows us to see the changes we have made in our project, adding-removing-editing.
> 
> ***git checkout***: allows us to switch between different branches
> 
> ***git stash***: It allows Git to temporarily save the changes you have worked on but not yet committed, and restore your active branch to a clean state with no changes.
> 
>***[click]*** for more commands
> 
[click]: <https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet>

### Git For DevOps

- Kubernetes configuration files, bash and phyton scripts and files like that should be tracked, stored and be shareable for the DevOps team.

- DevOps engineers as a team works and manages the same infrastructure together and they may need some kind of collaboration on those configuration files. This is the main reason why git repository is used for that.

- Secondly, for a DevOps engineer using CI/CD pipeline, git repository is necessary to integrate build automation tool.
