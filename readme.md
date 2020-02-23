# Git 教程
## git安装
- 见官方
## 初始化git仓库
- 命令：git init
## 在git中全局配置用户信息
- 命令：
    + 配置用户名：git config --global user.name "andy"
    + 配置邮箱： git config --global user.email "183458525@qq.com"
## 把代码放到.git仓库中
1. 把文件添加到暂存区
    - git add ./readme.md
    - git add ./   可以全部提交
2. 把文件添加到仓库中
    - git commit -m "提交说明文字"
    - git commit --all -m "全部提交暂存区的文件到仓库"
## 查看当前文件状态
- git status
## 查看git日志
- 会使用时间线进行记录 ，由近及远，打印提交的全部信息
    - git log
- 查看简洁信息，一行显示一条记录
    - git log --oneline

## 回退到指定版本
- 回退到上次代码提交的状态
    - git reset --hard Head~0
- 回退到上上次代码提交的状态
    -  git reset --hard Head~1
- 通过版本号精确回退到某次提交时的状态
    - git reset --hard 版本号
- 查看每一次切换版本的记录
    - git reflog

## 分支
- 默认有个主分支master
### 创建分支
- 创建一个dev分支,分支创建时dev里内容和master内容是一样的
    - git branch dev
### 切换分支
- 切换到dev分支
    - git checkout dev
- 查看当前有哪儿些分支
    - git branch
### 合并分支
- 合并把当前分支与指定分支进行合并
    - git merge dev
    - 当前分支至git branch 星号所在的分支
### 删除分支
- 在master分支删除指定分支dev
    - git branch -d dev
    - 在当前分支删除当前分支是删不掉的

这是在master上的任务

