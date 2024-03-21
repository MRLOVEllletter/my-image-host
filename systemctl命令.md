---
title: systemctl命令.md
date: 2024-03-21 16:31:38
tags: 
categories: 
---

# systemctl命令



LInux系统很多软件（内置或第三方）均支持使用systemctl命令控制：启动，停止，开机自启

而能够被systemctl管理的**软件**，一般也称之为：**服务**

## 语法

systemctl **start | stop | status | enable | disable** 服务名

> 加粗的是功能
>
> ![image-20240304142936518](/home/melody/.config/Typora/typora-user-images/image-20240304142936518.png)
>
> 系统内置的服务包括：
>
> - NetworkManger，主网络服务
>
> - network，副网络服务
>
> - firewalld，防火墙服务
>
> - sshd，ssh服务
>
>   ​	......

