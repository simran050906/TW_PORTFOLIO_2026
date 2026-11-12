# LaTeX Documentation

## 1. Introduction to LaTeX

LaTeX is a document preparation system based on the TeX typesetting system. It is used to create professional and well-structured documents such as assignments, research papers, books, reports and technical documents.

It uses commands to control the structure and formatting of a document.

## 2. Why LaTeX?

Some important advantages of LaTeX are:

- It is free and portable.
- It produces professional-quality documents.
- It provides excellent support for mathematical equations.
- It supports tables, figures, references and bibliographies.
- It automatically manages numbering and document structure.
- It is useful for preparing large and complex documents.

## 3. LaTeX Tools

LaTeX can be used through different offline and online tools.

**Offline tools:**
- MiKTeX
- TeX Live
- TeXstudio
- TeXnicCenter

**Online tools:**
- Overleaf
- Papeeria
- CoCalc

I use TeXstudio for writing and compiling LaTeX documents.

## 4. Input File and Output Format

A LaTeX source file is a plain text file saved with the `.tex` extension. It contains the document content and LaTeX commands.

Common output formats include:
- PDF (.pdf)
- DVI (.dvi)
- PostScript (.ps)
- RTF (.rtf)

## 5. Compiling a LaTeX Document

Compilation is the process of converting LaTeX source code into a readable document.

The following command is used to generate a PDF:

```latex
pdflatex filename.tex
```

TeXstudio also provides a Build and View option to compile and view the PDF.

## 6. Basic Structure of a LaTeX Document

Every basic LaTeX document contains a document class, preamble and document environment.

Example:

```latex
\documentclass{article}

\begin{document}

Hello World!

\end{document}
```

- `\documentclass{}` specifies the type of document.
- `\begin{document}` starts the document body.
- `\end{document}` ends the document.

## 7. Document Classes

The document class determines the overall structure and layout of a document.

Common document classes are:

| Class | Purpose |
|---|---|
| article | Articles and short documents |
| report | Reports and longer documents |
| book | Books and dissertations |
| letter | Formal letters |
| beamer | Presentations |
| exam | Exams and question papers |

Example:

```latex
\documentclass[12pt,a4paper]{article}
```

Here, `12pt` specifies the font size and `a4paper` specifies the paper size.

## 8. Document and Page Styles

Document style controls the overall structure, while page style controls headers and footers.

Common page styles:

- `plain` – Displays the page number at the bottom.
- `headings` – Displays section or chapter headings.
- `empty` – Removes headers and footers.

Example:

```latex
\pagestyle{plain}
```

## 9. Creating a Title Page and Abstract

The title page contains the document title, author name and date.

Example:

```latex
\title{Introduction to LaTeX}
\author{Your Name}
\date{\today}

\begin{document}

\maketitle

\begin{abstract}
This document introduces LaTeX.
\end{abstract}

\end{document}
```

The `\maketitle` command displays the title information, while the abstract environment provides a short summary of the document.

## 10. Text Formatting

LaTeX provides different commands to change the appearance of text.

| Command | Purpose |
|---|---|
| `\textbf{}` | Bold text |
| `\textit{}` | Italic text |
| `\underline{}` | Underlined text |
| `\emph{}` | Emphasized text |
| `\texttt{}` | Monospaced text |
| `\textsf{}` | Sans-serif text |

### Font Sizes

Common font size commands include:

- `\tiny`
- `\scriptsize`
- `\footnotesize`
- `\small`
- `\normalsize`
- `\large`
- `\Large`
- `\LARGE`
- `\huge`
- `\Huge`

## 11. Text Alignment

LaTeX provides three environments for text alignment.

```latex
\begin{flushleft}
Left aligned text
\end{flushleft}

\begin{center}
Centered text
\end{center}

\begin{flushright}
Right aligned text
\end{flushright}
```

## 12. Lists in LaTeX

LaTeX supports three commonly used list environments.

**Unordered List:**

```latex
\begin{itemize}
\item Apple
\item Mango
\item Orange
\end{itemize}
```

**Ordered List:**

```latex
\begin{enumerate}
\item First
\item Second
\item Third
\end{enumerate}
```

**Description List:**

```latex
\begin{description}
\item[CPU] Processor
\item[RAM] Memory
\end{description}
```

## 13. Mathematical Equations

LaTeX provides excellent support for writing mathematical expressions.

### Inline Equation

```latex
The area of a circle is $A=\pi r^2$.
```

### Display Equation

```latex
\[
E=mc^2
\]
```

### Common Mathematical Symbols

| Expression | LaTeX Command |
|---|---|
| Fraction | `\frac{a}{b}` |
| Square root | `\sqrt{x}` |
| Summation | `\sum` |
| Integration | `\int` |
| Alpha | `\alpha` |
| Beta | `\beta` |
| Infinity | `\infty` |
| Less than or equal | `\leq` |
| Not equal | `\neq` |

## 14. Mathematical Display Styles and Matrices

LaTeX supports different mathematical environments for displaying matrices and expressions.

Common matrix environments include:

- `matrix` – Matrix without brackets.
- `pmatrix` – Matrix with round brackets.
- `bmatrix` – Matrix with square brackets.
- `Bmatrix` – Matrix with curly brackets.
- `vmatrix` – Matrix with single vertical bars.
- `Vmatrix` – Matrix with double vertical bars.
- `smallmatrix` – Compact matrix for inline expressions.

Example:

```latex
\[
A =
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
\]
```

## 15. Tables in LaTeX

Tables are created using the `tabular` environment.

Column alignment options:
- `l` – Left alignment.
- `c` – Center alignment.
- `r` – Right alignment.

Example:

```latex
\begin{tabular}{|c|c|}
\hline
Name & Marks \\
\hline
Alice & 90 \\
Bob & 85 \\
\hline
\end{tabular}
```

## 16. Figures and Images

Images can be inserted using the `graphicx` package.

```latex
\usepackage{graphicx}
```

Example:

```latex
\begin{figure}[h]
\centering
\includegraphics[width=0.5\textwidth]{image.png}
\caption{Sample Figure}
\label{fig:sample}
\end{figure}
```

The `\caption` command adds a caption, and `\label` assigns a reference name to the figure.

## 17. Colours in LaTeX

The `xcolor` package is used to add colours to text and documents.

```latex
\usepackage{xcolor}
```

Examples:

```latex
\textcolor{red}{Red Text}

\colorbox{yellow}{Highlighted Text}

\pagecolor{yellow!10}
```

Custom colours can also be created using `\definecolor`.

## 18. Document Formatting and Page Layout

LaTeX provides commands and packages to customize page layout.

### Changing Page Margins

The `geometry` package is used to set page margins.

```latex
\usepackage{geometry}
\geometry{left=2.5cm,right=2.5cm,top=2.5cm,bottom=2.5cm}
```

### Headers and Footers

The `fancyhdr` package provides control over headers and footers.

```latex
\usepackage{fancyhdr}
\pagestyle{fancy}

\fancyhf{}
\fancyhead[L]{My Document}
\fancyhead[R]{\today}
\fancyfoot[C]{\thepage}
```

### Section Formatting

The `sectsty` package can be used to customize section heading styles.

### Custom Fonts

The `fontspec` package allows the use of system fonts and requires XeLaTeX or LuaLaTeX.

### Customizing Lists

The `enumitem` package provides options to customize bullet styles and list spacing.

## 19. Line Breaks and Paragraph Spacing

LaTeX provides commands to control line and paragraph spacing.

- `\\` – Creates a manual line break.
- A blank line – Starts a new paragraph.
- `\par` – Ends a paragraph.
- `\vspace{}` – Adds vertical space.
- `\hspace{}` – Adds horizontal space.
- `\noindent` – Removes paragraph indentation.

## 20. Page Breaks

Page breaks can be controlled using different commands.

- `\newpage` – Starts a new page.
- `\pagebreak` – Suggests or forces a page break.
- `\clearpage` – Starts a new page after placing pending figures and tables.

The `samepage` environment can be used to keep related paragraphs together.

## 21. Section and Subsection Numbering

Sections help organize a document into meaningful parts.

```latex
\section{Introduction}

\subsection{Background}

\subsubsection{Overview}
```

LaTeX automatically numbers sections and subsections.

## 22. Cross References

Cross-referencing allows us to refer to sections, figures, tables and equations automatically.

Important commands:

- `\label{}` – Defines a reference label.
- `\ref{}` – Displays the number of the referenced item.
- `\pageref{}` – Displays its page number.

Example:

```latex
\section{Introduction}
\label{sec:intro}

See Section~\ref{sec:intro}.
```

## 23. Bibliography and Citations

A bibliography contains the references used in a document.

The `thebibliography` environment can be used to add references manually.

BibTeX is another tool used to manage references through a separate `.bib` file.

Important commands:

```latex
\bibliographystyle{plain}
\bibliography{refs}
```

A citation can be inserted using:

```latex
\cite{reference_key}
```

Common BibTeX entry types include:

- `@article`
- `@book`
- `@inproceedings`
- `@techreport`
- `@misc`

## 24. Creating an Index Using MakeIndex

An index provides an alphabetical list of important terms along with their page numbers.

The `makeidx` package is used to create an index.

Example:

```latex
\usepackage{makeidx}
\makeindex
```

Inside the document:

```latex
\index{LaTeX}
\printindex
```

The document is compiled using LaTeX, MakeIndex and LaTeX again to generate the index.

## 25. Common LaTeX Errors and Warnings

Some common errors and warnings include:

- Missing braces or closing environments.
- Undefined commands.
- Missing packages.
- TeX capacity exceeded.
- Overfull `\hbox`.
- Underfull `\vbox`.

### Basic Troubleshooting

1. Check the error location in the log.
2. Check whether all environments are properly closed.
3. Verify spelling of commands.
4. Check whether required packages are included.
5. Compile the document again after correcting errors.

## 26. Applications of LaTeX

LaTeX is commonly used for:

- Academic assignments and reports.
- Research papers and publications.
- Mathematical and scientific documents.
- Books and dissertations.
- Technical documentation.
- Professional presentations.

## 27. Conclusion

LaTeX is a powerful document preparation system that helps create well-structured and professional documents. Through this topic, I learned about document structure, formatting, mathematical equations, tables, figures, references, page layouts and bibliography management.

It is especially useful for academic and technical writing.