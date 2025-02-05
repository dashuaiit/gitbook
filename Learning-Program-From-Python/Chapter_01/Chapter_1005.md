# 附录A Python的安装与运行

### 1．官方版本安装 {#官方版本安装 .kindle-cn-heading2}

#### 1）Mac

Mac系统上已经预装了Python，可以直接使用。如果想要使用其他版本的Python，建议使用Homebrew安装[^(9)^](part0005.xhtml#ch9){#ch9-back}。打开终端（Terminal），在命令行提示符后输入下面命令后，将进入Python的可以互动的命令行：

------------------------------------------------------------------------

    $python

------------------------------------------------------------------------

上面输入的python通常是一个软链接，指向某个版本的Python命令，如3.5版本。如果相应版本已经安装，那么可以用下面的方式来运行：

------------------------------------------------------------------------

    $python3.5

------------------------------------------------------------------------

终端会出现Python的相关信息，如Python的版本号，然后就会出现Python的命令行提示符``>>>``。如果想要退出Python，则输入：

------------------------------------------------------------------------

    >>>exit()

------------------------------------------------------------------------

如果想要运行当前目录下的某个Python程序文件，那么在python或python3后面加上文件的名字：

------------------------------------------------------------------------

    $python hello.py

------------------------------------------------------------------------

如果文件不在当前目录下，那么需要说明文件的完整路径，如

------------------------------------------------------------------------

    $python /home/vamei/hello.py

------------------------------------------------------------------------

我们还可以把Python程序hello.py改成一个可执行的脚本。只需在hello.py的第一行加上所要使用的Python解释器：

------------------------------------------------------------------------

    #!/usr/bin/env python

------------------------------------------------------------------------

在终端中，把hello.py的权限改为可执行：

------------------------------------------------------------------------

    $chmod 755 hello.py

------------------------------------------------------------------------

然后在命令行中，输入程序文件的名字，就可以直接使用规定的解释器运行了：

------------------------------------------------------------------------

    $./hello.py

------------------------------------------------------------------------

如果hello.py在默认路径下，那么系统就可以自动搜索到这个可执行文件，就可以在任何路径下运行这个文件了：

------------------------------------------------------------------------

    $hello.py

------------------------------------------------------------------------

#### 2）Linux操作系统

Linux系统与Mac系统比较类似，大多也预装了Python。很多Linux系统下都提供了类似于Homebrew的软件管理器，例如在Ubuntu下使用下面命令安装：

------------------------------------------------------------------------

    $sudo apt-get install python

------------------------------------------------------------------------

在Linux下，Python的使用和运行方式也和Mac系统下类似，这里不再赘述。

#### 3）Windows操作系统

对于Windows操作系统来说，需要到Python的官方网站[^(10)^](part0005.xhtml#ch10){#ch10-back}下载安装包。如果无法访问Python的官网，那么可以通过搜索引擎查找“python Windows下载”这样的关键字，来寻找其他的下载源。安装过程与安装其他Windows软件类似。在安装界面中，选择Customize来个性化安装，除了选择Python的各个组件外，还要勾选：

------------------------------------------------------------------------

    Add python.exe to Path

------------------------------------------------------------------------

安装好之后，就可以打开Windows的命令行，像在Mac中一样使用Python了。

### 2．其他Python版本 {#其他python版本 .kindle-cn-heading2}

官方版本的Python主要提供了编译/解释器功能。其他一些非官方版本则有更加丰富的功能和界面，比如更加友好的图形化界面、一个针对Python的文本编辑器，或者是一个更容易使用的模块管理系统，方便你找到各种拓展模块等。在非官方的Python中，最常用的有下面两个：

  1. Anaconda[^(11)^](part0005.xhtml#ch11){#ch11-back}
  2. Enthought Python Distribution（EPD）[^(12)^](part0005.xhtml#ch12){#ch12-back}

相对于官方版本的Python来说，这两个版本都更容易安装和使用。在模块管理系统的帮助下，程序员还可以避免模块安装方面的恼人问题。所以非常推荐初学者使用。Anaconda是免费的，EPD则对于学生和科研人员免费。由于提供了图形化界面，因此它们的使用方法也相当直观。我强烈建议初学者从这两个版本中挑选一个使用。具体用法可以参考官方文档，这里不再赘述。
