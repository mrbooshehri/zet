# Install latex and pandoc

1. Install the TexLive base
```bash
sudo apt-get install texlive-latex-base
```
Also install the recommended and extra fonts to avoid running into the error [1], when trying to use pdflatex on latex files with more fonts.
```bash
sudo apt-get install texlive-fonts-recommended
sudo apt-get install texlive-fonts-extra
```
2. Install the extra packages,
```bash
sudo apt-get install texlive-latex-extra
```

3. Install pandoc
```bash
sudo apt install pandoc
```

Tags:
```
#latex #pandoc #pdflatex
```

Related:
```
* https://gist.github.com/rain1024/98dd5e2c6c8c28f9ea9d
```
