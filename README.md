# Git-Cheat-Sheet
# 1-> Creating a Repository
`git init  `   
`git remote add origin [repoLink]   `   
`git remote -v  `   
`git add .   `  
`git commit -m "your message"  `   
`git push origin [branchName]  `  
 # 2-> Creating a Pull Request
### Fork the desired the Repo    
`git clone [forkedRepoLink]`    
### Do your Contribution  
`git add .`  
`git commit -m "your message"`
`git push origin [branchName]`  
# 3-> Getting Updates from the Main Repo to Your Forked Repo  
`git remote add upstream [originalRepoLink]`  
### Upstream Acts as a pointer towards the Main Repo  
`git pull upstream master`  
### Changes from the Main remote are pulled Locally  
`git push origin`    
### Changes are pushed to the Forked Remote Repo !  

 
