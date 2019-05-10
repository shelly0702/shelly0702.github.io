---
title:  "git相关操作命令"
date:   2018-12-28 14:40:00 +0800
author: "廖艳丽"
---

### 常用的git命令
- git status 查看仓库状态
- git add . 提交所有更改
- git commit -am '提交注释'
- git push 推送所有提交的内容到远程仓库


### 分支相关命令
- git branch 查看仓库所有命令
- git checkout aaa 切换仓库分支
- git checkout -b aaa 创建aaa分支
- git push origin aaa 提交aaa分支到远程仓库

### 切换到某个历史版本的命令
- git reset --hard fcdc86dd 本地回到fcdc86dd版本
- git push -f -u origin master 将本地的修改推送至远程仓库，远程仓库此时也会回到fcdc86dd版本

### vscode中合并分支。举例：将bbb分支的内容合并至dev分支
1. 切换至dev分支
2. 按住ctrl+shift+p出现合并分支的选项，选择bbb
3. 合并完成后推送至远程仓库
