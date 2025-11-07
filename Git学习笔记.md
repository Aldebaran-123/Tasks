# Git学习笔记

## 一、什么是Git

​        Git 是一个开源的分布式版本控制系统，用于高效地处理从小到非常大的项目版本管理。与集中式版本控制不同，Git 每个客户端都保存有完整的代码仓库（包括历史记录），支持离线工作，具有更灵活的分支管理机制

* **工作区**：用来放代码的地方
* **暂存区**：暂时存放改动，保存即将提交的内容
* **本地仓库**：git的版本库，会有一个隐藏的目录.git，打开文件资源管理器中的隐藏的项目就能看到
* **远程仓库**：要上传到的地方，如GitHub和gitee，可用于备份和团队协作

## 二、Git的用户配置

​        使用Git必须配置用户名和邮箱，配置一次以后就可以使用了，在gitbash里写以下代码

git config --global user.name "用户名"
git config --global user.email "邮箱"

*用户名和邮箱用GitHub或gitee的*

## 三、常用git命令                

| 命令                       | 说明                           |
| :------------------------- | :----------------------------- |
| `git init`                 | 初始化本地仓库                 |
| `git clone [url]`          | 克隆远程仓库                   |
| `git status`               | 查看当前仓库状态               |
| `git add <file>`           | 添加指定文件到暂存区           |
| `git add .`                | 添加当前目录的所有修改到暂存区 |
| `git commit -m "message"`  | 提交暂存区到本地仓库           |
| `git log`                  | 查看提交历史                   |
| `git log --pretty=oneline` | 简洁显示提交历史               |
| `git diff`                 | 查看工作区与暂存区的差异       |

## 四、如何用Git bash提交并推送文件到远程仓库

* 1、先在git上配置用户和邮箱（**重要**）
* 2、选择要上传的文档，右键点击选择git bash
* 3、输入git init
* 4、输入git add . 选中文件加入暂存区
* 5、输入git commit -m"任意字符“将文件提交到本地仓库
* 6、输入git remote add origin 仓库地址
* 7、输入git pull origin main
* 8、输入git pull origin main --allow-unrelated-histories（如果自建了README文件的话）
* 9、输入git push -u origin main进行推送

## 五、其他提交方式

个人觉得git bash比较麻烦，尤其是刚刚接触，根本搞不懂怎么上传文件。因此在网上找到了其他更好用的方式

* VS code（已尝试，很好用）

  内置git面版，可以提交、分支切换、差异对比，功能强大

* Github Desktop（网上说好用，我还没试）

  GitHub官方工具，界面简洁，深度集成GitHub功能

  