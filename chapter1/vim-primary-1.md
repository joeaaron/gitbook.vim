## Vim的四种模式 {#vim的四种模式}

正常模式 \(Normal-mode\)  
 插入模式 \(Insert-mode\)  
 命令模式 \(Command-mode\)  
 可视模式 \(Visual-mode\)

## 了解spf13 {#了解spf13}

懒人集合包spf13做了些什么工作，怎么使用它呢？

我们访问spf13官网，查询需要的信息，原来它把一些经典的vim插件给自动安装了。

同时又给与用户最大的灵活性，可以自己增减插件，以及配置快捷键映射。  
 Monday, 06. August 2018 11:13PM

> ~/.vimrc.local \#个性化配置文件  
>  ~/.vimrc.bundles.local \#本地bundle配置文件  
>  ~/.vimrc.before.local \#早于spf13-vim加载的个性化配置文件

## Vim:多标签切换\|窗口拆分 {#vim多标签切换窗口拆分}

vim 从 vim7 开始加入了多标签切换的功能， 相当于多窗口.  
 之前的版本虽然也有多文件编辑功能， 但是总之不如这个方便啦。  
 用法  
 :tabnew \[++opt选项\] ［＋cmd］ 文件 建立对指定文件新的tab  
 :tabc 关闭当前的tab  
 :tabo 关闭所有其他的tab  
 :tabs 查看所有打开的tab  
 :tabp 前一个  
 :tabn 后一个  
 :tabfirst 移动到第一个标签页  
 :tablast 移动到最后一个标签页  
 标准模式下：

gt , gT 可以直接在tab之间切换。  
 还有很多他命令， 看官大人自己， :help table 吧。

---

**参考文献：**  
 【1】[vim的四种模式及模式切换](https://blog.csdn.net/zhangzeyuaaa/article/details/53404808)  
 【2】 [spf13-vim安装与使用](https://www.cnblogs.com/274914765qq/archive/2015/11/03/4934503.html)  
 【3】 [vim多标签和多窗口](https://blog.csdn.net/shuitawuhen/article/details/50263003)



