***just for note ***
to check child directories or files in a parrent directory: command: ls (which will give a list) 
then cd foldername/
to check current directory : pwd 
--------working directory to git staging--------
initialization : git init
to staging the changes all: git add --all / git add -A  [note: if you command "git add --all" in child directory it will stage all directory or all changes]
Stage present folder:  git add . [if you command git add . in a child directory it will stage only this folder]  
To unstage the changes : git reset
if you delete one file and then add another after the "git add --all" command; then command:  git add * which will add the newly added file and will not add the deleted file. 
for single file: git add filename 

-----------git stage to local repository-------
now your commitment to change.  
git commit -m "commit here anything"
now if want to back again to stage: git reset HEAD~  [before commit it was just "git reset" but after commit for back roll "git reset HEAD~"
"git rm" for romove file or folder.
"git reset --hard" [hard reset for after remove]
"git rm two.txt -f" [force to remove; when you change somting didn't commit but want remove; then force it]
git --cached two.txt 

---------git branch ------
how many branches are in your repo? checking command: git branch 
create new branch, command: git branch branchName
command : git merge development -m "merging on development with main"
command : git merge main -m "merging on main with development" 
-----merge conflict ---
go to conflict section and edit or select which change you actually want then remove rest 
----remote repository ---
"git push origin main" 
Now, if you edit anyfile from remote(means on giithub) you dont see the change in local file. 
That's why you need to fetch and merge "git fetch" then "git merge" or just command "git pull"




