#LintCode题解
-----------------
##PDF下载
<a href="https://github.com/soulmachine/lintcode/raw/master/C%2B%2B/lintcode-cpp.pdf">LintCode题解(C++版).pdf</a>

<font color="red">**本书即将由电子工业出版社出版，因此这个Repo更新会略落后于纸质版。欢迎大家购买纸质版，支持我持续更新本书。**</font>

C++ 文件夹下是C++版，内容一摸一样，代码是用C++写的，

Java 文件夹下是Java版，目前正在编写中，由于拖延症，不知道猴年马月能完成。

##LaTeX模板
本书使用的是陈硕开源的[模板](https://github.com/chenshuo/typeset)。这个模板制作精良，很有taste，感谢陈硕 :)

##在Windows下编译
1. 安装Tex Live 2013 <http://www.tug.org/texlive/>。把bin目录例如`D:\texlive\2013\bin\win32`加入PATH环境变量。
1. 安装字体。这个LaTex模板总共使用了9个字体，下载地址 <http://pan.baidu.com/s/1gdefYiJ> ，有的字体Windows自带了，有的字体Ubuntu自带了，但都不全，还是一次性安装完所有字体比较方便。
1. 安装TeXstudio <http://texstudio.sourceforge.net/>
1. (可选)启动Tex Live Manager，更新所有已安装的软件包。
1. 配置TeXstudio。

    启动Texstudio，选择 `Options-->Configure Texstudio-->Commands`，XeLaTex 设置为 `xelatex -synctex=1 -interaction=nonstopmode %.tex`；

    选择 `Options-->Configure Texstudio-->Build`

    Build & View 由默认的 PDF Chain 改为 Compile & View；

    Default Compiler 由默认的PdfLaTex 修改为 XeLaTex ；

    PDF Viewer 改为 “Internal PDF Viewer(windowed)”，这样预览时会弹出一个独立的窗口，这样比较方便。

1. 编译。用TeXstudio打开`lintcode-cpp.tex`，点击界面上的绿色箭头就可以开始编译了。

    在下方的窗口可以看到TeXstudio正在使用的编译命令是`xelatex -synctex=1 -interaction=nonstopmode "lintcode-cpp".tex`

##在Ubuntu下编译
1. 安装Tex Live 2013 <http://www.tug.org/texlive/>
	
	1.1. 下载TexLive 2013 的ISO 光盘，地址 <http://www.tug.org/texlive/acquire-iso.html>

    1.2 mount 光盘，`sudo ./install-tl` 开始安装

	1.3 加入环境变量

		sudo vi /etc/profile
		export PATH=$PATH:/usr/local/texlive/2013/bin/x86_64-linux
		export MANPATH=$MANPATH:/usr/local/texlive/2013/texmf-dist/doc/man
		export INFPATH=$INFPATH:/usr/local/texlive/2013/texmf-dist/doc/info

1. 安装字体。这个LaTex模板总共使用了9个字体，下载地址 <http://pan.baidu.com/s/1gdefYiJ> ，有的字体Windows自带了，有的字体Ubuntu自带了，但都不全，还是一次性安装完所有字体比较方便。
1. 安装TeXstudio <http://texstudio.sourceforge.net/>
1. 配置TeXstudio。

    启动Texstudio，选择 `Options-->Configure Texstudio-->Commands`，XeLaTex 设置为 `xelatex -synctex=1 -interaction=nonstopmode %.tex`；

    选择 `Options-->Configure Texstudio-->Build`

    Build & View 由默认的 PDF Chain 改为 Compile & View；

    Default Compiler 由默认的PdfLaTex 修改为 XeLaTex ；

    PDF Viewer 改为 “Internal PDF Viewer(windowed)”，这样预览时会弹出一个独立的窗口，这样比较方便。

1. 编译。用TeXstudio打开`lintcode-cpp.tex`，点击界面上的绿色箭头就可以开始编译了。

    在下方的窗口可以看到TeXstudio正在使用的编译命令是`xelatex -synctex=1 -interaction=nonstopmode "lintcode-cpp".tex`
1. 懒人版镜像。如果不想进行上面繁琐的安装过程，我做好了一个Ubuntu VMware虚拟机镜像，已经装好了TexLive 2013, TexStudio和字体(详细的安装日志见压缩包注释)，开箱即用，下载地址 <http://pan.baidu.com/s/1jGj5uQi>。

##如何贡献代码
编译通过后，就具备了完整的LaTeX编译环境了。

本书模板已经写好了，基本上不需要很多LaTeX知识就可以动手了。

欢迎给本书添加内容或纠正错误，在自己本地编译成PDF，预览没问题后，就可以发pull request过来了。

##北美求职微博群
我和我的小伙伴们在这里：<http://q.weibo.com/1312378>

## 【友情推荐】九章算法

1. 算法辅导在线视频直播课程：<http://www.jiuzhang.com?source=soulmachine>
1. Leetcode在线答案：<http://www.jiuzhang.com/solutions/?source=soulmachine>
1. 新一代刷题网站，比LeetCode题型更多，质量更高 ：<http://www.lintcode.com/?source=soulmachine>


