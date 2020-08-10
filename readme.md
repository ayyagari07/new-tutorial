The following basic git commands are used to work on repositories on the local computer and also push or pull the repositories from the remote server.  

To create a new repository on the local computer:

1. git init (name of the repository)
2. move to the created repository by typing (cd (name of the repository))
3. create a new file by typing (code (name of the file) &) --- vs code editor will be opened. Work on the file and save it before closing it.
4. before adding the file to git, check which files are modified by typing (git diff)
5. Stage the file in the git, meaning add the file in the git by typing (git add (name of the file)) 
6. to see the file that has been changed and added to the git type (git diff --cached) or type (git diff --staged)
7. now commit the files to the git by typing (git commit -m "enter a comment to what or why change has been made for future reference")
8. add the origin path to the path by typing (git remote add origin https://github.com/(user name)/(name of the repository)). 
   if the origin has been already added then you could set the url by typing (git remote set-url origin https://github.com/(user name)/(name of the repository))
Note: before doing the next step just create an empty repository in the remote server.
9. to add the commited file to the remote server type (git push --set-upstream origin master) if it is being done for the first time. 
10. now create a branch of the repository by typing (git branch (name of the branch))
11. move to the created branch by typing (git checkout (name of the branc)) -- from this point you will be working in the branch and not in the master.
12. make changes in the old files or create new files
13. before commiting the changes add the files to the git and do the commit
14. after commit push the files to repository to the remote server by typing (git push --set-upstream origin (name of the branch))
15. before merging the branch with the master move the master by typing (git checkout master)
16. after everything is done and you are satisfied with the work then the branch can merged with the master by typing (git merge (name of the branch))
17. to push the files in the master to the remote server type (git push --set-upstream origin master)


To create repository on the local machine from the existing repository in the remote server:

1. to get the repository to the local machine from the remote server type (git clone https://github.com/(user name)/(name of the repository))
2. move the newly cloned repository by typing (cd (name of the repository))
3. create a branch in order not to disturb the master branch by typing (git branch (name of the branch))



To work on the existing branch in the remote server from the local computer with already existing repository in the local computer:

1. move to the repository by typing (cd (name of the repository))
2. copy the branch from the remote server to the local computer by typing (git pull)


