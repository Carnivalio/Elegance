# Why Python Is Popular In Data Science

## Introduction

[Python](https://en.wikipedia.org/wiki/Python_(programming_language)) is an interpreted, dynamically-typed language with a precise and efficient syntax. Python has good [REPL](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop), this is one of many reasons why choose Python over other programming languages such as [C](https://en.wikipedia.org/wiki/C_(programming_language)), [C++](https://en.wikipedia.org/wiki/C%2B%2B), [C#](https://en.wikipedia.org/wiki/C_Sharp_(programming_language)) or [Java](https://en.wikipedia.org/wiki/Java_(programming_language)). But there are popular alternatives to Python for data science purpose, such as [R](https://en.wikipedia.org/wiki/R_(programming_language), [Matlab](https://en.wikipedia.org/wiki/MATLAB)/[Octave](https://en.wikipedia.org/wiki/GNU_Octave), and [Mathematica](https://en.wikipedia.org/wiki/Wolfram_Mathematica)/[Sage](https://en.wikipedia.org/wiki/SageMath).

Python is pretty easy to learn and also has a very large [community](https://www.python.org/community/), this means large [documentation](https://www.python.org/doc/) as well, thefore there are many growing data analytics libraries are available.

## What's In Python For Data Scientists?

Python community has many work invested in Python, one of them is this functionality:
- [Numeric](http://hugunin.net/story_of_jython.html): extension for Python to support numberic analysis as naturally as [M]atlab does.
- [NumPy](http://www.numpy.org/): numeric then evolved to NumPy (Numeric Python?) later on.
- [matplotlib](http://matplotlib.org/): several years after NumPy, the plotting functionality from Matlab was ported to python as matplotlib.
- [SciPy](https://www.scipy.org/): this library was born around NumPy and matplotlib, those 2 libraries bundled into one SciPy library.

That's not the only thing Python has, recently there are several popular features from R and Mathematica which ported into Python. To extend python capabilities as mentioned above, these are libraries to extend Python's useful features for data scientist:
- [pandas](http://pandas.pydata.org/): as the data frame and associated manipulation (originated from the *plyr* and *reshape* packages) ported from R.
- [skikit-learn](http://scikit-learn.org/stable/): presents a common interface to many machine learning algorithms, similar to the *caret* package in R.
- [IPython notebooks](http://blog.fperez.org/2012/01/ipython-notebook-historical.html): conceptual of "notebook" like the one that implemented in Mathematica/Sage.

## Python's Weakness From Data Scientists Perspective

After all of that, Python is far from perfect, some areas that Python are lacking are:
- Matlab/Octave syntax for array manipulation is still preferred over Python, also good to mention the R syntax for formula specification is also quite nice.
- The matplotlib library is hard to install, hard to use, and doesn't support building interactive visual for the web.
- The scalability limitation of NumPy and pandas when working with large data sets.
	- [Anaconda](https://www.anaconda.com/) community is working to address this issue, but they won't produce something coherent and usable in a short period of time
- Python is still lacking an embedded, declarative language for data matipulation like LINQ project. Pandas is useful as a low-level data manipulation toolkit, but working with complex operations this way could be very frustrating.
- No specific IDE for data scientists, like for example R studio for R.
