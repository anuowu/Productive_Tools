# git 学习

## 目录

[1. git基础](#1.git基础)
- [1.1 git中文件的三种状态](#1.1git中文件的三种状态)
- [1.2 git工作流程](#1.2git工作流程)
- [1.3 git安装](#1.3git安装)
- [1.4 配置用户信息](#1.4配置用户信息)
- [1.5 获取帮助](#1.5获取帮助)

[2. git基础命令](#2.git基础命令)

## 1. git基础
### 1.1 git中文件的三种状态
在git中文件有三种状态， 已提交（commited）, 已修改（modified）和以暂存（staged。
已提交表示文件已经保存在本地数据库， 已修改表示已经修改了某个文件，但是还没有提交保存，已暂存
表示把已修改的文件放在下次提交时要保存的清单。由此确定了git工作的三个区域：git的工作目录(working directory)，暂存区域(staging area)， 以及本地仓库（git directory/repository）。
![图1.1](/images/git_working_area.png)
### 1.2 git工作流程
1. 在工作目录中修改文件
2. 对修改后的文件快照， 保存到暂存区域
3. 提交更新， 将保存在暂存区域的文件快照永久存入git目录

### 1.3 git安装
- 在linux下安装
`sudo apt-get install git`

- 在window下安装
可以从[git 官网](https://git-scm.com/download/win)下载window下的命令行工具

### 1.4 配置用户信息
+ `git config --global user.name "anuowu"`
+ `git config --global user.email 'xxx@gmail.com'`
`--global` 表示只适用于该用户的配置文件
`--system` 表示对系统所有用户都适用的配置文件
+ `git config --list` 查看已有配置信息
`git config user.name` 查看用户名
`git config user.email` 查看用户邮箱

### 1.5 获取帮助
使用`git help [order]` 查看某个order的使用

## 2. git基础命令
### 2.1 取得git项目仓库
有两种方法可以取得项目仓库：
  + 初始化本地的工作目录，`git init`
  + 从现有仓库克隆，`git clone`

如果想要对自己目前的某个目录进行管理，可以在当前目录下使用`git init`初始化，得到一个`.git`目录。如果在github上看到某个开源项目想要参与，可以使用`git clone`克隆项目到本地。

git clone的使用
`git clone [url]` 在当前目录下创建一个新的某个目录，和原项目目录一致
`git clone [url] fldername` 在当前目录下创建一个新的foldername文件夹

### 2.2 git的常用命令

+ 

+ git中的分支管理
在git中默认分支是master,可以使用  
 [1.] `git branch +分支名`创建新的分支  
 [2.] `git checkout +分支名`在不同的分支间切换分支。git中使用head指针指向正在工作的分区。  
 [3.] `git checkout -b +分支名` 相当于直接创建新的分支并切换到这个分支。  
 [4.] `git merge +分支名`把这个分支和当前所在的工作分支合并    
 [5.] `git branch -d +分支名`可以删除分支  
 [6.] 如果遇到分支冲突, 在不同的分支中对同一个文件都做了修改时  
 [7.] `git branch`命令列出当前的所有分支数  
 [8.] `git branch --no-merged`查看未合并的分支，删除未合并的分支会有提醒  
 [9.] 