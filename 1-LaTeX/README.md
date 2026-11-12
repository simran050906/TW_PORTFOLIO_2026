# LaTeX Documentation

## 1. Introduction

LaTeX is a document preparation system used to create professional documents such as assignments, reports, research papers and books.

## 2. Features

- Professional document formatting.
- Mathematical equations.
- Automatic numbering.
- Tables and images.
- References and bibliography.

## 3. Basic Structure

```latex
\documentclass{article}

\begin{document}
Hello World!
\end{document}
```

## 4. Document Classes

- `article` – Articles.
- `report` – Reports.
- `book` – Books.
- `letter` – Letters.
- `beamer` – Presentations.

## 5. Packages

Packages provide additional features.

- `graphicx` – Images.
- `amsmath` – Equations.
- `geometry` – Page margins.
- `xcolor` – Colors.
- `fancyhdr` – Headers and footers.

Example:

```latex
\usepackage{graphicx}
\usepackage{amsmath}
```

## 6. Sections and Text Formatting

```latex
\section{Introduction}
\subsection{Features}

\textbf{Bold Text}
\textit{Italic Text}
\underline{Underlined Text}
```

## 7. Lists

**Bulleted List**

```latex
\begin{itemize}
\item C++
\item Python
\end{itemize}
```

**Numbered List**

```latex
\begin{enumerate}
\item First
\item Second
\end{enumerate}
```

## 8. Mathematical Equations

```latex
\[
E = mc^2
\]

\[
\frac{a}{b} + \sqrt{x}
\]
```

## 9. Tables

```latex
\begin{tabular}{|c|c|}
\hline
Name & Marks \\
\hline
Anika & 90 \\
Simran & 95 \\
\hline
\end{tabular}
```

## 10. Images and Figures

The `graphicx` package is used to insert images.

```latex
\includegraphics[width=5cm]{image.png}
```

## 11. Page Formatting

The `geometry` package controls page margins.

```latex
\usepackage[a4paper, margin=1in]{geometry}
```

## 12. Headers and Footers

The `fancyhdr` package customizes page headers and footers.

```latex
\usepackage{fancyhdr}
\pagestyle{fancy}
\lhead{LaTeX}
\rhead{Documentation}
```

## 13. References and Bibliography

LaTeX supports labels, cross-references and bibliographies.

```latex
\label{sec:intro}
\ref{sec:intro}
```

## 14. Indexing

The `makeidx` package creates an alphabetical index.

```latex
\usepackage{makeidx}
\makeindex
```

## 15. Conclusion

LaTeX is a useful tool for creating well-structured academic and technical documents. It simplifies formatting, equations, tables, images and references.