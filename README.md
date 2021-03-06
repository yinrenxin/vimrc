# vim配置

![](./im.png)

## 安装

安装vundle插件  
在家目录下创建.vim/bundle 文件夹  
然后执行如下命令
```
git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
将.vimrc 复制到家目录下  
之后在命令行输入vim  
安装插件使用如下命令
```
:PluginInstall
```

这样插件就会安装完成 所有的插件都在 .vim/bundle/下  
如果打开vim有报错试试这个  
 
```
https://github.com/tpope/vim-pathogen
```
或者将第3行的注释  
之后就能愉快的使用了
## 支持的功能


自动补全，函数跳转，目录树等等  
可简单的替换ide  

## 简单使用


F2 打开关闭目录树  
F3 打开关闭tagbar  

安装Ctags  
在项目根目录输入:  

```
$ ctags -R *
```
生成一个索引文件  
使用Ctrl + ] 和 Ctrl + O 在函数间跳转和跳回  

cscope几个简单的功能  

```
:cs find s 查找函数名、宏、枚举出现的地方
:cs find g 类似上面ctags的功能
:cs find d 查找当前函数调用的函数
:cs find t 查找指定的字符串
:cs find f 查找文件
```


## vim的几个实用技巧

### 编辑
cw 删除当前字母到单词的末尾
0 到行首  
$ 到行尾 
多行编辑使用ctr + v 然后按I 编辑完在按ESC

### 搜索
/ 向下搜索 ？ 向上搜索 取消高亮使用:noh

### 分屏
:sp 上下分  
:vs 左右分  
ctr+w - 或 + 可以调整分屏大小

### 光标移动  

NG -> 到第N行  
gg -> 到第一行  
G -> 到最后一行  
w -> 到下一个单词的开头  
e -> 到下一个单词的结尾  
% -> 匹配括号移动  
`#`  匹配当前单词并高亮显示(所有的) `#` 上一个 `*` 下一个  

ctr+o 后退  
ctr + i 前进  

fx -> 到下一x字母所在的位置  
t, -> 到逗号前的第一个字符，也可以为其他字符  
3fa -> 在当前行查找第三个出现的a  
大写的F，T 效果一样只不过反向的  

