#LearnGit 

To create a git repository:
1. Go to GitHub page and click on Start a project
2. Enter Repository Name and Description
3. Then create a folder on your system where you want to keep the local version
4. Open terminal and go to this location and enter the below commands

echo  "# LearnGIt" >> README.md
#Creating a readme file

git init
#This command kind of makes your folder a git repository

git status
#this command shows the changes and newly added files which are yet to be added and checked in to the repositoryadded

git add README.md
#To add new files and new changes to existing files.


git commit -m "Added ReadMe File"
#Commit the changes, but this is not yet pushed to your server. Its in local.

git remote add origin https://github.com/jishinv/LearnGit.git
#creating refrence of repository to originadd

git push -u origin master
#Pushing the changes to server
