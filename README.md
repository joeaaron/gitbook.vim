# Why use vim?

如果这个世界上有一款编译器用过后，觉得不会再爱上其它的了，我只想说，非VIM莫属。

Ubuntu的Terminal自带透明属性:

> Edit-&gt;Profile Preferences-&gt;Background

当开启透明的那一刻，你编译器的逼格就瞬间超越了市面上很多牛逼的诸如sublime……

OK，我们的目标不在于装，而在于实实在在用来写代码。正因为Vim可以配置，包括配色和插件，才会被很多高手牛人所喜欢，毕竟可以按照自己的风格胡来，谁能拒绝呢。

但是对于初入Vim大家庭的小伙伴，尤其是新手，有个比较省力的方式，也是Z比较推荐的一款扩展——[spf13-vim](https://link.zhihu.com/?target=https%3A//github.com/spf13/spf13-vim)，支持Linux、Mac OS、Windows各个平台，集成了大部分常用的插件比如括号不全、目录树、语法高亮etc，里面也集成了上百种主题，任君挑选，有没有很稀饭？最为关键的是，你只需一行命令，就可以安装。

> $ curl [http://j.mp/spf13-vim3](http://j.mp/spf13-vim3)-L &gt;[spf13-vim.sh](http://spf13-vim.sh/)&& sh[spf13-vim.sh](http://spf13-vim.sh/)

如果不是你的style，可以选择其它主题，不过默认主题我觉得挺好的，唯一缺点是字符串是灰色的，所以开启透明后，肉眼辨识度大打折扣。在此，老夫也倾囊相授：

> $ echo colorscheme peaksea &gt;&gt; ~/.vimrc.local

至此，一款可以写代码的高逼格编译器横空出世。不过，接下来，你可能需要看一下vim的简明教程，推荐看一下简明[VIM 练级攻略](https://coolshell.cn/articles/5426.html)。  
  
若有任何疑问或建议，欢迎提出。







