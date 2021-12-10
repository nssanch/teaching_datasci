# Three Ways to the Game of Life

+ [ ] Using this notebook as a base:
    + Make a game of life that runs a known repeating pattern for 100 
      iterations. 
    + Come up with a work-around for dealing with cells on 
      the edge of the grid.

> For the things we have to learn before we can do them, we learn by doing them.


You should first read all about the Game of Life at 
[Wikipedia](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life).

The game takes place on a 2-dimensional grid of cells, at each iteration
we enforce the following rules (from the wiki):

1. Any live cell with two or three live neighbors survives.
1. Any dead cell with three live neighbors becomes a live cell.
1. All other live cells die in the next generation. Similarly, all other 
   dead cells stay dead.

For this lesson you should restrict yourself to the following components
of Python.

+ [syntax]()
+ [functions](https://docs.python.org/3/library/functions.html#built-in-funcs)
    + [`sum()` or `+`]()
    + [`type()`]()
    + [custom functions via `def()`]()
+ [types](https://docs.python.org/3/library/stdtypes.html)
    + [`list`]()
    + [`set`]()
    + integers
    + strings
    + floats
+ [constants](https://docs.python.org/3/library/constants.html#built-in-consts)
    + [`True`]()
    + [`False`]()
    + [`None`]()

## Goal Breakdown

Now that we have a clear idea as to the process we would like to implement, and
have a notion of which tools are available for use, we can being to breakdown
our larger goal into discrete tasks.

> With more experience you will find initial planning easier and more fruitful. 
If you are new to programming you should explore functions in an almost 
child-like manner until you are satisfied with some level of understanding.


This process of breaking down goals is iterative in practice. So I will
demonstrate that process here. Any visualization at this step we will 
just hope can be handled by looking at raw output. I begin with a natural
language description broken down into steps with arrows:

1. Populate a world with cells based on given conditions, then simulate a step,
    and update the world. Loop the simulation step.

    Conditions --> World Population --> Simulate Step --> Output --> loop

It is hopefully clear (or unclear) to you as to why the above is not quite
right. It starts well enough with generating a world from some conditions,
but the structure of the loop doesn't come through correctly. We can try
again, this time remembering that we are running our simulation for only a
limited number of steps:

2. Populate a world with cells based on given conditions, then for each
    iteration apply the rules and update the population.

    Conditions --> World Population --> for each --> apply rules --> update world
    
When it is no longer reasonable or obvious how to break down a given step,
it is time to detail that step out more to determine which is appropriate.
Sometimes this is done in theory, sometimes this happens after you find
that code for a step grows more complex than anticipated.

### Modeling Data

Here we must consider which of the builtin object types we should use to
hold the data needed for our simulation.

#### The Cell

The first question to answer is how should we represent a cell, and how
should we know if it is alive or dead?

After some thought, we can envision a few options:

1. informative, unambiguous strings. Like "Alive" and "Dead".
2. Integers, like 0 for dead, and 1 for alive.
3. Boolean values, False for dead and True for alive.

When we consider that we should like to count these in order to apply
the rules, it seems that the integer representation should be more
convenient.

After all that let us try some trilling code:

OBJECTIVES HERE.

#### The World

Now that we have a notion of what a cell can be modeled as, we need
a place to put them. This has to have some notion of order, as we
must examine which cell is adjacent to which neighbor.

>In more programming or computer-science oriented approaches a great to-do
is made over the nature of modeling data. Usually this approach is a bit
beyond what we need in data science. To clarify via an example: 1) Consider
designing a website that has users logging into it to update content on
that site. 2) You have survey data that is indexed on a per-person basis.
Data scientist often find themselves closer to the second example, though
in simulations with dynamic or random data we do have to concern ourselves
with practices more commonly and rigorously used in 1. I mention this as
you are sure to read well-intended advice that may goad you into
over-engineering your application.

Now, the documentation under lists tells us how we can construct one, but
not much about what can go in one -- because you can put anything in there.

Here, we can make a list of cells:

Now I hope the choice of what *type* of object to use is clear, even if what an
object actually is remains murky.


Now, we have a number of issues with how this behaves at the edges.
The top and bottom rows are kept the same, while the left and right
edges are (mostly) set to zero.

That said, I hope that the 'real' lesson has become clear:

1. Understand your computational goal to the degree that it could
    theoretically be done 'by hand'.
2. Envision a mapping of your 'by hand' method to the types,
    functions and constants available.
3. Iteratively plan and program as you learn or encounter issues.

As you gain experience you will find the ease and depth of your
planning increases.