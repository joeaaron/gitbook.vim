## Vim 设置代码折叠 {#vim-设置代码折叠}

#### 1.有6种方法来选定折叠： {#1有6种方法来选定折叠}

* manual 手工定义折叠
* indent 更多的缩进表示更高级别的折叠
* expr 用表达式来定义折叠
* syntax 用语法高亮来定义折叠
* diff 对没有更改的文本进行折叠
* marker 对文中的标志折叠

#### 2.折叠命令 {#2折叠命令}

* zc 折叠
* zC 对所在范围内所有嵌套的折叠点进行折叠
* zo 展开折叠
* zO 对所在范围内所有嵌套的折叠点展开
* zR 打开所有折叠
* zM 关闭所有折叠
* zE 删除所有的折叠标签

## 了解spf13 {#了解spf13}

#### 1.spf13高亮问题 {#1spf13高亮问题}

在 ~/.vimrc.local 中添加：

> autocmd VimEnter \* set nospell

#### 2.spf13-vim常用插件NERDTree {#2spf13-vim常用插件nerdtree}

![](/assets/3-1.png)

## Vim:3rd level——Better. Stronger. Faster. {#vim3rd-levelbetter-stronger-faster}

#### 1.Better {#1better}

. → \(dot\) will repeat the last command,  
 N → will repeat the command N times

#### 2.Stronger {#2stronger}

NG → Go to line N  
 gg → shortcut for 1G - go to the start of the file  
 G → Go to last line

#### 3.Faster {#3faster}

0 → go to the beginning of this line  
 y → yank from here  
 $ → up to the end of this line

---

**参考文献：**  
 【1】[Vim技巧\#Vim foldmethod代码折叠功能](https://blog.csdn.net/qq_27968607/article/details/60956584)  
 【2】[安装spf13之后，设置nospell和colorcolumns](https://blog.csdn.net/justheretobe/article/details/50708951)  
 【3】[vim终极配置:spf13-vim](https://blog.csdn.net/u011729865/article/details/49210841)  
 【4】[Learn Vim Progressively](http://yannesposito.com/Scratch/en/blog/Learn-Vim-Progressively/)



