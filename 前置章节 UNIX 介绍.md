## 什么是UNIX？

UNIX是一个二十世纪60年代首次开发的操作系统，从那以后一直在不断完善。通过操作系统，我们指的是一系列能让电脑工作的程序。它是一个应用在服务端，台式电脑和笔记本电脑上的稳定的、多用户、多任务的系统。

UNIX也有和微软一样的用户图形界面，它提供了一个轻松的使用环境。然而，当操作是没有被图形程序覆盖的，或者是没有可用的界面接口，比如说在远程登录的时候，就需要UNIX的知识。

## UNIX的类型

有很多版本的UNIX，虽然它们拥有很多共性。最出名的UNIX系统有：Solaris，GNU/Linux，和MacOS X。

在学校里，我们在自己的服务器和工作站中使用Solaris，而在服务器和电脑上使用Fedora Linux。

## UNIX操作系统

UNIX操作系统由三部分组成：内核、shell（外壳）和程序。

### 内核

内核是操作系统的核心，它给程序分配时间和内存，并且响应系统调用来处理文件存储和通信。

举例说明shell和内核一起工作的方式，加入一个用户输入：rm myfile（这个命令有删除myfile文件的功能）。shell就会在文件存储中搜索包含有rm程序的文件，然后就通过系统调用来请求内核，在myfile文件上执行rm程序。当rm myfile进程执行结束，shell会返回给用户提示符%，从而等待其他命令的输入。

### shell

shell在内核和用户之间扮演着接口的角色。当一个用户登录，登录程序检查用户名和密码，之后打开一个叫做shell的程序。shell是一个命令行解释器，它解释用户输入的命令，并安排他们执行。命令本身就是程序，当命令结束，终端会给用户另一个%提示符（在我们的系统上是%）。

熟练的用户可以定制自己的shell，用户在同一台机器上可以使用不同的shell。职工和学校的学生使用默认的tcsh shell。

tsch shell有一些功能来帮助用户输入命令：

* 文件名称补全 - 输入一部分的命令、文件或是路径名，按下tab键，tcsh shell会自动补全剩下的名称。如果shell发现多个以你已经输入的字母开头的名称，会发出蜂鸣声，提示你再次按下tab键时再多输入几个字母。
* 历史记录 - shell保存着你已经输入的命令清单，如果你需要再次输入某个命令，你可以使用方向键在终端内上下翻看，也可以输入history来查看之前命令的列表。

## 文件和进程

UNIX系统里只有两种东西，文件和进程。

进程是由唯一的PID（进程标识符）标识的执行进程。

文件是数据集合，它们是用户使用文本编辑器、运行编译器等创建的。

文件的例子：

* 一个文档（报告、笔记等）
* 一些高级程序语言写的程序代码
* 一个机器能直接读懂的指令，对普通用户是看不懂的。比如二进制数字（可执行文件或二进制文件）的集合。
* 一个目录，包括它的内容信息，可能是其他目录（子目录）和普通文件的混合。

## 目录结构
所有文件在目录结构里分组放在一起。文件系统被设计成层次结构，像一个倒置的树。文件目录的顶层通常被叫做根目录（用一个斜线来表示）。

![目录结构](http://www.ee.surrey.ac.uk/Teaching/Unix/media/unix-tree.png)

从上面的图片中我们可以看到，本科生的主目录“ee51vn”包含两个子目录（docs和pics目录），和一个叫做report.doc的文件。

report.doc文件的完整目录是：/home/its/ug1/ee51vn/report.doc。

## 打开一个UNIX系统终端
点击应用（Applications）或者附件（Accessories）菜单中的终端（Terminal）标志来打开一个UNIX终端窗口。

![窗口1](http://www.ee.surrey.ac.uk/Teaching/Unix/media/gnome-window.gif)

这样一个UNIX终端窗口就打开了，并且出现了一个%提示符，等待着你输入命令。

![窗口2](http://www.ee.surrey.ac.uk/Teaching/Unix/media/unix-xterm0.gif)













