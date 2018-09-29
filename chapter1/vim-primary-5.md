## 一、VIM 操作 {#一vim-操作}

#### 1.自动给新建的文件添加头部注释 {#1自动给新建的文件添加头部注释}

将下面的代码复制到_~/.vimrc.local_文件中：

**autocmd BufNewFile \*.c,\*.cpp,\*.sh,\*.py,\*.java exec ":call SetTitle\(\)"                                                                                       **

"定义函数SetTitle，自动插入文件头

`func SetTitle()`

`        "如果文件类型为.c或者.cpp文件`

`        if (&filetype == 'c' || &filetype == 'cpp')`

`                call setline(1, "/*************************************************************************")  `

`                call setline(2, "\ @Author: 你的名字")  `

`                call setline(3, "\ @Created Time : ".strftime("%c"))  `

`                call setline(4, "\ @File Name: ".expand("%"))  `

`                call setline(5, "\ @Description:")  `

`                call setline(6, " ************************************************************************/")  `

`                call setline(7,"")  `

`        endif`

`        "如果文件类型为.sh文件`

`        if &filetype == 'shell'  `

`                call setline(1, "\#!/bin/sh")`

`                call setline(2, "\# Author: 你的名字")`

`                call setline(3, "\# Created Time : ".strftime("%c"))`

`                call setline(4, "\# File Name: ".expand("%"))`

`                call setline(5, "\# Description:")`

`                call setline(6,"")`

`        endif`

`        "如果文件类型为.py文件`

`        if &filetype == 'python'`

`                call setline(1, "\#!/usr/bin/env python")`

`                call setline(2, "\# -*- coding=utf8 -*-")`

`                call setline(3, "\"\"\"")`

`                call setline(4, "\# Author: 你的名字")`

`                call setline(5, "\# Created Time : ".strftime("%c"))`

`                call setline(6, "\# File Name: ".expand("%"))`

`                call setline(7, "\# Description:")`

`                call setline(8, "\"\"\"")`

`                call setline(9,"")`

`        endif`

`        "如果文件类型为.java文件`

`        if &filetype == 'java'  `

`                call setline(1, "//coding=utf8")  `

`                call setline(2, "/**")  `

`                call setline(3, "\ *\ @Author: 你的名字")  `

`                call setline(4, "\ *\ @Created Time : ".strftime("%c"))  `

`                call setline(5, "\ *\ @File Name: ".expand("%"))  `

`                call setline(6, "\ *\ @Description:")  `

`                call setline(7, "\ */")  `

`                call setline(8,"")  `

`        endif`

`endfunc`

#### 2.快速切换头（.h）/源（.c，.cpp，.cc）文件 {#2快速切换头h源ccppcc文件}

1. 在~/.vimrc.bundles.local文件中添加：

   Bundle ‘a.vim’

2. 进入vim，  
    ：BundleInstall

## 二、spf13 {#二spf13}

#### spf13-vim常用插件ctags {#spf13-vim常用插件ctags}

将下面的代码复制到_~/.vimrc.local_文件中:

![](/assets/5-1.png)

快捷键映射：

![](/assets/5-2.png)

在源码根目录中输入ctags -R命令。

重启vim，打开src文件，就能使用F3或 F4 来实现跳转了

![](/assets/5-3.png)  


---

**参考文献：**  
 【1】[vi技巧之自动给新建的文件添加头部注释](https://blog.csdn.net/daoshuti/article/details/66970506)

【2】[vim 自动添加头注释](https://blog.csdn.net/qq844352155/article/details/50513072)

【3】[vim插件之快速切换头（.h）/源（.c，.cpp，.cc）文件——a.vim](https://blog.csdn.net/zhangsming/article/details/42652695)

【4】[使用Ctags在Vim跳转到定义](https://blog.csdn.net/xiana_yz/article/details/40516243)

【5】[个人渣翻译 spf13插件—Tagbar（ctags） 使用教程](https://blog.csdn.net/dark_tone/article/details/52940939)

【6】[使用map自定义快捷键](https://www.jianshu.com/p/8ae25a680ed7)



