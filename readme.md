first learngit commit github

# 个人网站

- https://用户名.github.io
- https://smallinsect.github.io

## 搭建步骤

- 1)创建个人站点

创建仓库（注：仓库名必须是【用户名.github.io】）

- 2)在仓库下新建index.html

- 3)

# 项目网站搭建

## 去项目路径 点几settings





# 指定某个文件或文件夹回退到某个版本

1. 一看就知道要用哪个命令：
git checkout [<options>] [<branch>] -- <file>...
2. 那么执行的时候就是这个样子：
git checkoutee25a1a3f9465 config/database.php
3. 如果要回退整个文件夹到某个版本呢？
git checkout e2fb85c827d24a460d app/Http/Controllers/Auth
4. git强制回退到上一个版本：

git reset --hard HEAD^

# 设置当前机器的用户名和邮箱
* git config --global user.name "Your name"
* git config --global user.email "Your email"
# 查看用户名和邮箱
* git config --global user.name
* git config --global user.email
* git config --list
# 连接远程库
* 创建SSH Key。在用户主目录下，看看有没有.ssh目录，如果有，再看看这个目录下有没有id_rsa和id_rsa.pub这两个文件，如果已经有了，可直接跳到下一步。
如果没有，打开Shell（Windows下打开Git Bash），创建SSH Key：
ssh-keygen -t rsa -C "youremail@example.com"


# 创建版本库
* mkdir learngit
* cd learngit
* pwd
* git init

# 把文件添加到仓库
* git add file1.txt
# 把文件提交到仓库
* git commint -m "wrote a readme file1.txt"


# for example
* git add file1.txt
* git add fi1e2.txt file3.txt
* git commit -m "add 3 file"
* git add *	添加所有修改的文件

# 删除文件
* git rm -rf hehe
# 删除远程库文件
* git rm -rf --cached hehe

# 添加远程库
# 要在github.com网站新建一个learngit库
# 将本地与我的远程库关联
* git remote add origin git@github.com:smallinsect/leargit
# 将本地库的所有内容推送到远程库上，第一次腿上加-u
* git push -u origin master
# 从现在起，只要本地提交，就可以通过命令
* git push origin master

# 从远程库克隆
* git clone git@github.com:smallinsect/learngit

# 查看版本控制系统 历史记录
* git log

* 上一个版本是HEAD^
* 上上个版本是HEAD^^
* 上100个版本是HEAD~100
# 版本回退
* git reset --hard a0fvf8
* git reset --hard HEAD^
* git reset --hard 本版号前7位数
* git revert 5lk4er 

记录你的每一次命令 
* git reflog
* git checkout -- [file name] 
* （若文件有修改，可以还原到最初状态; 若文件需要更新到服务器上，应该先merge到服务器，再更新到本地
# 查看当前分支情况
* git branch
# 若分支位本地分支，则需切换服务器的远程分支
* git checkout [remote branch]若分支为本地分支，则需切换到服务器的远程分支)
# 从远程库更新到本地
* git pull

# 错误 `Could not resolve host: github.com`
1. 查看ip地址
    * ping github.com
2. 打开文件 C:\Windows\System32\drivers\etc
    * 添加 13.229.188.59   github.com