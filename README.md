# Flux - ECT/UFRN

Este é uma adaptação do tema [Flux](https://github.com/pvanberg/flux-beamer/)
para beamer, com as cores e logotipos de acordo com os manuais de identidade
visual da [UFRN](https://ufrn.br/imprensa/identidade-visual) e da
[ECT](https://drive.google.com/drive/folders/0BxzvzGMijShuYU9XS2VkZkp4WW8?usp=sharing).

# Flux beamer

Flux is a modern style beamer presentation. It is based on simple design patterns and flat colors.

Original is available as template on [Overleaf](https://www.overleaf.com/latex/templates/flux-beamer/vhzbnhyymddd#).

> Disclaimer: This theme is mainly optimized for personal needs and shared without guarantees.

## Demos

![alt text](https://github.com/pvanberg/flux-beamer/blob/master/demo.png)

## Themes

Flux provides five differents color palettes. (asphalt, blue, red, green, gray)

![alt text](https://github.com/pvanberg/flux-beamer/blob/master/demo_themes.png)

## Minimal Working Example

```
\documentclass[9pt]{beamer}
\usepackage[sfdefault]{roboto}
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
\usepackage{styles/fluxmacros} 	% Define where theme files are located.
\usefolder{styles}
\usetheme[style=ect]{flux} % Available styles: ect, ufrn, asphalt, blue, red, green, gray

\title{Flux beamer template}
\subtitle{Modern theme v0.2 --- ECT--UFRN}
\author{John Doe}
\institute{Institute, location}
\date{\today}
\titlegraphic{assets/ECT_horiz.png}

\begin{document}

\titlepage

\begin{frame}
 \frametitle{Table of contents}
 \tableofcontents
\end{frame}

\end{document}
```

## Compilation

Due to the use of bibliography and tikz figures, the compilation sequence must follow:

```
pdflatex demo.tex
biber demo.tex
pdflatex demo.tex
pdflatex demo.tex
```

