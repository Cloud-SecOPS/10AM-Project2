git --version   : <-- this one used for to see version of the present using git  
git config --global user.name "username"   : for configure the user name 
git config --global user.email "mail id "  : for configure the local machine user's mail id /employee mail id 
git add . : <-- this one used for to add all files at a time  from working directory to staging. 
git status : <-- this one used for to see the status of working tree. 
git commit -m "any one message" : to send the from staging to commtting area.
git push origin main  : <-- to send the files form local commtting area to remote repository. 

pwd : <-- this one used for to see present working directory
ls   : <-- this one used for to list only files and directories 
ll : <-- this one used for to list in long list format 
cd ..  : <-- this one used for to come out from the child directory 

   example:
    mkdir /ravi
    pwd
    /ravi 
    note: / also a directory
    ravi is directory int the /
    cd .. 
    this cursor will come out from the ravi directory 




cd <path>  : <-- this one used for to enter into the child directory 
touch : <-- this is the command and it used for to create a file or files.

syntax: 1

  touch file-name 

example: 
  touch  java 

syntax: 2
touch file-name file-name file-name  .. nth file

example: 

   touch devops aws linux python 


note: we can't insert data/text/content inside the file while a file/files by using thouch command  



git add : 

  git add is a command and it used for to  the file /files from working directory to staging area 

syntax: 1
  git add file name    : <-- this one used for to add only one file at a time  
example:
  git add aws 

syntax: 2 : here w can add one or more files at a time . 

  example:
      git add devops azure python 


syntax: 3

git add .  : <-- this one used for to add all files at a time from working directory to staging

 example :
   git add . 

syntax: 4

   git add *   : <-- this one used for to add only normal files and directories 

syntax: 5

git add  --all  : <-- this one used for to add all files at a time from working directory to staging

syntax: 6

git add  -A  : <-- this one used for to add all files at a time from working directory to staging


git add <first character of the file/files >: this one used for to add the file files by the first charater from the files /files 


  touch java jsp javascript oracle  dbms dba mysql python python-fullstack 


example:
  git add j* d* 


git stage: this is also one command for adding the files from working directory to staging

syntax : 1
  git stage file-name

 example:

  git stage aws 


syntax : 2
  git stage file-name file-name


example:
  git stage devps azure linux 

syntax  & example : 3

git stage .   <-- this one used for to all files at a time 


syntax  & example : 4

git stage *    <-- here we can add only normal files and normal directories 


syntax  & example : 5

git stage --all  <-- this one used for to all files at a time  

syntax  & example : 6

git stage -A    <-- this one used for to all files at a time 

git stage <first character of the file/files >: this one used for to add the file files by the first charater from the files /files 


  touch java jsp javascript oracle  dbms dba mysql python python-fullstack 


example:
  git stage j* d* 



Commit:

  commit is a command and it used for  to commit the files from staging to commtting area.


syntax: 1

   git commit -m "any one message" file-name


example: 1

   git commit -m "version 1.0" file-permissions.sh 


syntax: 2 : <-- this one used for to commit more than one file 

   git commit -m "any one message" file-name file-name 


example: 1

   git commit -m "version 1.1" file-permissions.sh Dockerfile 


To commit all staged files:

syntax & example: 

git commit -m "message" : <-- this command used for to commit all files at a time


git show:

git show is a command and it used for to see the latest commited files along with commit id and data/content in the files 

for example:

Cloud Gen@DESKTOP-GS3L6T2 MINGW64 /h/My-Git-Projects/DevOps (main)
$ git show   :
commit 7445622723613402ceae00666510d1513d279d75 (HEAD -> main)
Author: ravindra <ravindra@cloudgen.in>
Date:   Fri Jan 6 10:56:15 2023 +0530

    test commit V1.0

diff --git a/sai b/sai
new file mode 100644
index 0000000..e69de29
diff --git a/shaym b/shaym
new file mode 100644
index 0000000..e69de29
diff --git a/shiava b/shiava
new file mode 100644
index 0000000..e69de29
diff --git a/sundar b/sundar
new file mode 100644
index 0000000..e69de29
diff --git a/sunil b/sunil
new file mode 100644
index 0000000..e69de29

Cloud Gen@DESKTOP-GS3L6T2 MINGW64 /h/My-Git-Projects/DevOps (main)
$



reset the file/files form committing: 

  git reset --soft HEAD~ : 
    above command used for reset/un-commit the latest files from committing to staging area 


example:

Cloud Gen@DESKTOP-GS3L6T2 MINGW64 /h/My-Git-Projects/DevOps (main)
$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 2 and 2 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .asp
        2PM Linux Class.sh
        aws
        azure
        cloud/
        devps
        git sylbus
        java
        linux
        python

nothing added to commit but untracked files present (use "git add" to track)

  Cloud Gen@DESKTOP-GS3L6T2 MINGW64 /h/My-Git-Projects/DevOps (main)
$ git reset --soft HEAD~   :

Cloud Gen@DESKTOP-GS3L6T2 MINGW64 /h/My-Git-Projects/DevOps (main)
$ git status   :
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 2 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   sai
        new file:   shaym
        new file:   shiava
        new file:   sundar
        new file:   sunil

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .asp
        2PM Linux Class.sh
        aws
        azure
        cloud/
        devps
        git sylbus
        java
        linux
        python


Cloud Gen@DESKTOP-GS3L6T2 MINGW64 /h/My-Git-Projects/DevOps (main)
$



git 4th class: 


  git reset @~ : this one used for to reset the files form commtting and staging to working directory

touch devops1 java1 python1 jsp1 javascript1 ruby1 
git add devops1 java1 python1 jsp1 javascript1 ruby1 
git commit -m "test commit" devops1 java1 python1 jsp1 javascript1 ruby1 

git status -s

on result: 
we we are seeing the ??  : - its mean that file located in working directory and in untracked location
Cloud Gen@DESKTOP-GS3L6T2 MINGW64 /h/My-Git-Projects/DevOps (main)
example: 

$ git status -s
?? .asp
?? "2PM Linux Class.sh"
?? aws
?? azure
?? cloud/
?? devops1
?? devps
?? "git sylbus"
?? java



we we are seeing the green Clolor  A before the file / files : its mean this file located in staging area and we need to understand its a newly added file  from working to staging

example:

Cloud Gen@DESKTOP-GS3L6T2 MINGW64 /h/My-Git-Projects/DevOps (main)
$ git add azure java python devops1


example: output : 

Cloud Gen@DESKTOP-GS3L6T2 MINGW64 /h/My-Git-Projects/DevOps (main)
$ git status -s
A  azure
A  devops1
A  java
A  python
?? .asp
?? "2PM Linux Class.sh"
?? aws
?? cloud/
?? devps
?? "git sylbus"
?? java1

Red Color M  :

when we are seeing the Red color M by applying the status -s  command  it's mean we need understand about this file like below

this file committed and its modified, due to modifying the file  we are seeing in red color and in working directory in modified location

example:

  Cloud Gen@DESKTOP-GS3L6T2 MINGW64 /h/My-Git-Projects/DevOps (main)
$ git status -s
 M "10 am git class"
A  azure
A  devops1
A  java
A  python
?? .asp
?? "2PM Linux Class.sh"
?? aws
?? cloud/
?? devps
?? "git sylbus"



Green Color M  :
  
when we are seeing the Green color 'M' by applying the status -s  command  it's mean we need understand about this file like below

this file committed and its modified

after modifying this filed added into staging area so that we are seeing the green color M 



example:

  Cloud Gen@DESKTOP-GS3L6T2 MINGW64 /h/My-Git-Projects/DevOps (main)
$ git status -s
 M "10 am git class"
A  azure
A  devops1
A  java
M  linux
A  python
?? .asp
?? "2PM Linux Class.sh"
?? aws
?? cloud/
?? devps


********************************************


Linux Commands:


touch file-name : just can create the file 

but  not we can't insert the data 

so now we are using the cat command for create along with data/content

syntax for create the file by using cat command:
  syntax:

    cat > file-name
    --------------
    -----------------

    ---------------


     ^d (ctrl+d) for save and exit 

example:
  cat > python
  hi good morning 
  python is the one of the best and easy programming language. 
  we can learn very easly 

press for save and exit ctrl+d 


append the file:
  cat>>python

we can use python for web design
frame working
net working
adminstration
automation
for big data
and so .. on 

cat file-name  : this one used for to see the data/content from a file


***********************
git diff :

example:

  git 



git branch:  
   branch list
   branch create
   branch rename
   branch delete
   branch swithch
   branch swithch create enter into new branch
   git merge
   git push origin branch name 
   git push origin --all 






6th Class:

  git add -u   : this one used for to add the files which are modified and deleted in working directory
  git commit -am "message"  : this one used for to commit the files from working and staging at a time directoly 

      note: 
        1. we can commit the files along with all staged files  
        2. we can't commit the untracked files with above command used
 

  git commit --amend --no-edit
  git reset --hard HEAD~

linux:

   rm -f file-name  : deleting the file by linux command  forcefully
   vim file-name : editing the file by using vim editor

 git rm file-name : deleting the file by git command 




 Class 7:


     git branch
     git branch <branch-name>
     git branch -m <old-Branch-name> <new branch name>
     git branch -d <exsisted branch name>
     git checkout <branch-name> 
     git checkout -b <non exsisted new branch-name>

    git merge  : this one used for to merge the data/files from one branch to another branch

       1. for merging the files from lcoal committing to working branch after applying the git fetch command
       2. this one used for to merge the files from one branch to another in local repository

    git push origin <branch name>   : this one used to send or push the files from local branches to remote repository branch

     note:  by the above syntax or command we can push only from one branch to remote branches

    git push origin --all : by this command we can push all branches at a time. 

    git pull   : this one used for to get the updates only from remote branch to local branch 

    note: by above command automatically fetch and merge into local branch by applying above command 
    git fetch   : by this command we can get into the local commit area  
    git rebase : by this we will merge into working branch after applying the git fetch 
    











   















   reset:  <-- reset is a command and it used for to unstage/ send back /call from  from staging to working directory

syntax: 1

git reset file-name : to unstage only one file at a time 

example:
  git reset aws


for unstage more than one file  
syntax: 2 

  git reset file-name file-name file-name

example:


 git rest devops linux python 
  
syntax: 3

  git reset : this one used for to reset(un stage) all files at a time  

  example 

  git reset  


syntax: 4

git reset .   <-- this one used for to reset all files at a time

syntax: 5

git reset * <-- 



syntax: 1
syntax: 1
syntax: 1
syntax: 1
syntax: 1
syntax: 1
syntax: 1
syntax: 1
syntax: 1
syntax: 1
syntax: 1
syntax: 1
syntax: 1
syntax: 1
syntax: 1






