---
layout: post
title: "My Makefile Workflow"
subtitle: 'From Cstudio to makefile'
author: "Hji"
header-style: text
tags:
  - Makefile
---

隐含规则：
%.c %.o :任意的.c文件和任意的.o文件
*.c *.o :所有的.c文件和所有的.o文件

.c ----> .i ----> .s ----> .o ----> bin



make工作方式
GUN的make工作时，执行如下步骤：
1. 读入所有的Makefile
2. 读入被include的其它Makefile
3. 初始化文件中的变量
4. 推导隐晦规则，并分析所有规则
5. 为所有的目标文件创建依赖关系链
6. 根据依赖关系，决定哪些目标要重新生成
7. 执行生成命令

Make 的“拖延”执行方式

伪目标.PHONY的作用
在当前makefile目录下建立文件clean ，如果makefile中的clean没有声明为伪目标，则使用make clean命令后，clean：下的所有指令将不会被执行，反而clean文件会被更新（依据makefile中clean：下的具体操作指令）。
Master Makefile
```make
target...:prerequisites...
   command
 ```
目标:依赖
   操作系统指令
说明:在定义好依赖关系后，后续的那一行定义了如何生成目标文件的操作系统命令，一定要以一个Tab键作为开头。记住，make并不管命令是怎么工作的，他只管执行所定义的命令。make会比较targets文件和prerequisites文件的修改日期，如果prerequisites文件的日期要比targets文件的日期要新，或者target不存在的话，那么，make就会执行后续定义的命令。

理解文件和文件夹也是可以是"目标"。那么，没有依赖文件(目标)也可以执行对应的命令。如果文件或者文件夹（目标）已经存在，则不执行对应的命令，如果不存在，则转移到依赖项的位置执行。

执行make后的编译和文件操作过程要求Makefile中的命令指令以target：target1，target1：target2 … 形成依赖链。
"clean:"必须放在all（假设all为头部伪目标）后面，如果放在首位。make后将直接执行clean后的命令，如果要执行all编译链，需要make all；相反，一般的情况是，make 默认执行前部的all编译链，make clean执行clean目标下的编译链。
命令前加“-”，表示忽略命令执行过程的错误。

为目标（文件）添加依赖关系，当依赖文件更改后，目标将可以通过make重新执行。并依次执行依赖链的命令。

通常，make会把其要执行的命令行的命令在执行前输出到屏幕上，当我们用@字符加在命令行前，这个命令不会被make显示出来。
例如：echo xxxx，执行时候显示：
echo xxxx
xxxx
@echo xxxx 执行时显示：
Xxxx

参考文献：
 《跟我一起写makefile》《驾驭makefile》


### Vim-binding



```vim
command! -nargs=* D  belowright split | terminal <args>
```
















