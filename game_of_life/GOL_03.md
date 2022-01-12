# Ways to the Game of Life -- The Third Way

*Here we continue upon our dual-purpose journey: to learn Python by implementing
a version of Conway's Game of Life. Here we assume you have completed the
previous two notebooks to your satisfaction.*

> Standing on the shoulders of giants

It may have occurred to you that the number of functions and data models
contained in Python and the standard library are not quite enough for your
adventurous goals. So as in every field of science we scramble up to peer
out from the shoulders of the giants that came before us.

Were we computer scientists we would be much more interested in the
implementation of discrete mathematics. Since we are trying to be data
scientists we shall have to trust in those implementations rather than
spend our lives constructing our own.

Predominately you will find yourself using `numpy` and `pandas`,
and perhaps `xarray` for storing data and the like. So we will
approach step 3 and consider the object types and functions
made available from `numpy`, the others will wait until another
lesson.


## Overview

Here we take our first dip into an 'unofficial' package. One not a part
of the standard library. We implement the Game of Life again, this time
using the `numpy.ndarray` to model the grid.

Our learning goal here is the inclusion of external packages, along with
their objects and functions into our ***learning by doing*** process.


### Lab Overview

The flow for this lab is a little different. As stated, our true goal is
to get you comfortable using a package and its included documentation.

We first examine the types of objects made available in that package and
ask if any of them are suitable for our use. Then we do the same for 
methods of those objects, as as functions provided by the package.
Hopefully you can at least inform your queries with the correct names of 
objects and functions.


### Lab Objectives

Our learning goals for this notebook:
+ Reinforce basic Python syntax, builtin functions, types and constants.
+ Reinforce self-learning methods and resources.
+ Introduce the `numpy` package and the `numpy.ndarray` object.


## Lab

As in the previous lessons you should restrict yourself from using just anything.
For this lesson we are only considering the use of:

+ Python and included functions, types and constants.
+ The standard library.
+ The `numpy` package.


### Task: Learn some `numpy`

+ You need not submit any files for this task.
+ Go to the `numpy` [documentation](https://numpy.org/doc/stable/)
  and skim each section.
+ Look at a tutorial from the people who wrote `numpy`.
+ Go to the [fundamentals](https://numpy.org/doc/stable/user/basics.html)
  concerning the `numpy.ndarray` object (created with 
  `numpy.array()`) and:
  + Look at the methods that object has. That is: if you create
    an array:
    ```
    x = np.array([1, 2, 3])
    ```
    What are the methods / functions you can access via the
    period / dot syntax:
    ```
    x.sum()  # An example.
    ```
+ Skim through the [API reference](https://numpy.org/doc/stable/reference/index.html). 
  This is the exhaustive list of stuff contained within `numpy`.


### Task: Implement the Game of Life using `numpy`

+ [ ] Create the Game of Life (again). Use `numpy`.
