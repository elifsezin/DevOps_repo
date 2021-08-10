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

###Basic Git Commands:

| Command | Effect |
| ------ | ------ |
|git init| it helps us to install git in our project. now our project becomes a git repository in our local.|
|git add| We add the files we want git to follow by specifying them with the git add command. 'git add .' we can add our files other than the files specified in .gitignore.|
|git commit| we commit the changes of the project to our local repo.|
|git pull| we pull changes from remote server to our local.|
|git push| we push our local changes to the remote server.|
|git fetch| pull branch information from remote server.|
|git status| allows us to see the changes we have made in our project, adding-removing-editing.|
|git merge| allow us to apply changes in one branch to another. |

***[click]*** for more commands

[click]: <https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet>

### Git For DevOps

- Kubernetes configuration files, bash and phyton scripts and files like that should be tracked, stored and be shareable for the DevOps team.

- DevOps engineers as a team works and manages the same infrastructure together and they may need some kind of collaboration on those configuration files. This is the main reason why git repository is used for that.

- Secondly, for a DevOps engineer using CI/CD pipeline, git repository is necessary to integrate build automation tool.

## _Build Tools and Package Managers_
- Build tools are used to build the artifact and they are specific to the programming language. To examplify, for [Java], [Maven] and [Gradle] are used as a build tool. Then when you install dependencies, you can compile and compress the code. 

[Java]: <https://www.java.com/tr/>
[Maven]:<https://maven.apache.org>
[Gradle]: <https://gradle.org>

>### Dependencies
> Other applications that we use in our project are collected under the title of dependecy.
> 
> Our project needs these applications in order to work properly and fully, that is, it is dependent on these projects.
> 
> We specify the author of the application we use in dependency, the name of the application and the version we use
so maven/gradle can understand exactly which app to pull.

for Java;
```java
java -jar <name of the file>
``` 
runs the application

- On the other hand [Java Script] has no special artifact type (zip/tar files are the type of js and they does not include dependencies) and to build package managers like [npm] and yard are used. This package managers both use the same dependency file (package.json).

- Java Script is more flexible and not standardized thet is why a lot of people choose it to use in their projects.


[Java Script]: <https://www.javascript.com>
[npm]: <https://www.npmjs.com>

###Some Build Tools & Package Managers for different Programming Languages

|Programming Languag  | Build Tool / Package Manager |
| ------ | ------ |
|java|maven/gradle|
|java script|npm/yarn/webpack|
|phyton|pip|
|C/C++|conan|
|C#|NuGet|


### Build Tools and Docker

- Thanks to Docker there is no need to build different artifact types and repository for each file type. Also dependencies are not necessary on Docker,too.
- Docker uses Docker Images which is an alternative for all artifact types and it makes most of the process easier but you still need to build the Apps.

### Build Tools and DevOps
- the process as an Devops engineer is
> build docker image => push to repo => run on server

so you need the configure the buil automation tool.
