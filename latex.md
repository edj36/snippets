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

Add a new command and corresponding package via the following line, make sure these lines are both above `\begin{document}` 

```
\usepackage{amssymb}
\newcommand*{\QED}{\hfill\ensuremath{\blacksquare}}
```

And to use it simply write `\QED`

**Make a matrix**

```
\usepackage{amsmath}
```

```
\[
\begin{pmatrix}
    1 & 0 \\
    0 & 1
\end{pmatrix}
\]
```

**Align Equations**

```
\usepackage{amsmath}
```

```
\begin{align*}
e^{i\pi}+1 &= -1+1 \\
           &= 0
\end{align*}
```

**Header on each page**

Include all of the following before `\begin{document}`

```
\usepackage{fancyhdr}
\pagestyle{fancy}
\lhead{Left header}
\rhead{Right header}
\renewcommand{\headrulewidth}{1pt}
```

If you don't want a line across the top, you can change the `1pt` to `0pt`. If you delete the `\renewcommand` line there will still be a line across the top, it's the default. 

**Include code from another file**

For when you need to include source code (an entire separate file, not a code snippet) you wrote for something you are writing about. This is easiest as long as you have the file of code in the same location as your .tex document. 

```
\usepackage{listings}
```

```
\lstinputlisting{helloworld.py}
```

For a template LaTeX document with all of the packages you need to make everything above, see my `homework_template.tex` document in this repository. 
