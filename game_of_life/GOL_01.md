# Ways to the Game of Life -- The First Way

> For the things we have to learn before we can do them, we learn by doing them.

*Here we set out to create Conway's Game of Life in Python, our goal being to 
learn Python along the way. No previous programming knowledge is needed on the
part of the reader; only a willingness to learn by (failing) doing.*

Before we start this first lesson you will want to save a copy of the source notebooks to your private persistent storage space in `~/Desktop/classroom/myfiles`. To do so, start a terminal and enter the following commands:

```bash
cd ~/Desktop/classroom/myfiles  # Change directory.
git clone https://github.com/biggstd/teaching_datasci.git  # Use git to download a  copy of a remote directory.
```

You should now see a `teaching_datasci` folder, and a `game_of_life` folder within. Open the first notebook and continue.


## Overview

Here we are going to learn core components of Python by implementing Conway's game of life. You should read all about the Game of Life at [Wikipedia](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life).


### Lab Overview

***The learning by doing process:***

1. Understand your goal to the degree to which you could implement a
   solution 'by hand'. **Write this method down.**
2. Envision a mapping of your solution to one that makes use of
   the object types, functions and constants you have available.
3. Attempt to implement your plan.
4. Assess your implementation as you work, and be prepared to return
   to a previous step.

      
### Game of Life Overview

The game of life takes place on a 2-dimensional grid of cells, at each iteration
we enforce the following rules (from the wiki):

1. Any live cell with two or three live neighbors survives.
1. Any dead cell with three live neighbors becomes a live cell.
1. All other live cells die in the next generation. Similarly, all other
   dead cells stay dead.


### Lab Objectives

Our learning goals for this notebook:
+ Introduce basic Python syntax, builtin functions, types and constants.
+ Introduce self-learning methods and resources.


## Lab

***For this lesson you should restrict yourself to the following components
of Python.***

+ [Python](https://docs.python.org/3/reference/index.html#reference-index)
  + This reference document is too large to be useful beginners. I include it
    so that you are aware as to the 'official' documentation on the language
    syntax. It is fine if you do not 'use' this reference right away, its purpose
    is not instructional but referential. As such you should practice finding
    the same items of interest herein, as well as use this as a vocabulary source
    for internet queries.
+ [functions](https://docs.python.org/3/library/functions.html#built-in-funcs)
  + A much more practical reference list for the beginner: these are the functions
    'builtin' to Python. For the purposes of this notebook you can limit yourself
    to the builtin functions below, from which we will compose our own functions.
    + `help()`
    + `dir()`
    + `type()`
    + `sum()`
    + `len()`
    + `print()`
    + `range()`
    + `enumerate()`
+ [types](https://docs.python.org/3/library/stdtypes.html)
  + integer
  + boolean
  + list
+ [constants](https://docs.python.org/3/library/constants.html#built-in-consts)
  + True
  + False


### Task: Implement the Game of Life

1. Create directories:
   + [ ] Create a folder in the `homework` director. The title should be your last name.
   + [ ] Create a folder within that directory named `{LAST_NAME}_GOL`, save your results therein.
2. Create a sketch of the solution you plan to implement, make sure your approach to 
   solving the edge cases is mentioned in your sketch.
   + [ ] Save to your data folder.
3. Using this notebook as a base:
   + [ ] Save a notebook in your FOLDER that has a implementation of the game of life that:
     + [ ] uses markdown to display your sketched plan.
     + [ ] runs a known repeating pattern.
     + [ ] runs for (at least) 10 iterations.
     + You should have a clear idea as to if the output is correct based on the 
       pattern you choose.
   + [ ] Come up with a work-around for dealing with cells on the edge of the grid.
     + Implement a solution that is *practical for you*, regardless of how 'poorly'
       the simulation *runs*.
     + This means artifacts or violations of the rules are fine, so long as the code
       it self *runs*. We will improve upon our code in further lessons.
