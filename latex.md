# LaTeX Snippets

Some blocks of LaTeX that I find myself looking up a lot. Hopefully having them all in one place is useful for me and anyone else who wants to write things in LaTeX. If any of the LaTeX I am including requires an extra package, I include a `\usepackage{}` above the snippet, if you are going to copy and paste into a document, you need to make sure that you copy the `\usepackage{}` part into the preamble before you have the `\begin{document}`

**To make a table:**

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

**To show a graphic:**

For this, make sure you have the file you want to show in the same directory as the .tex file or that you write the correct path to the file in the brackets where I have `fig.png`. You can also change the scale of the picture if it is too large or small and you don't want to deal with cropping it in a different way.  

```
\usepackage{graphicx}
\usepackage{float}
```

```
\begin{figure}[H]
    \centering
    \includegraphics[scale=0.5]{fig.png}
    \caption{Your caption here}
    \centering
\end{figure}
```

**QED sign for the end of proofs:**

This one is a little more complicated. We add a new command via the following line 

```
\newcommand*{\QED}{\hfill\ensuremath{\blacksquare}}
```

And to use it simply write `\QED`

**Sample bi-partite graph:**




For a template LaTeX document with all of the packages you need to make everything above, see my `homework_template.tex` document in this repository. 
