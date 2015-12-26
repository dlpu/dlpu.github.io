---
layout: post
title: Vim常用插件
---
最近觉得在小部分修改代码的时候应该抛弃大型的IDE而转向Vim，下面的图就是我的环境了。

![](/image/QQ20141213-3.png)

关于Mac上vim的版本更新，我建议使用Macvim，然后alias命令

```vim
alias vi=vim
alias vim=/Applications/MacVim.app/Contents/MacOS/Vim 
```

[在这里](https://github.com/tcitry/my-tools/blob/master/vimrc)是我的.vimrc的配置。

## 常用插件推荐

[vundle](https://github.com/gmarik/Vundle.vim)是一个用来部署其他插件的插件，用来更方便的管理其他插件的更新和删除。在.vimrc中如上图编辑vundle部分，保存后在vi中执行`:BundleInstall`就能自动安装其他插件

```bash
:PluginList       - 枚举已安装的插件列表
:PluginInstall    - 安装插件或者后面加上'!'更新
:PluginUpdate     - 更新插件 同 :PluginInstall!
:PluginSearch foo - 查找插件。例如查找名称为foo的插件。或者后面加'!'更新本地缓存
:PluginClean      - 清理无用插件或者后面加'!'自动清理
```

[surround](https://github.com/tpope/vim-surround)用来编辑“hello world”，(button)，这样成对符号格式的字符串，

[airline](https://github.com/bling/vim-airline)是状态栏增强插件，根据上面的示例图可以看到。

[autoclose](https://github.com/vim-scripts/AutoClose)用来输出(),"",{}这样的字符，当我打出左半个，自动输出右半个，人性化的是，当两个符号中间没有其他字符删除左半个右半个也一起删除。

[Pydiction](https://github.com/rkulla/pydiction)这个插件的python语法自动补全绝对是能替代IDE的理由，十分强悍。

[NERDtree](https://github.com/scrooloose/nerdtree)是一个文件管理器插件。这个插件还有个加强版在[这里](https://github.com/jistr/vim-nerdtree-tabs)。从最上面的图里面可以看到左侧的效果。

[syntastic](https://github.com/scrooloose/syntastic)用来检查语法错误

[vim-go](https://github.com/fatih/vim-go)用来使go语言高亮，而且建议安装vim-go插件后运行`:GoInstallBinaries`可以批量安装go内置的几个vim插件。

[Matrix](https://github.com/vim-scripts/matrix.vim--Yang)绝对是vim插件里最装X的一个，没有之一。

![](/image/matrix1.gif)

[gist-vim](https://github.com/mattn/gist-vim)可以向自己的github-gist上传代码

[xml](https://github.com/othree/xml.vim)可以匹配<></>这样的字符成对输出