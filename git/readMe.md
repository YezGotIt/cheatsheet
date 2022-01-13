# Git CheatSheet Basic

## Requirements :
- ### install git [link](https://git-scm.com/download/win)

<br>

### *Note*: default add .gitignore file in your repository

## 1. Adding the user name and email in git
### By globally

    - git config --global user.email "you@example.com"

    - git config --global user.name "Your Name"

    - git config --global user.password "your password"


### Only in current repository

    - git config user.email "you@example.com"

    - git config user.name "Your Name"

    - git config user.password "your password"

## 2. Initial the git in your current directory.

    - git init

## 3. Adding to the local repository.

    - git add . || git add <fileName>  

## 4. Checking the status.

    - git status

## 5. Commit your code
    - git commit -m "your message" 
    - git commit -am "your message" 
### If last commit message is an typo  
    - git commit --amend -m "your message"
    - git commit --amend --no-edit
        - KG --> certutil -hashfile <file path> sha256 (hash value)
### To create your alias
    - By globally
        - git config --global alias.co checkout
        - git config --global alias.br branch
        - git config --global alias.ci commit
        - git config --global alias.st status
        - git config --global alias.ca "commit -am"

        - By local directory
        - git config alias.co checkout
        - git config alias.br branch
        - git config alias.ci commit
        - git config alias.st status
        - git config alias.ca "commit -am"   

### Create commit message properly 
![one](./ss/1.png)

### [link](https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/)


## 6. See the git log
    - git log
    - git log --oneline --graph --decorate --all
### [link](https://explainshell.com/explain?cmd=git%20log%20--oneline%20--graph%20--decorate%20--all#:~:text=%2D%2Doneline%20This%20is%20a,history%20to%20be%20drawn%20properly.)


## 7. Use of checkout
    - git checkout log/branch
    

## 8. Use of push
    - git push origin master
### if use -u keyword
    - git push -u origin master


## 9. Use of pull
    - git pull <remote> <branch> 
### if use -u keyword
    - git pull  

## 10. Use of fetch
    - git fetch <remote> <branch>    


## Adding personal access token
    - git remote set-url origin https://username:token@github.com/username/repository.git     