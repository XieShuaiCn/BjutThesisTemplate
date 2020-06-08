# BjutThesisTemplate
北京工业大学论文模板（Beijing University of Technology Thesis，bjutthesis），该项目在thuthesis基础上二次开发完成，并整合了学生们已在用的一些设置。

## 安装配置

本项目在TexLive环境中测试通过，MiKTEX等环境请自行尝试。
（注：CTex默认环境不支持。）

1. 下载并安装TeXLive软件。官方网站是[http://tug.org/texlive/](http://tug.org/texlive/ "TeXLive官方网址")，或者在TUNA清华镜像站[下载](https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/Images/ "TUNA TeXLive")。
2. 安装编辑器。你可以使用任何带有文本编辑功能的软件进行论文编写，甚至是记事本。从易用、高效的角度，推荐使用：
   + VSCode + LaTex Workshop插件
   + Sublime Text + LatexTools
   + Atom + 插件
   + TeX Studio
   + Overleaf（在线编辑器）

    以上选项看自己需求和爱好，暂不区分好坏。只要自己用起来顺手任何组合都可以。
3. 将模板下载到某目录中。推荐使用git下载，也可以直接下载zip文件再解压。
4. 编辑论文内容，入口文件main.tex。
5. 编译论文。编译时请使用`xelatex`。一般编译顺序为`xelatex`->`bibtex`->`xelatex`->`xelatex`。一些编辑器可以直接选择或设置编译步骤。

## 目录结构

```
/
├─ref
|  └refs.bib
├─fig                 # 图片目录
|  └ (*.png *.jpg *.eps) 
|─data                # 子页面目录
|  |─ack.tex          # 致谢页
|  ├─chap01.tex       # 第一章，后续章节自行创建
|  ├─conclusion.tex   # 结论
|  ├─cover.tex        # 封面信息
|  ├─notation.tex     # 符号标记，可以不使用
|  └─publications.tex # 研究成果
├─.gitignore          # Git忽略列表，不使用git时可以删除此文件
├─bjut.png            # 校标
├─bjutthesis.bst      # 论文模板文献格式
├─bjutthesis.cfg      # 论文模板配置文件
├─bjutthesis.cls      # 论文模板类文件
├─bjutthesis.sty      # 论文模板包文件
├─cover.docx          # Word版封面
├─main.pdf            # 输出文件
├─main.tex            # Tex入口文件
└─thesis_format(北京工业大学研究生学位论文格式要求新).pdf
                      # 2020年更新
```
