# BjutThesisTemplate
The Latex template project of Beijing University of Technology Thesis(bjutthesis), which is inherited from thuthesis and merge some setings of students in use.

## Installation

This project passed the test in the TexLive environment, and tried its own effect in other enviroments.

(PS: As far as we know, The CTeX default enviroment does not support this project.)

1. Download and install TeXLive software. The Offical website is [http://tug.org/texlive/](http://tug.org/texlive/ "TeXLive website"), and you can also find it in [TUNA](https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/Images/ "TUNA TeXLive").
2. Install the editor. You can use any software with text editing function for thesis writing, even Notepad.In terms of ease of use and efficiency, we recommend the following:
   + VSCode + LaTex Workshop plugin
   + Sublime Text + LatexTools
   + Atom + plugins
   + TeX Studio
   + Overleaf (online editor)

    The above options are based on your own needs and hobbies, and do not distinguish good from bad. Any combination can be used as long as you can.
3. Download the template into your directory. It is recommended to download it with git, otherwise you can download the zip file directly and extract it.
4. Edit paper content, entry file `main.tex`.
5. Compile the paper. `xelatex` is used at compile time. The general compilation order is `xelatex`->`bibtex`->`xelatex`->`xelatex`.

## Directory Structure

```
/
├─ref
|  └refs.bib
├─fig                 # figure data
|  └ (*.png *.jpg *.eps) 
|─data                # Subpages
|  |─ack.tex          # Acknowledgements
|  ├─chap01.tex       # The 1st chapter, subsequent chapters are created by yourself.
|  ├─conclusion.tex   # Conclusions
|  ├─cover.tex        # Your information on cover.
|  ├─notation.tex     # Symbol mark, you can either use it or not.
|  └─publications.tex # Research works
├─.gitignore          # Git ignore file, delete it if without git.
├─bjut.png            # School logo
├─bjutthesis.bst      # Template reference format
├─bjutthesis.cfg      # Template configure
├─bjutthesis.cls      # Template class
├─bjutthesis.sty      # Template package
├─cover.docx          # Cover in MS Word
├─main.pdf            # Output file
├─main.tex            # Tex entry file
└─thesis_format(北京工业大学研究生学位论文格式要求新).pdf
                      # Updated in 2020.
```
