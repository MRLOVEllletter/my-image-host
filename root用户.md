---
title: root用户.md
date: 2024-03-21 16:31:38
tags: 
categories: 
---

# root用户

## 什么是root？

在Linux中root用户拥有最大的操作权限，又称超级管理员

### 权限

普通用户一般在自己的HOME目录内是不受限的

一旦出了HOME目录，大多数地方都只有只读和执行权限，无修改权限

## su和exit命令

### su命令

> switch user

#### 语法

su [-] 用户名 

> -符号是可选的，表示是否加载环境变量，一般建议加上
>
> 用户名也可以不加，如果不加的话默认是切换到root用户
>
> 从一个账号切换到另一个账号后，要想退回原来的账号，
>
> 可以用exit命令，或者快捷键crtl+d
>
> 从普通用户到root用户要输入密码
>
> 从root用户到普通用户不用输入密码

## sudo命令

> Substitute *User* *DO*

作用是可以让一条命令以root权限去运行

### 前因

因为su命令所赋予的长期使用root账户很容易造成误操作，所以需要短暂的root权限

### 配置

sudo命令需要root权限的配置

1. su - root切换到root用户
2. 输入visudo，打开配置文件并进行编辑
3. 在最后一行输入melody ALL=(ALL)         NOPASSWD: ALL

> NOPASSWD前的空格是一个TAB的距离

![image-20240302123949538](/home/melody/.config/Typora/typora-user-images/image-20240302123949538.png)

> [csdn上的root权限相关知识](https://blog.csdn.net/weixin_44803446/article/details/103530746)

这样配置完毕

每次用root权限时，只需要在命令前加个sudo就行了

> eg.
>
> sudo visudo

