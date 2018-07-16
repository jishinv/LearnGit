#LearnGit 

To create a git repository:
1. Go to GitHub page and click on Start a project
2. Enter Repository Name and Description
3. Then create a folder on your system where you want to keep the local version
4. Open terminal and go to this location and enter the below commands

echo  "# LearnGIt" >> README.md
#Creating a readme file

git init
#This command kind of makes your folder a git repository This will be also done for new repository

git status
#this command shows the changes and newly added files which are yet to be added and checked in to the repositoryadded

git add README.md
#To add new files and new changes to existing files.


git commit -m "Added ReadMe File"
#Commit the changes, but this is not yet pushed to your server. Its in local.

git remote add origin https://github.com/jishinv/LearnGit.git
#creating refrence of repository to originadd

git push origin master
#Pushing the changes to server. You will have to enter your github id and password if prompted

git clone  <url>
#<url> is the repository which you want to clone or checkout to yourb system


git clone  <url>   --recursive
#checkout with submodules


git branch <new-branch>
#create a new branch from master branch

git checkout <new-branch>
#move to new branch, now you will be editing in new branch

git push origin <new-branch>
#push the new branch to remote

git pull origin master
#taking update on master branch or use just git pull


git diff
#To check for difference  and new changes in local copy


git log
#To check commit logs

git checkout --<filename>
#If you mess up you can replace the changes in your working copy with the latest contents of the head


git submodule add <submodule url> <foldername>
#Add submodule, where you specify the repository link for the submodule and the folder name in which you want to add the submodule.

git submodule update
#update the submodule

#use the commit and push now to add this as submodule in your repository

#To checkin submodule change, do the following

cd pathToSUbmodule
git add <filename>
git commit -m "message"
git push

cd pathToMainProjeect
git add <pathToSubModule>
git commit -m "message"
git push
