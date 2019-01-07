## [文章链接](https://mp.weixin.qq.com/s/gkheK5b9mj8sdge0bISFlg)
conda install -c conda-forge jupyter_nbextensions_configurator
## 执行shell命令

Shell是一种与计算机进行文本交互的方式。

一般来讲，当你正在使用Python编译器，需要用到命令行工具的时候，要在shell和IDLE之间进行切换。

但是，如果你用的是Jupyter，就完全不用这么麻烦了，你可以直接在命令之前放一个“!”，就能执行shell命令，完全不用切换来切换去，就能在IPython里执行任何命令行。

```
In [1]: !ls
example.jpeg list tmp
In [2]: !pwd
/home/Parul/Desktop/Hello World Folder 
In [3]: !echo "Hello World"
Hello World
In [4]: files= !ls
In [5]: print(files)
[ example.jpeg ,  list ,  tmp ]
In [6]: directory = !pwd
In [7]: print(directory)
[ /Users/Parul/Desktop/Hello World Folder ]
In [8]: type(directory)
IPython.utils.text.SList
```

