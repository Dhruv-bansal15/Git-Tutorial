# General commands 
1. pwd => to show the present working directory 
2. ls => to show all the files and folders in current directory 
3. cd <folderName> => to enter in a folder of current directory 
4. touch <filename> => to create a file in current directory which you are in 
5. 


# Some basic commands every time you guys will use 
1. git init => To declare that the current directory is a git repo and git will have an eye over all the changes made here 
2. git remote add origin <url> => to refer to the repo in github where u wish to push all the data

# Various ways to stage changes
1. git add -A or git add --a => stages all changes

2. git add .  => stages new files and modifications, without deletions (on the current directory and its subdirectories).

3. git add -u => stages modifications and deletions, without new files

4. git rm <filename> => to stage a particular file only 

# Commit the change 
1. git commit -m <commit message (in inverted commas)> 

# Remove a file from staging area 
1. git restore --staged <filename>

# Stage and commit simontaneously 
1. git commit -a -m <"commitMessage"> 

# push to origin 
1. git push origin master => to finally see the reflected changes in your master branch on github 

# To see prev commits 
1. git log => View all the prev commits  
2. git log -p -i => to show the last i commits 
3. git log --preety=short => display all the commit info in very precize way and simpler to understand 

# To make a repo back to normal, i.e not a git repo anymore 
1. rm -rf .git 

# .gitignore file 
*log => then git will not track all the .log files present in your repo/directory

# To compare between staged and unstaged and present dir 
1. git diff --staged => will only show changes to files in the "staged" area.

2. git diff HEAD => will show all changes to tracked files. If you have all changes staged for commit, then both commands will output the same.

precisely we can say, 
1. git diff :- View difference between Stage and Working Directory
2. git diff --staged :- View difference between HEAD and Stage
3. git diff HEAD :- View difference between HEAD and Working Directory

# To clone a Repo 
1. git clone <url> <Name> => It will clone the repo linked to url with all the prev commit info and copy the files in your folder with name <Name>

# Stop tracking a file 
1. git checkout -- <filename>