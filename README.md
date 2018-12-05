# HUST-CS-Report-Template

**本文档禁止一切个人、媒体、网站转载发布，引用请带上本仓库链接**

本仓库为笔者长期使用的华中科技大学计算机科学与技术学院实验报告模板。

众所周知，华中科技大学计算机实验与报告学院一直有着超多的实验以及臭长的格式严格的实验报告，一直是同学们的一个头疼的问题，伴随我们三年。因此，有一个完整的格式规范以及通用的报告模板以便在每次遇到实验报告时直接使用就显得尤为重要，可以极大的减少我们花在报告上的时间同时获得较高的分数。

于是本仓库就是这么来的。

## About

在大二的数据结构实验之后，就想着如何去整合一下各科报告所要求的格式规范来制成这样一个通用模板，于是就参考了一些老师的文档和国家学术论文格式标准，将字体段落等格式整合运用在实验报告中。

在使用该模板后，笔者已取得数据结构实验94，数电实验98，操作系统实验99，数据库课设99，操作系统课设100的成绩，即说明了实验报告不一定非要按照老师给的格式进行修改，只要做到位，老师不会说什么。

现将模板进行了重制，将所有的字体格式规范，段落距离规范，页眉规范，页码规范，图表规范等嵌入文档后制成，现以`GPL v3`协议开源发布，供计算机学院的学弟学妹们参考。

## Usage

* 适用软件：
  * Microsoft Office 2016，Windows上的主要文档工具
  * Wps Office，适用于Linux的解决方案，要注意的是在Linux上，如果没有手动移植过Windows的字体包的话，部分文字可能无法看到，但仍然可以使用格式刷的形式，给新添加的内容刷上文档中固有的格式，在Microsoft Office中打开可以看到修改后的效果。当然Linux用户建议下载Win字体包手动安装字体，即可完整显示所有格式规范。
* 常用工具：
  * 格式刷：用来复制一段文字的格式到另一段文字
  * 标题：共含有`标题`、`标题1`、`标题2`、`标题3`四种格式，对某一行点击即可改变格式，三级标题已包含所有的学校要求的文档格式
  * 插入->页眉/页脚/页码：修改`页眉`，`页脚`，`页码`的工具，其中如何断开页码需要一些操作，这里不提供教程，可以自行搜索，模板中已经将页码重排，从正文开始新的页码。
  * 引用->目录：用来设置你的报告目录的工具，其中`自定义目录工具`可以设置你的目录格式。
  * 文件->选项->保存：这里可以设置`将字体嵌入目录`，适用于文档移植。
  * 文件->选项->校对：这里最下方可以设置`隐藏拼写检查`，消除烦人的红线
  * 文件->选项->高级：把`输入法控制处于活动状态`打钩可以防止有时Office出现中文输入法无法使用的情况。

## Linux字体迁移

对于Linux用户，你可以选择将Win磁盘挂载，并将字体打包复制过来，或者从网上下载Win10的原生字体包，将其放入`WinFonts`文件夹中，并执行以下操作：

```sh
sudo mkdir /usr/share/fonts/WinFonts
sudo cp ./WinFonts/*  /usr/share/fonts/WinFonts
sudo chmod 644 /usr/share/fonts/WinFonts/*
cd /usr/share/fonts/WinFonts
sudo mkfontscale
sudo mkfontdir
sudo fc-cache -fv
```

## 格式规范说明

关于以下部分具体的带图文的说明，可以在模板中看到关于这部分的详细的带图文的说明。

### 标题
* 标题1：宋体 小三 加粗 居中 单倍行距 段前12磅 段后12磅
* 标题2：宋体 四号 加粗 靠左 1.25倍行距 段前6磅 段后0磅
* 标题3：宋体 小四 加粗 靠左 单倍行距 段前3磅 段后8磅
* 正文：宋体 小四 1.25倍行距 段前0磅 段后0磅
* 西文字体统一为Times New Roman字体
* 内部小标题，中文括号，后面不加空格
* 阿拉伯数字标题，加点后加空格，例：1. 我是文字

### 图表

* 图：环绕文字嵌入型，调整至适当大小，图前不空行，图后空一行，图前面的两个空格不能要。
* 图下方文字：宋体 小五 居中，标号从1.1开始按章节标号，标号与图标题之间空一格。
* 表：表居中，表前后各空一行，表头宋体 小五 加粗 居中，表正文宋体 小五。
* 表上方文字：表标题在表上方，宋体 小五 居中，标号方式和图相同。


### 代码段

* 代码段格式说明：段前不空行，段后空一行，代码字体为Times New Roman。
* 方框效果和高亮效果制作：利用网站http://pygments.org/ 进行高亮化处理，复制到Word文档中，将字体改为Times New Roman 小四 黑色。
* 代码段前文字：宋体 小五 居中，标号和图一致。

### 其他格式

* 目录格式：请按照本文档中的目录格式，我已经设置好，直接更新目录即可。
* 页码格式：页码从正文开始计数，不计入目录，我已经设置好，无需修改。

### 参考文献

* A 图书：
[序号]  作者. 书名. 版本(第×版). 译者. 出版地：出版者, 出版年：起页-止页.
* B 期刊：
[序号]  作者. 文章名称. 期刊名称，年号，卷号(期号)：起页-止页.
* C 会议论文集：
[序号]  作者. 文章名称. In(见)：整本文集的编者姓名ed. (多编者用eds.). 文集名. 会址. 开会年. 出版地：出版者,出版年：起页-止页.
* D 专利：
[序号]  专利申请者. 专利题名. 专利国别，专利文献种类，专利号，出版年：起页-止页.
* E 学位论文：
[序号]  作者. 题名：[博士或硕士学位论文]. 保存地点：保存单位(如华中科技大学)，年份.
* F 网页:
[序号]  URL：网络地址

## 关于课程设计

课程设计的报告，无非是在之前加上一个前言写出课题背景与意义，加上一个需求分析来详细说明，在之后加上一个总的感想与心得。测试模块则在倒数第二个统一进行测试。

在格式的控制和标题的控制上，完全适用本文档所提供的格式。无非是对于具体不同的课程设计任务，中间的部分会有一些不同罢了。

当然了，还是要注意封面的修改和页眉的修改。

这里并没有提供课程设计的报告模板（而且我也没有做出来），如果真的需要的话，可以在`issue`里提出意见或者认识我的就QQ私戳我吧。

## Others

我的其他仓库里有着大一以来的所有实验的源代码，当然部分仓库出于知识产权以及防止不劳而获的原因没有公开报告。如果是出于学习为目的的话可以联系我进行索要。

Copyright (C) 2019 zxcpyp