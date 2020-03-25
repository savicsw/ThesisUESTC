本模板基于wangwen学长最新模板（2020.3.24）进行了修改，主要修改的如下

1.针对论文题目过长的情况（尤其指超过一行的题目），可以自己调整封面上论文题目换行的位置

```bash
\maintitle={这是一个非常长长长长\\长长长的题目}    // <-手动插入\\换行，该字段只影响封面上的论文题目
```


2.针对专硕和学硕论文的不同之处，在采用[promaster]选项编译时，修改“学科专业”->“专业学位类别”，增加了扉页的“工程领域名称”项

```bash
\EngineeringFieldName{测试工程领域名称}{Test Engineering Field Name}
```

3.考虑到专硕扉页和之前有所不同，因此扉页中的相关字段可以直接在main.tex中自定义

```bash
\degree{硕士}     // 申请学位级别
\major{无线电物理}{Radio Physics}    %该字段 学硕对应学科专业   专硕对应专业学位类别
```

4.兼容旧模板的subfigure命令插入子图，subfigure命令被自动替换为新版的subfloat


# ThesisUESTC-电子科技大学毕业论文模板
[![](https://img.shields.io/badge/license-LPPL-blue)](https://www.latex-project.org/lppl/)
[![](https://img.shields.io/github/last-commit/x-magus/ThesisUESTC)](https://github.com/x-magus/ThesisUESTC/zipball/master)
[![](https://img.shields.io/github/issues/x-magus/ThesisUESTC)](https://github.com/x-magus/ThesisUESTC/issues)

此项目提供用于排版电子科技大学毕业论文的LaTeX模板类，旨在帮助电子科技大学的毕业生高效地完成毕业论文的写作。模板提供各种方便的命令，自动化地排版论文的各个部分，使毕业论文轻易地满足学校的格式要求。为了支持更好的字体效果，模板基于XeLaTeX编写，并且放弃对CTeX的依赖，使模板更加稳定。

模板由电子科技大学物理电子学院2014级硕士研究生王稳编写，由于在毕业论文写作中遇到各种问题，希望有一个理想的解决方案，所以决定写一个模板出来。祝愿此项目能继续发展，解决各位同学毕业论文写作中的困难。

*由于GitHub最近访问很不稳定，如果下载链接失效请使用[Gitea分支](https://gitea.com/Xmagus/ThesisUESTC)的[下载链接](https://gitea.com/Xmagus/ThesisUESTC/archive/master.zip)。*

This project provides the LaTeX template for UESTC theses, aims to help the students in UESTC efficiently complete the thesis writing task. The template provides various convenient commands, automatically typesets the portions of the thesis, render it perfectly fits the requirements of the school. To support better font effects, the template is based on XeLaTeX, and gives up the dependence on CTeX, to attain better reliability.

The template is authored by Wang Wen, a 2014 master graduate of UESTC. Because of the problems that occurred in thesis writing, an ideal solution is expected, and a LaTeX template is provided overcoming such difficulties. Wishes to the further development of this project, to spare the students' overheads on this matter.

## 使用方法

### 基本环境
使用模板需要系统安装任意一种TeX环境，如[TeXLive](http://mirror.ctan.org/systems/texlive/Images/)、[MacTeX](https://www.tug.org/mactex/mactex-download.html)和[MiKTeX](https://miktex.org/download)（都自动带有XeLaTeX引擎，但是不推荐CTeX），安装有 SimSun 和 SimHei 字体（其实就是宋体和黑体）以及 Times New Roman 英文字体。在 MacOS 系统下编译会自动识别操作系统，使用 Songti SC 和 STHeiti 字体，但需要启用`--sh
