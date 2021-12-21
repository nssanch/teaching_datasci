# Ways to the Game of Life -- The Second Way

*Here we continue upon our dual-purpose journey: to learn Pyton by implementing
a version of Conway's Game of Life. Here we assume you have completed the
previous notebook to your satisfaction.*

**The Zen of Python**

>Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!

[Tim Peters -- PEP 20](https://www.python.org/dev/peps/pep-0020/)

## Overview

Here we are going to do what you (surely) resisted doing previously -- examine
the internet for existing solutions. I caution you against spending too much time
examining other solutions, our goal here is to learn by doing, not to properly
engineer a solution. That said -- I know that new students need to see how others
approach problems. 

Here we take inspiration from an implementation by Peter Norvig, which you should
examine for yourself [here](https://nbviewer.org/url/norvig.com/ipython/Life.ipynb).

Recall our ***learning by doing*** process, as a data scientist you must be
cognizant of the down-stream consequences of a given data model. Norvig uses
a sparse representation using `set` objects. Here we aim to explore a fundamental
data structure in Python, the `set` and to explore the consequences of those
choices.


### Lab Overview

In examining the code of others we are going to try to pay
attention to the same things we consider in creating our own code:

+ Nature of the data model.
+ Input and output types of functions.
+ Complexity
  + Number of packages imported.
  + Number of functions declared.


### Lab Objectives

Our learning goals for this notebook:
+ Reinforce basic Python syntax, builtin functions, types and constants.
+ Reinforce self-learning methods and resources.
+ Introduce `set` objects and sparse representation.
+ Introduce the Standard Library.


## Lab

As in the previous lesson you should restrict yourself from using just anything.
For this lesson we are only considering the use of:

+ Python and included functions, types and constants.
+ The standard library.


### Task: Implement the Game of Life

1. Hand-draw a sketch of the solution Norvig implements.
  + [ ] Save to your data folder.
1. Using this notebook as a base:
   + [ ] Save a notebook in your FOLDER that has a implementation of the game of life that:
     + [ ] runs for (at least) 100 iterations.
     + [ ] Use the demonstrated sparse representation.
2. Bonus
   + [ ] Code your own display function.