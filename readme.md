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
- 默认有个主分支master,是一条commit链条
### 创建分支
- 创建一个dev分支,分支创建时dev里内容和master内容是一样的
    - git branch dev
- 创建并进入分支dev
    - git checkout -b dev
### 切换分支
- 切换到dev分支
    - git checkout dev
- 查看当前有哪儿些分支
    - git branch
### 合并分支
- 合并把当前分支与指定分支进行合并
    - git merge dev
    - 当前分支至git branch 星号所在的分支
    - 合并分支前，另一个分支提交了内容，合并时会产生冲突，需手动处理，并重新提交
### 删除分支
- 在master分支删除指定分支dev
    - git branch -d dev
    - 在当前分支删除当前分支是删不掉的

### 提交代码到github
- git push [地址] master
    - git push git@github.com:wowweihuacao/gitstudy.git
    -或者给远程仓库设置一个别名：git remote add origin git@github.com:wowweihuacao/gitstudy.git，以后提交，第一次使用git push -u origin master建立关联，之后使用git push推送就行
    - 会把当前分支内容上传到远程master分支上

--------------------
- git pull [地址] 分支名称
    -  git push git@github.com:wowweihuacao/gitstudy.git master
    - 会把远程分支的数据得到：本地先需要一个初始仓库







