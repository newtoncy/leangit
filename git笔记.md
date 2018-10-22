# git笔记

- 配置名字和邮箱

  ```shell
  git config --global user.name "Your Name"
  git config --global user.email "email@example.com"
  ```

- 查看修改

  git status 查看工作区状态

  git diff 查看修改

- 提交修改

  ```shell
    git add <file name> #添加要提交的文件
    git reset HEAD <file name> #删除暂存区的文件
    git rm <file name> #删除索引中的文件
    git commit #提交版本
    git add -A  #提交所有变化
    git add -u  #提交被修改(modified)和被删除(deleted)文件，不包括新文件(new)
    git add .  #提交新文件(new)和被修改(modified)文件，不包括被删除(deleted)文件
  ```

- 回滚

  ```shell
  git reset [--soft --mixed --hard] <commit> 
  ```

  commit可以为版本号的一部分 head^ head^^ head~10什么的

  git reset HEAD拉取暂存区里面的文件

- 日志

  ```shell
  git log #版本日志
  git reflog #命令日志
  ```

- 分支

  ```shell
  git cheakout <branch> #切换分支
  git branch <new_branch> #新建分支
  ```

- 远程仓库

  ```shell
  git remote add <origin> <url>
  git push [origin] [branck]
  ```



