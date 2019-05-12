# git_command
git命令

1. git init 初始化repository .git
2. git add . 添加path的文件到.git
3. git commit -a -m 'comment'  提交跟新到本地分支
4. git pull 从远程仓库分支拉取最新的跟新代码
5. git push 从本地推跟新到远程分支

## 分支

1. git branch  查看本地分支
2. git branch -r 查看远程分支
3. git branch -a 查看所有分支
4. git checkout 分支名 切换到本地分支(没有则创建 git checkout -b 分支名创建分支 在当前分支下)
5. git push origin 本地分支名 将本地分支推送到远程(创建远程分支)
6. git branch --set-upstream-to=远程分支名 (将本地分支（当前）关联到远程分支)
7. git checkout -b 本地分支名 远程分支名   切换远程分支(意思为checkout 远程的分支 ，在本地起名为[本地分支名]的分支，并切换到本地的分支)
8. 合并分支

> 合并前要先切到<b>要并入</b>的分支  git checkout 要并入其他分支的分支  ---> 合并分支 git merge 要被并入的分支  

9. 删除分支

> 先提交本地分支到远程分支 然后 切回到主分支或者其他分支  执行git branch -d <本地分支> 执行删除， 然后删除远程分支 git push origin --delete <远程分支名> 执行删除远程分支
