# 半圆笔记
## 6.将practice下的new开头的文件夹都删除掉
修改后：

* find ./ -type d -name "new*" | xargs -d '\n' rm -rf '{}'(在Linux下合法)
* find ./ -type d -name "new*" -print0 | xargs -0 rm -r(在mac os 下合法)

## vim
### 三种模式
* normal
* insert
* visual

esc 切换模式
## normal模式
：命令行

使用 :set showmode 打开状态栏用以显示当前的模式（注意：normal模式不会被显示出来）

使用 Esc 从 insert 进入到 normal 模式
## insert模式（输入文本）

使用 i 或者 a 从 normal 进入到 insert 模式

## 保存退出
* 保存：在 normal 状态下 输入 :w
* 退出：在 normal 模式下输入 :q
* 保存并退出：在 normal模式下输入 :wq

## 移动
* k往上移动
* j往下移动
* h往左移动
* l往右移动
* w e 往后移动一个词
* b 往前移动一个词
* 0移到行首
* $移到航尾

## 复制粘贴
y复制
p粘贴

## 记录行号
set nu

移动到行号

（行号）+gg

## 不保存退出
q！ 

## Linux的学习
### 改变权限的命令行
* chgrp

改变文件所属群组 例如：chgrp users install.log(注：改变的组名必须在/etc/group文件内存在)
* chown

改变文件拥有者（可顺便群组的名称 chown root:root install.log） 例如：chown bin install.log

* chmod

改变文件权限(权限设定方法两种)

 符号|分数|
---|:--:|
r|4|
w|2|
x|1|

chomd语法[root@www ~]# chmod [-R] xyz 文件或目录
## 绝对路径和相对路径
 根据档名写法的不同，也可将所谓的路径(path)定义为绝对路径(absolute)与相对路径(relative)
* 绝对路径：由根目录(/)开始写起的文件名或目录名称， 例如 /home/dmtsai/.bashrc；
* 相对路径：相对于目前路径的文件名写法。 例如 ./home/dmtsai 或 ../../home/dmtsai/ 等等。反正开头不是 / 就属于相对路径的写法

## 课后作业
练习mac快捷键

练习命令行

练习预备练习2