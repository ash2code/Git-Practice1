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

remove files from staged:

let's say you have two files and you added those two files to staging area by using command git add <file names> , after executiung this command both files are in staging area.


