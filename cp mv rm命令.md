---
title: cp mv rm命令.md
date: 2024-03-21 16:31:37
tags: 
categories: 
---

# cp mv rm命令

## cp命令

用于复制文件/文件夹

> copy

### 语法

cp [-r] 参数1 参数2

> -r 全称为recursion，用于复制文件夹，直译是递归
>
> 参数一，代表路径，表示被复制的文件或文件夹
>
> 参数二，代表路径，表示要复制去的地方

> eg.
>
> cp awa.txt awa2.txt
>
> cp -r awa awa2

## mv命令

用于移动文件/文件夹

> move

### 语法

mv 参数1 参数2

> 参数一，代表路径，表示被移动的文件夹
>
> 参数二，代表路径，表示被移动去的地方，
>
> 如果目标不存在则有改参数一名字的效果

> eg.
>
> mv awa.txt Desktop/
>
> mv awa.txt awa2.txt

## rm命令

用来删除文件/文件夹

> remove

### 语法

rm [ -r -f ] 参数1 参数2 ... 参数n

> -r和cp的r相同，都是用于复制文件夹
>
> -f用于强行删除（管理员看不到消息）

