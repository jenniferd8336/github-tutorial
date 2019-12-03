# GitHub Tutorial

_by Jennifer Delgado_

---
## Git vs. GitHub
Git: A version control system that allows users to keep track of changes done to their code. By using git the user is able to keep track the history of theiur code, as well as rerieve any previous deleted code.

Github: A website that allows users to store code in an github internet account. Github allows users to visually keep track of changes done to their code, as well as effectively collaborating with other github users. In order to efffectively use the tools github offers, users need to have some background knowledge in git.

---
## Initial Setup
Before a user starts using their IDE, they must set up by linking it to github. Go to the following link, to go through the procedure. m
https://github.com/hstatsep/ide50


---
## Repository Setup

When using your IDE, you will have to use two types of folders
A Directory: a normal folder
A Repository: a project folder in which git had been initialize in order to keep track of teh chnages of the project. 

In order to create a repository you must:
1. Create a directory with the command:
    mkdir "repository-name"
2. enter to the newly made directory with the command:
    cd "repository-name"
3. Initialize git in the directory with the following command
    git init 
3. Now that git has been intialized, the folder must be a repository, and (master) must appear after the name of the repository.

---
## Workflow & Commands
make edit git status, commit and push 
In the ide: ( make an unordered list)
git status: an optional command that show you the files in the repository that have been changed in red, and the files that are ready to be commited in green.
git add . : the command that prepares all the files in the repository to be commited to be committed.
git add "file-name" ; the command that prepares certain files to be commited.
git commit -m "commit message" : this command commits all of the files that were added. In other words snapshots of the desidered files are saved with this command.
git log : a command that shows you the list of commits

To push code to github:
git remote add origin URL : commit that links the local repository in the IDE with the external one in Github.
git push -u origin master : the shortened brnch of git push add origin master
git push : takes the commits from the locak repository, and passes a copy to the repository in github.
git remote rm origin : unlinks the local reposity and the repository on github.

---
## Rolling Back Changes
Every commit that is done within a repository has a SHA, which works as an Identification for every commit. They usually appear in yellow when git log is used. This SHA will become specially necessary when taking back a chnage that had been comitted.

git revert SHA: undoes the changes that were marked by the specific commit called.

