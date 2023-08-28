# Git-Cheat-Sheet
## Git Bash Terminal  
[Download the Terminal from here](https://git-scm.com/downloads)  

### 0-> Configuring the Bash Terminal
`git config --global user.name “Your Name”`    
`git config --global user.email “Youremail@anything.com”`    
### 1-> Creating a Repository
`git init  `     
`git remote add origin [repoLink]   `  
#### Origin works like a pointer to the repoLink, making the referencing easier 
`git remote -v  `   
`git add .   `  
`git commit -m "[your message]"  `   
`git push origin [branchName]  `  
 ### 2-> Creating a Pull Request
#### Fork the desired Repo    
`git clone [forkedRepoLink]`    
#### Do your Contribution  
`git add .`  
`git commit -m "your message"`  
`git push origin [branchName]`  
### 3-> Getting Updates from the Main Repo to Your Forked Repo  
`git remote add upstream [originalRepoLink]`  
#### Upstream Acts as a pointer towards the Main Repo's remote  
`git pull upstream master`  
#### Changes from the Main remote are pulled Locally  
`git push origin`    
#### Changes are pushed to the Forked Remote Repo !  
### 4-> Get Information about Your Commits
`git log --pretty=oneline`  
### 5-> Move to Your Desired Commit or Branch
`git checkout hash/branch` 
### 6-> Undoing Staged Files  
`git reset HEAD <file>`  
#### where HEAD can be your Hash number (First Four Digits will do fine) or your Branch Name  
### 7-> Undoing Commited Files
`git revert HEAD`  
####  where HEAD can be your Hash number (First Four Digits will do fine) or your Branch Name  
### 8-> Pulling changes Locally from a Remote Repo
`git pull origin [branchName]`  
#### Where the origin can be replaced by the respective remote pointer.  
### 9-> View the state of your Staging Area and Changes in your Directory
`git status`    
### 10-> View the History of your Commits along with their Hash Codes of the Repo  
`git log --pretty=oneline`  

### 11-> View the difference between branches    
`git diff --color thatBranchNameYouWantToCompare`    

### 12-> Delete a branch remotely    
`git push origin --delete <branch>`  

### 13-> Unstage your changes
`git reset`

### 13-> Unstage your changes and reset the working directory
`git reset --hard`

### 13-> Revert back to the last commit (Undo Last Commit)  
`git reset HEAD~1` 

**OR**  

`git revert [last-commit-hash]` (This will create a new commit for reverted changes)


## Some Questions and Answers !!
### Q1-> I have pushed some commit/s that I shouldn't. Now, I want to remove them locally and remotely. I want my History on Github to be cleared of those wrong commits. What should I do ??  
#### First, see your commits, understand them and select how many commit/s you want to delete.  
`git log --pretty=oneline`    
#### Now, choose a number of commits you want to change i.e lets say recent 4 commits and delete them locally. Type the following command and simply remove the commits in your text editor(simply delete the line) and save the file  
`git rebase -i HEAD~4`    
#### Check your commit tree by using git log command and become sure that your commits have been removed locally. Once, you're certain, push the remaining commits.
`git push origin branchName --force`  
#### Your History will be altered and the commits will be removed remotely as well as locally    
### Q2-> How can I pull a certain branch from GitHub ?
`git fetch origin`  
`git branch -f [branchName]/[branchName]`  
`git checkout branchName`  
#### This command will create a branch of the same name of the remote branch that you're going to pull from   
  

  

 
