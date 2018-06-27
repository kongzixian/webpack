











1.git init
2.git status
3.git add -all
4.git config --global user.name author #kongzixain
5.git config --global user.email author@15218803807@163.com
6.git commit -m '提交内容日志'



1. 先在github上创建一个项目：例如 vue-demo

2. 在本地vue-demo 项目中使用 git init 把其变成git可以管理的仓库

git init
1
3. 若要忽略本地的文件或文件夹不被提交到github ，则需要在项目根目录下创建 .gitignore 文件

touch .gitignore
1
2
4. 打开文件，编辑内容，例如：


node_modules/ 
update.txt 

则可以忽略目录下node_modules 文件夹及updata.txt 文件.

配置文件可以在github在线浏览

5. 添加文件夹下所有文件到暂存区 git add .

git add .
1
6. 把文件提交到仓库 git-commit -m “”

git commit -m 'decriptions'
1
5. 关联远程仓库 （第一次使用需要添加github公钥）

git remote add origin https://github.com/kongzixian/webpack.git
1
2
或者

git remote add origin https://github.com/***/vue2.1-sell.git
1
2
6. 获取远程库与本地同步（远程仓库不为空需要这一步）

git pull --rebase origin master
1
7. 把本地内容推送到远程库 使用 git-push

git push -u origin master
