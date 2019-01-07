# 执行shell命令

Shell是一种与计算机进行文本交互的方式。

一般来讲，当你正在使用Python编译器，需要用到命令行工具的时候，要在shell和IDLE之间进行切换。

但是，如果你用的是Jupyter，就完全不用这么麻烦了，你可以直接在命令之前放一个“!”，就能执行shell命令，完全不用切换来切换去，就能在IPython里执行任何命令行。

1In [1]: !ls
2example.jpeg list tmp
3In [2]: !pwd
4/home/Parul/Desktop/Hello World Folder 
5In [3]: !echo "Hello World"
6Hello World
7
1In [4]: files= !ls
2In [5]: print(files)
3[ example.jpeg ,  list ,  tmp ]
4In [6]: directory = !pwd
5In [7]: print(directory)
6[ /Users/Parul/Desktop/Hello World Folder ]
7In [8]: type(directory)
8IPython.utils.text.SList
