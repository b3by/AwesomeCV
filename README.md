AwesomeCV
=========

This is a simple latex class for CVs. It is heavily inspired by CompactCV (you
can find it here: http://www.ctan.org/pkg/moderncv).

AwesomeCV uses ```fontawesome``` packet for the icons, so ```lualatex``` is
required when compiling.

A simple titlebox can be generated as follows:

```latex
\begin{titlebox}

\authorname{Walter White Sr.}{awesome \emph{curriculum vit\ae}}

\qrcode{qrcode.png}

\tcblower

\begin{showinfo}
\birthdate{september 7th, 1959}
\location{Albuquerque, New Mexico}
\mobile{1-505-1111}
\phone{1-505-1111}
\firstMail{gimmemeth@gmail.com}
\otherMail{alotofit@gmail.com}
\github{https://github.com/b3by}
\twitter{https://twitter.com/BryanCranston}
\end{showinfo}

\end{titlebox}
```

It will produce something like this:

![alt tag](https://raw.githubusercontent.com/b3by/AwesomeCV/master/titlebox.png)

I generated my qrcode here: https://www.the-qrcode-generator.com/

Icon list can be foun here: http://ctan.mirror.garr.it/mirrors/CTAN/fonts/fontawesome/fontawesome.pdf

Solarized colors are used: http://chrisvoncsefalvay.com/codebase/solarized-listings-in-latex

![alt tag](https://raw.githubusercontent.com/b3by/AwesomeCV/master/voice.png)

Please report any error you get when using it.
