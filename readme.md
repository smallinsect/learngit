first learngit commit github

note

# 设置当前机器的用户名和邮箱
git config --global user.name "Your name"
git config --global user.email "Your email"

# 查看用户名和邮箱
git config --global user.name
git config --global user.email

# 添加远程库
# 要在github.com网站新建一个learngit库
# 将本地与我的远程库关联
git remote add origin git@github.com:smallinsect/leargit
# 将本地库的所有内容推送到远程库上，第一次腿上加-u
git push -u origin master
# 从现在起，只要本地提交，就可以通过命令
git push origin master

# 从远程库克隆
git clone git@github.com:smallinsect/learngit

# 把文件添加到仓库
git add file1.txt
# 把文件提交到仓库
git commint -m "wrote a readme file1.txt"

# for example
git add file1.txt
git add fi1e2.txt file3.txt
git commit -m "add 3 file"
