# learningGitAndGithub
This readme file contains all the basic git commands

  $cd <directory name>  //use to change the directory
  
  $ cd ..  //folder up
  
  $ mkdr <directory name>  //make new directory or folder name
  
  $ git status  //status of git
  
  $ git init/ git init . // initialize git in that directory
  
  $ rm -rf .git  //remove the directory from git
  
  $touch <file name>  // create a file in the current directory
  
  $ git add <file name>  // will add the file in staging area where changes can be made
  
  $ git rm --cached <file name>  // unstage the file 
  
  $ git add .  // will add all the files in current directory and downwards to staging area
  
  $ git rm -r --cached . // unstage all the files
  
  $ git add -A  //add all the files(upwards or downwards) in staging area
  
  $ git commit -m "message"  // commit the files with message
  
  $ git log  // see the changes made in files or repo

  $ git log --oneline  // see changes of each file in oneline i.e. only commit message
  
  $ vi <file name>  //open the file   --> i  //now we can make changes their itself  -->  esc :wq
  
  $ cat <file name>  // show the file
  
  $ git diff  // show the differences made after the last commit
  
  $ git restore <file name>  // restore the file from changes made since last commit
  
  $ git --ammend -m "message"  // changes the message of last commited file
  
  $ git branch -r  //branches in the remote server i.e. github

  $ git branch -a  // all the branches

  $ git branch <branch name> // create a new branch

  $ git checkout <branch name>  // switch to given branch from main branch

  $ git checkout - // switch to previous branch

  $ git push --set-upstream origin <branch name> OR $ git push -u origin <branch name> // push the branch to github

  $ git checkout -b <branch name>  //create a new branch and directly switch to it

  $ git branch -d <brach name>  // delete given branch, note that to delte a branch we must be in upward branch, main in this case

  $ git merge <branch name>  // merge the given branch to main branch in our system other way is to create pull request for remote server

  solving conflicts: if you made some changes in your branch and meanwhile their are some commits in master branch on the file you are working
		then you can't push your branch directly to the github, you must first pull the changes and then resolve conflicts of which changes
		need to be prefered and then push the branch

  git rebase : suppose you are working on side branch and	main branch on remote server has moved on and you dont have commit from main 
	branch, so what rebase does is it is going to bring all the changes from whichever branch you want and put your changes(which you did
	on your branch) on top of it

  $ git pull -r origin main/master  --> resolve conflicts manually --> git rebase --continue --> git push -f

  

