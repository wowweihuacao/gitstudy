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
    -  -git reset --hard Head~1

