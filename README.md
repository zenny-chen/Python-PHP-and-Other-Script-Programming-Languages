# Python, PHP and Other Script Programming Languages
Python、PHP与其他脚本语言

- [Python（2.x）](https://docs.python.org/2/)
- [最新稳定版本的Python 3.x的相关文档](https://docs.python.org/3/)
- [Python调用C/C++的种种方法](https://blog.csdn.net/fxjtoday/article/details/6059874)
- [Format Strings for PyArg_ParseTuple()](http://www.wingware.com/psupport/python-manual/1.5/ext/parseTuple.html)
- [The Py_BuildValue() Function](http://www.wingware.com/psupport/python-manual/1.5/ext/buildValue.html)
- [2018年，10个最好用的Python集成开发环境（IDE）](https://mp.weixin.qq.com/s/AnqgTBNKmtNng7T-0-eRoQ)
- [理解python中yield关键字](https://blog.csdn.net/libbyandhelen/article/details/78957369)
- [将Python代码转为C代码的神奇——Nuitka](http://nuitka.net/doc/user-manual.html)
- [python 中pack和unpack的用法](https://blog.csdn.net/fengjinghuanian/article/details/83994585)
- [python--常用的十进制、16进制、字符串、字节串之间的转换](https://www.cnblogs.com/fqfanqi/p/7900758.html)
- [Python将字节串转为整数](https://blog.csdn.net/wbdxz/article/details/82153550)
- [Python线程创建的两种方法](https://blog.csdn.net/nicholas_dlut/article/details/80800396)
- [Python3之数组（array）](https://cloud.tencent.com/developer/article/1406351)
- [python中base64编码与解码](https://www.cnblogs.com/zanjiahaoge666/p/7242642.html)
- [在Python3里有的变量前面有个\*号，或许你不知道，没关系，看文](https://www.toutiao.com/a6728656306883789316)
- [Python里面这些点，据说80%的新手学习都会一脸懵逼](https://www.toutiao.com/i6754640229165974030/)
- [理解Python的协程(Coroutine)](https://www.jianshu.com/p/84df78d3225a)
- [Python协程深入理解](https://www.cnblogs.com/zhaof/p/7631851.html)
- [python编程_秒懂if \_\_name\_\_ == "\_\_main\_\_"](https://www.toutiao.com/a6753082183482606087/)
- [Python 判断变量是否是 None 的三种写法](https://www.toutiao.com/a6756516715061838343/)
- [拒绝手动下载，python网络爬虫下载图灵数学统计学丛书](https://www.toutiao.com/i6504976182029582861/)
- [PHP中文手册](http://tool.oschina.net/apidocs/apidoc?api=php-zh)
- [利用php调用C语言——使用扩展函数](http://c.biancheng.net/cpp/html/1401.html)
-  [php调用C函数的一种方式——通过执行命令行](https://www.cnblogs.com/freeweb/p/5645699.html)
- [PHP、Javascript 对lambda表达式的支持](https://blog.csdn.net/m0_37968109/article/details/77182593)
- [PHP: 深入pack/unpack 字节序](https://www.cnblogs.com/andydao/p/4200662.html)
- [PHP中pack、unpack的详细用法](https://segmentfault.com/a/1190000008305573)
- [php高级知识：非阻塞模式与PHP多进程](https://www.toutiao.com/a6725332273668817419)
- [php架构之CGI、FastCGI、php-fpm有什么关系？原来这么简单](https://www.toutiao.com/a6765084314993426952/)
- [Lua教程](http://www.runoob.com/lua/lua-tutorial.html)
- [C interop using dart:ffi](https://dart.dev/guides/libraries/c-interop)
- [Flutter 使用阿里巴巴icon库](https://www.toutiao.com/a6809520001628766723/)
- [go runtime 简析](https://www.toutiao.com/a6801023322407567885/)

<br />

### Ubuntu下安装Python的常用工具：

安装基于Python 2.7的pip工具，只需要输入命令行：`sudo apt-get install python-pip`    
安装基于Python 3.x的pip工具，只需要输入命令行：`sudo apt-get install python3-pip`    
对于Python 2.7安装easy_install：`sudo apt-get install python-setuptools`    
对于Python 3.x安装easy_install：`sudo apt-get install python3-setuptools`

安装完pip工具之后，如果要安装numpy等Python库，则可以用：`python -m pip install --user numpy scipy matplotlib ipython jupyter pandas sympy nose`。这里要注意的是，在Windows系统下安装需要使用命令行选项`--user`。

<br />

### Ubuntu下安装tkinter这一Python包

由于Python2.x与Python3.x差异比较大，因此tkinter包也是分了这两个版本。如果我们都要进行安装的话可使用以下命令：
```bash
sudo apt-get install python-tk python3-tk tk-dev
```

在Python2.x下导入使用tkinter见以下代码：
```python
import Tkinter

tk = Tkinter.Tk()
tk.mainloop()
```

这里各位要注意，Tkinter的T是大写的。
在Python3.x下导入使用tkinter见以下代码：
```python
import tkinter

tk = tkinter.Tk()
tk.mainloop()
```

注意，这里的tkinter的t是小写的。

<br />

### 声明当前Python源文件的编码格式为UTF-8编码格式。
由于Python解释器默认会将源文件中的字符编码作为ASCII码进行解释，因此如果我们要将当前源文件作为UTF-8编码的话需要在头一行用注释进行声明，如下所示：
```python
# -*- coding: utf-8 -*-

import sys

print("你好，世界！")
```

这里第一行的注释就告诉解释器将此文件作为UTF-8编码进行解释。如果没有第一行，在执行此Python文件的时候就会这种错误：“SyntaxError: Non-ASCII character '\xe4' in file /Users/zenny-chen/programs/Python/test.py on line 9, but no encoding declared; see http://python.org/dev/peps/pep-0263/ for details”。

