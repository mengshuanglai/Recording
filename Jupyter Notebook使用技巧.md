## [文章链接](https://mp.weixin.qq.com/s/gkheK5b9mj8sdge0bISFlg)
```
说明：为了实现在jupyter notebook中实现代码编写目录，尝试了很多安装方法，经过多次失败后，终于发现了问题所在，现总结下安装过程  
.1，确定是已经安装好anaconda  
2，要在anaconda prompt模式下

3、pip install jupyter_contrib_nbextensions 

4，配置：jupyter contrib nbextension install --user --skip-running-check

  5，启动jupyter notebook，“Nbextensions”出现在导航栏中，在勾选目录。  
--------------------- 
作者：focusxy 
来源：CSDN 
原文：https://blog.csdn.net/qq_34705900/article/details/80197956 
版权声明：本文为博主原创文章，转载请附上博文链接！
```
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

