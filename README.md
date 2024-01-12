# Git-Practice1
creating repo for git practice

this repo contains basic shell scripts and python scripts

**************UNDERSTANDING THE WORKSPACE AND STAGING AREA AND LOCAL REPOSITORY***************
1) Creating workspace
2) git initialization
3) Creating files with some content in the working directory
4) Adding these files to staging area
5) Git Configurations before first commit
6) Commit those changes to local repository.

1) CREATING WORKSPACE : **mkdir <folder>**
                                  **cd <folder>**
2) GIT INITIALIZATION: **git init**
3) CREATING FILES:  by using nano/touch/vim we can create files and insert content (nano/vim).
4) ADDING FILES TO THE STAGING AREA: git add . (it refers all files in that folder)
                                                      git add <file-name> (refers only given file name)
5) GIT CONFIGURATION: git config --global user.name "git userid"
                                                         git config --globaluser.email "git email"
6) COMMIT : commit the changhes with command git commit -m "need to give commit message here"
            
   
###########################################################################
* To check last modify by user for ecah line of a file use command = git blame file_name
* switch to a new branch in one step - git checkout or git swith -c branch_name

GIT STATUS:

gti status command will give the status of our git commands.

for example in your local repo you created a new file and checked th status git status , it will show us that the new file is untracked.
when you add the file by using git add command , it will show us changes are in staging area , and changes yet to be committed.

Remove files from staged:

let's say you have three files and you added those three files to staging area by using command git add <file names> , after executiung this command three files are in staging area.

Ramesh@soma MINGW64 ~/desktop/ash2code/git_practice1 (bug-fix)
$ git status
On branch bug-fix
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file1.txt
        new file:   helloworld.sh
        new file:   sample.py

now if we don't want to continue to move changes of sample.py , we need to remove sample.py file from staging area. we can do that by running the command git restore --staged <file name>
Ramesh@soma MINGW64 ~/desktop/ash2code/git_practice1 (bug-fix)
$ git restore --staged sample.py

now check the git status again.
Ramesh@soma MINGW64 ~/desktop/ash2code/git_practice1 (bug-fix)
$ git status
On branch bug-fix
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file1.txt
        new file:   helloworld.sh

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        sample.py



