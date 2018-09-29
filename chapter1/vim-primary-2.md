## 如何使 Vim 下开发 Python 调试更方便？ {#如何使-vim-下开发-python-调试更方便}

> $ gedit ~/.vimrc.local

添加：

`map <F5> :call CompileRunGcc()<CR>`

`func! CompileRunGcc()`

`exec "w"`

`if &filetype == 'c'`

`exec "!g++ % -o %<"`

`exec "! ./%<"`

`elseif &filetype == 'cpp'`

`exec "!g++ % -o %<"`

`exec "! ./%<"`

`elseif &filetype == 'java'`

`exec "!javac %"`

`exec "!java %<"`

`elseif &filetype == 'python'`

`exec "!time python2.7 %"`

`elseif &filetype == 'sh'`

`:!./%`

`endif`

`endfunc`

## YouCompleteMe {#youcompleteme}

* 和IDE一样，自动补全，
* 根据include的文件进行补全
* 不用再蹩脚的生成tags
* 补全非常精准，而且速度很快，不会有延迟\(以前在大项目上，acp用起来实在是很卡\)
* 支持类似tags的跳转，跳到定义处以及使用处
* 出错提示很智能，并且用起来真的是如丝般柔滑，不用输入:w进行强制检测

## Vim:2nd level——Feel Comfortable {#vim2nd-levelfeel-comfortable}

![](/assets/1.png)

## ![](/assets/2.png) {#vim2nd-levelfeel-comfortable}

---

**参考文献：**

【1】[如何使 Vim 下开发 Python 调试更方便？](https://www.zhihu.com/question/20271508)

【2】[Vim自动补全神器：YouCompleteMe](http://blog.jobbole.com/58978/)

【3】[Learn Vim Progressively](http://yannesposito.com/Scratch/en/blog/Learn-Vim-Progressively/)

