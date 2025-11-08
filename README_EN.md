# Jiangsu University Beamer Template

English | [简体中文](README.md)

This is a Beamer presentation template I created for the mid-term project defense of the "Embedded Application Development" course in the first semester of my sophomore year. It is modified based on the [Nanjing University Software Institute Beamer Template](https://github.com/EagleBear2002/NJUSE-Beamer-Template). There are many areas that need improvement, especially the color scheme which hasn't been well-adjusted yet, resulting in average visual appearance. Contributions and improvements are warmly welcome!

A LaTeX Beamer template for Jiangsu University academic presentations, suitable for course defenses, academic reports, project demonstrations, etc.

## Features

- Jiangsu University official visual identity system
- Clear top navigation bar (with university name logo and emblem)
- Green theme color (Jiangsu University standard color)
- Support for Chinese and English mixed typesetting
- 16:9 widescreen aspect ratio
- Clean and elegant page layout

## Directory Structure

```
.
├── jsu.sty                          # Jiangsu University Beamer style file
├── jsu_resources/                   # Template resource folder
│   ├── jsulogo.pdf                  # Jiangsu University emblem
│   ├── jsuname.png                  # Jiangsu University name (Chinese & English)
│   └── jsubackground.pdf            # Background image
├── example.tex                      # Example template file
├── JSU-Beamer-UniTrack.tex         # Original project example (for reference)
└── README.md                        # Documentation
```

## Quick Start

### Requirements

- TeX Distribution: TeX Live (recommended) or MiKTeX
- Compiler: XeLaTeX (required for Chinese support)
- Editor: TeXstudio, VS Code + LaTeX Workshop, etc.

### Compilation

Using XeLaTeX (recommended):

```bash
xelatex example.tex
xelatex example.tex  # Compile twice to generate correct TOC and references
```

Or using latexmk for automatic compilation:

```bash
latexmk -xelatex example.tex
```

### Usage

1. **Copy the example file**
   ```bash
   cp example.tex my-presentation.tex
   ```

2. **Modify basic information**

   In `my-presentation.tex`, update the following:

   ```latex
   \title{Your Presentation Title}
   \author[Name]{
       Name\ Major \& Class\\
       Student ID: xxxxxxxxxx\\
       {\small \url{https://github.com/your-username}}
   }
   \date{Month Year}
   ```

3. **Add content**

   Use `\section{}` to create sections, and `\begin{frame}...\end{frame}` to create slides.

4. **Compile to PDF**

   Compile twice with XeLaTeX to generate the final PDF.

## Common Features

### Create title page

```latex
\begin{frame}
    \titlepage
\end{frame}
```

### Create table of contents

```latex
\begin{frame}
    \frametitle{Contents}
    \tableofcontents
\end{frame}
```

### Create regular frame

```latex
\begin{frame}{Frame Title}
    Frame content
\end{frame}
```

### Two-column layout

```latex
\begin{frame}{Two-column Example}
    \begin{columns}
    \column{0.5\textwidth}
    Left content

    \column{0.5\textwidth}
    Right content
    \end{columns}
\end{frame}
```

### Lists

```latex
% Unordered list
\begin{itemize}
    \item First item
    \item Second item
\end{itemize}

% Ordered list
\begin{enumerate}
    \item First item
    \item Second item
\end{enumerate}
```

### Insert images

```latex
\begin{frame}{Image Example}
    \begin{center}
    \includegraphics[width=0.6\textwidth]{images/example.png}
    \end{center}
\end{frame}
```

### Emphasis blocks

```latex
\begin{block}{Title}
    Content
\end{block}

\begin{alertblock}{Alert}
    Important content
\end{alertblock}

\begin{exampleblock}{Example}
    Example content
\end{exampleblock}
```

## Contributing

If you have any questions or suggestions, feel free to submit an Issue or Pull Request.

## License

This template follows the MIT License and can be freely used and modified.

---

**Author**: Xu Yibo, Communication 2402
**Institution**: Jiangsu University
**Last Updated**: November 2025
