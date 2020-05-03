(Our local repository is identical to remote repo : files inside folder change according to branch (localy) )

# put directory where you want to download the code 

git clone <repository link>


# you can make new branch localy and switch to:

git checkout -b “<new branch>” 

# show my local branches 
git branch

# show all branches locally and in git 
git branch -a

##show branches remotely git
git branch -r

##now you can check on which remote branch we are  

git status 

##  if you are not on the right branch localy: 
git checkout <new branch> 

## push my new  local branch to remote repo (origin) without add or commit, but you don’t push the change now, only the new branch, you need add and commit to push changes
git push origin <my new local branch name>



## then add the files to local repository to specific branch I am in : 
git add .

## now commit the code : 
git commit -m “edit by me”

##after commit It is better to write
clear


##now push the code git push,It pushes all the changing that is why we switch to our local branch and change in it, not stay ##in master to apply change on our branch :
git push 
Or 
git push -u origin <branch-name> 


##push is the opposite of fetch and merge, after changing in our local repo we pushed to remote repo to fetch
##Commit means new copy of this branch but does not mean new branch 
————————————————————————————————————————————————————————————————————————————
##lists references in local repository
git show-ref



##Remove all branches in local repository Necessary earn there are two repositories 
rm -rf .git

##Initialize local repo
git init

## to connect to the repository (origin : repo name)
git remote add origin https://github.com/user/repo.git

## to fetch with repo (pull include fetch and merge) It is better to mention the name of repo we want to fetch with 
git fetch 
Or 
Git fetch origin

##to fetch the master , It is after fetch we mean ( origin : name of repo, master : the branch )
git merge
Or 
git merge origin/master 

##show us the name of remote repo (origin as default) or if we add another repo  (upstream)
git remote -v

## remove the repository remote or upstream 
git remote remove <origin or upstream> 

#Remove a file Useful when I want to detelet tracked file 
git rm <file-name> 
git rm <file-name> -f


##When there is overwrite we can use : 
git add  - -all

##to see all the commits
git log



##if there if files not sending 
git add <filename> -f
git commit -m “lsadjkas”
git push 

##addition files could be in remote repo not local



## remove the connection with remote repository (origin : remote repo)
git remote rm origin
