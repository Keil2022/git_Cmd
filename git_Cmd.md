## 查看用户名和邮箱地址：  
git config user.name  
git config user.email  

## 修改用户名和邮箱地址：  
git config --global user.name  "xxxx"  
git config --global user.email  "xxxx"  

## 修改本地分支：  
git branch -m <old_branch> <new_branch>

## 删除远程分支：  
git push origin :<old_branch>

## 切换到本地新分支，将本地新分支推到远程：  
git checkout <new_branch>  
git push --set-upstream origin <new_branch>

## 查看本地分支：  
git branch -a

## 本地分支关联远程分支:  
git branch --set-upstream-to=origin/sit-basic-v1.0.1

## 查看分支关联情况:  
git branch -vv  

## 新建项目：  
初始化——————git init  
修改本地分支名称—git branch -m master main  
添加到本地仓库——git add .  
提交到本地仓库——git commit -m "文件说明"  
关联远程仓库———git remote add origin “项目地址”  
上传本地代码———git push -u origin main  

## 上传项目到已有仓库分支：  
初始化————————git init  
创建分支———————git branch test	（”test“为分支名）  
切换分支———————git checkout test  
上传修改的文件————git add . —— "." 可替换成具体要上传的文件名，"."  表示提交所有有变化的文件)  
添加上传文件的描述——git commit -m "test"  
与远程分支相关联———git remote add origin “项目地址”  
将分支上传——————git push origin test  

## 下载项目到本地：  
初始化—————git init  
关联远程项目——git remote add origin <你的项目地址>  
下载项目到本地—git clone <项目地址>

## 下载项目分支到本地：  
git clone -b "项目名" “项目地址”

## Git 可以在你提交时自动地把回车（CR）和换行（LF）转换成换行（LF），而在检出代码时把换行（LF）转换成回车（CR）和换行（LF）：  
git config --global core.autocrlf true