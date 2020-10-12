# Git-Cheat-Sheet
## 0-> Configuring the Bash Terminal
`git config --global user.name “Your Name”`    
`git config --global user.email “Youremail@anything.com”`    
## 1-> Creating a Repository
`git init  `     
`git remote add origin [repoLink]   `   
`git remote -v  `   
`git add .   `  
`git commit -m "your message"  `   
`git push origin [branchName]  `  
 ## 2-> Creating a Pull Request
### Fork the desired Repo    
`git clone [forkedRepoLink]`    
### Do your Contribution  
`git add .`  
`git commit -m "your message"`  
`git push origin [branchName]`  
## 3-> Getting Updates from the Main Repo to Your Forked Repo  
`git remote add upstream [originalRepoLink]`  
### Upstream Acts as a pointer towards the Main Repo's remote  
`git pull upstream master`  
### Changes from the Main remote are pulled Locally  
`git push origin`    
### Changes are pushed to the Forked Remote Repo !  
## 4-> Get Information about Your Commits
`git log --pretty=oneline`  
## 5-> Move to Your Desired Commit or Branch
`git checkout hash/branch` 
## 6-> Undoing Staged Files
`git reset HEAD <file>`  
### where HEAD can be your Hash number (First Four Digits will do fine) or your Branch Name  
## 7-> Undoing Commited Files
`git revert HEAD`  
###  where HEAD can be your Hash number (First Four Digits will do fine) or your Branch Name  
## 8-> Pulling changes Locally from a Remote Repo
`git pull origin [branchName]`  
### where origin can be replaced by the respective remote pointer  

  

 
