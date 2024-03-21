---
title: chmod命令.md
date: 2024-03-21 16:31:37
tags: 
categories: 
---

# chmod命令

用以修改文件/文件夹的权限信息

> 只有文件/文件夹的所属用户或root用户才能修改

## 语法

chmod [-R] 权限 文件/文件夹

> -R 表示对文件夹内的全部内容应用同样的操作

### 示例

### chmod u=rwx,g=rx,o=x c.txt

> u g o 对应 user group other，表示赋予不同群体什么权限

## 数字式语法（chmod）

![image-20240304131503096](/home/melody/.config/Typora/typora-user-images/image-20240304131503096.png)

![image-20240304131535041](/home/melody/.config/Typora/typora-user-images/image-20240304131535041.png)

> eg.
>
> ![image-20240304131740163](/home/melody/.config/Typora/typora-user-images/image-20240304131740163.png)

