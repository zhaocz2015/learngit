rest
//TODO

# git command

## git init

## git add <file>
## git commit -m "comments"

## git diff 比较的是，本地工作区与暂存区的内容
## git diff --cached 比较的是，暂存区与版本仓库的内容
## git diff HEAD 比较的是，本地工作区与版本仓库的内容


git reset HEAD <file> 从版本仓库的内容，回复到暂存区
git checkout -- <file> 从暂存区的内容，回复到本地工作区


git reset --hard HEAD^ 回退到上一个提交的版本
git reset --hard HEAD^^ 回退到上上一个提交的版本
git reset --hard HEAD~10 回退到倒数第十个提交的版本


git log 查看提交版本的日期

git log --pretty=oneline  每一个提交版本的日志，一行显示

git reflog 查看所有的版本记录


##  删除文件

rm test.txt 本地工作区删除test.txt文件

git rm test.txt 暂存区删除test.txt文件
git commit -m "提交说明" 提交至版本仓库，版本仓库的test.txt文件也会被删除

## 如果删除错误了，就使用git reset --hard HEAD^ 回退版本 


## 使用github网站，创建一个Repository代码仓库
## 本地仓库与远程仓库关联

git remote add origin https://github.com/zhaocz2015/learngit.git  关联远程仓库
git push -u origin master 推送本地仓库的提交至远程仓库 第一次使用-u之后，后面推送直接使用 
git push origin master 
git push

## 从远程仓库clone一个仓库
git clone https://github.com/zhaocz2015/learngit.git
git push -u origin master 推送本地仓库的提交
git push origin master
git push

