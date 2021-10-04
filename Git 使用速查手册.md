# 用户名/邮箱—查看&设置

```shell
# 查看当前项目用户名与邮箱
git config user.name
git config user.email

# 查看全局用户名和邮箱
git config --global user.name
git config --global user.email

```

```shell
# 设置当前项目用户名和邮箱
git config user.name 用户名
git config user.email 邮箱

# 设置全局用户名和邮箱
git config --global user.name 用户名
git config --global user.email 邮箱

注：用户名和邮箱不需要加引号
```

------



# 创建仓库

```shell
git init
```

------



# 文件操作

```shell
# 将文件提交至暂存区
git add 文件名
```

------



#  文件状态

```shell
git status
```

------



# 分支操作

```shell
 #查看本地分支
git branch
git branch -v 

 #查看远程分支
git branch -r
git branch -rv

# 创建分支（此操作必须是有文件提交）
git branch 分支名

# 切换分支
git checkout 分支名

# 分支合并
git merge 分支名
git rebase 分支名

# 分支取消合并
git merge --abort
```



------



# 远程仓库操作

```shell
# 添加远程仓库
git remote add 别名 远程仓库地址

# 删除远程仓库
git remote rm 别名

# 当本地仓库不是clone，需要使用此命令
git pull origin master --allow-unrelated-histories
 
 # 本地分支关联远程分支
git branch --set-upstream-to origin/master master
  
```



# SSH密钥创建&查看

```shell
# 查看ssh密钥
cat ~/.ssh/id_rsa/pub

# 设置ssh密钥
ssh-keygen -t rsa -C "邮箱"
```

`~ : 表示家目录，在windows系统中位置为C:\Users\用户名\`

