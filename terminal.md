# Terminal Snippets

Some useful commands I tend to have to google when using the terminal. My main machine is a Mac, so these commands should work on Unix/Linux systems in general but I haven't tested them at all outside of my local environment. For some commands, you may need to have certain tools (e.g. Pandoc) installed. 

**Move (or rename a file):**
```
mv <path/to/old.txt> <path/to/new.txt>
```

**Pandoc**

Markdown to standalone HTML (.txt could also be .md)
```
pandoc -s MANUAL.txt -o example2.html
```

**Jupyter notebook to .tex file**
```
jupyter nbconvert --to latex notebook.ipynb
```

**Compile LaTeX**
```
pdflatex file.tex
```
