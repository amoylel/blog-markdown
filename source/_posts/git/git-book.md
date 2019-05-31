---
title: Git学习笔记
date: 2019-05-30 17:47:20
tags: git
categories:
    - GIT
---

## 1. init

初始化一个版本库

```github
    #初始化一个版本库, 主要用于客户端
    git init 
    # 初始化一个版本库，主要用于服务端
    git init --bare
    
```

<!--more-->

## 2. config

配置`git`参数
+ --global 作用到域当前用户
+ --system 作用域为整个系统
+ --local 作用域当前项目

**参数优先级：** git config > git config --global > git config --system

+ 设置用户名： `git config --global user.name "usename"` 

+ 设置用户邮箱：  ` git config --global user.email "email@emil.com"`
+ 设置命令别名： `git config --global alias.br branch`, 可使用`git br`代替`git branch`命令
```Bash
    # 设置用户名
    git config --global user.name "username"
    # 设置用户邮箱
    git config --global user.email "email@emil.com"
    # 设置命令别名, 可用 git br 代替 git branch
    git config --global alias.br branch
```



## 3. add

将文件添加到暂存区
+ 添加所有.txt结尾的文件到暂存区

```
   git add *.txt
```

```git
    # 添加所有.txt结尾的文件到暂存区
    git add *.txt
    # 添加全部文件到暂存区
    git add -A
    # 会轮流询问每一个文件是否需要添加
    git add -p
    #交互式暂存
    git add -i 

```

