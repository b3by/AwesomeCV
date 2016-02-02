AwesomeCV
=========

[![forthebadge](http://forthebadge.com/images/badges/built-with-swag.svg)](http://forthebadge.com)

This is a simple latex class for CVs. It is heavily inspired by moderncv class
(you can find it [here](http://www.ctan.org/pkg/moderncv)).

AwesomeCV uses [`FontAwesome`](http://fortawesome.github.io/Font-Awesome/) icon
set, so ```lualatex``` is required when compiling.

Titlebox
--------

A simple titlebox can be generated as follows:

```latex
\begin{titlebox}

\authorname{Walter White Sr.}{awesome \emph{curriculum vit\ae}}

\qrcode{qrcode.png}
\includegraphics[scale=.07]{../pics/ww.png}

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

![alt tag](https://raw.githubusercontent.com/b3by/AwesomeCV/master/pics/tbox.png)

A generic title element can be added with:

```latex
\generic{\faMoney}{Rich as hell}
```

As result:

![alt tag](https://raw.githubusercontent.com/b3by/AwesomeCV/master/pics/generic.png)

Sections
--------

If you want to open a section, write:

```latex
\opensection{icon}{Title}
```

This will generate just the header for that section. The actual section content
has to be declared within:

```latex
\begin{describesection}
...
\end{describesection}
```

A section line is composed by the left side and the right side. Simply write:

```latex
\leftside{\bf sep 1982}
\rightsidecomplex{Master of Science in Chemistry}{California Institute of
Technology}{Los Angeles, California}{Final grade: the best}
\leftside{thesis title}
\rightsideplain{\textsc{Badass Proton Radiography}}
\leftside{advisor}
\rightsideplain{Some guy}
```

You will get:

![alt tag](https://raw.githubusercontent.com/b3by/AwesomeCV/master/pics/voice2.png)

The right part of a line can be declared as:

* ```\rightsideplain``` : one argument, one line
* ```\rightsidesingle``` : four arguments, two lines (the last argument takes
the second line)
* ```\rightsidecomplex``` : four arguments, three lines (argumens 2 and 3 take
the second line, argument 4 takes the last line)

Sections can contain subsections. You can add a subsection header with:

```latex
\subdescription{color}{icon}{Title}
```

A little bit more elaborate example:

![alt tag](https://raw.githubusercontent.com/b3by/AwesomeCV/master/pics/voice.png)

Spares
------

* I generated my qrcode [here](https://www.the-qrcode-generator.com/).
* Icon list can be found [here](http://ctan.mirror.garr.it/mirrors/CTAN/fonts/fontawesome/doc/fontawesome.pdf) (the package seems to be quite old, so please for a full list of icons refer to [this](https://fortawesome.github.io/Font-Awesome/icons/)).
* [Solarized](http://ethanschoonover.com/solarized) colors are used for the
  color palette.

Please report any error you get when using it.
