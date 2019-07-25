# Git + GitHub

1. initialize git in your folder
  ```
  git init
  ```
2. add files
  ```
  git addFileName.xxx
  git add . (if you want to add all the files)
  ```
3. commit
  ```
  git commit -m "message for this commit"
  ```
4. push
  ```
  git push --set-upstream git@github.com:yourName/repositoryName.git branchName (if you push for the first time?)
  ```

# Git + VS Code
Using the former commands, you can use Git Bash to connect to your repository already, you can use `git push` to easily push your commits to the remote repository you used last time (it works like this for me). But it still cannot be pushed to remote repository in VS Code. To enable push and fetch in VS Code, you need to first add the remote repository.
```
git remote add [name this remote connection, usually 'origin'] [remote repository URL]
```
Then you can check if you're connected by checking remote branches
```
git branch -r
```
if the branches in remote repository appears, it means you have connected. Then you can push your commits to remote repository in VS Code.

> Some other things good to know, you can open `config` file in `.git` to check your branches and remote repositories. If you have added extension "Git Graph", you can easily check and set remote repositories by clicking the gear icon.
