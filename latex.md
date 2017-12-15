# LaTeX Snippets

Some blocks of LaTeX that I find myself looking up a lot. Hopefully having them all in one place is useful for me and anyone else who wants to write things in LaTeX. If any of the LaTeX I am including requires an extra package, I include a `\usepackage{}` above the snippet, if you are going to copy and paste into a document, you need to make sure that you copy the `\usepackage{}` part into the preamble before you have the `\begin{document}`

To make a table:

```
\begin{center}
\begin{tabular}{ c | c | c }
    top & row & here \\ 
    \hline 
    middle & row & here \\
    \hline
    bottom & row & here 
\end{tabular}
\end{center}
```

To show a graphic:




Sample bi-partite graph:




For a template LaTeX document, check out my `homework_template.tex` document in this repository. 
