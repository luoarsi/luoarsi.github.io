---
title: "Git的简单命令"
date: 2021-09-17T17:19:17+08:00
draft: false
---

#### 在gitee或github中下载一个项目：

1. 本地新建一个文件夹
2. 在gitee或github中复制下载路径的【URL】
3. 右键打开Git Bash Here，输入git init
4. 输入“git clone【URL】”回车



#### 上传更新的代码到仓库去：

1. (Git status)
2. Git add .   // 添加修改
3. Git commit -m ”XXX”
4. Git pull
5. Git push origin master



#### 上传本地文件到gitee或github：

前提：已经在gitee或github里面新建了一个“与本地要上传文件同名”的仓库

1. 删除 .git 文件
2. cd 到文件目录下（在cmd里cd到文件目录下或者直接在本地目录右键打开Git Bash Here）
3. git init
4. git config --global user.name”胡思佳”
5. git config --global [user.email”2943767211@qq.com”](mailto:user.email\”2943767211@qq.com\”)
6. git add .
7. git commit -m “first commit”
8. git remote add origin https://gitee.com/某某某.git
9. git push -u origin master

 

#### 工作流程：

“git pull origin master”

// 上班的时候 开始pull 最新版本的代码

// 开始写代码

// 在 pull 一下代码

// 下班 上传push代码 

 

#### 解决冲突：

<<<<<<< HEAD

//zhihu@1

//zhihu@2         （要么删掉这儿）

//zhihu@3

//zhihu@4

=======

//root@1

//root@2          （要么删掉这儿）

//root@3

//root@4

 

解决玩冲突就重新提交

git add .   // 添加修改

git commit -m '我是注释'  //提交代码到本地仓库 -m 表示写一个注释

Git push origin master   // 推送代码到远端仓库
