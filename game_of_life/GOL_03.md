# Three Ways to the Game of Life
## The Second Way

Our first attempt went well-enough that we learned
something and can do better next time. 

Previously we constructed a function, and while I am
sure you can think of many ways it could be improved, we should 
ensure we are using the correct tooling first.

Consider our steps of planning and doing:

1. Understand your computational goal to the degree that it could
    theoretically be done 'by hand'.
2. Envision a mapping of your 'by hand' method to the types,
    functions and constants available.
3. Iteratively plan and program as you learn or encounter issues.
    + Consider builtins, then the standard library, then the
      numFocus libraries, then other sources.

I would argue all we have really done are steps 1
and 2. With a little more programming experience we probably
would have seen the trouble on the edge coming.

Predominately you will find yourself using `numpy` and `pandas`,
and perhaps `xarray` for storing data and the like. So we will
approach step 3 and consider the object types and functions
made available from `numpy`, the others will wait until another
lesson.

How does one know what can be done with `numpy`? You read the
documentation. Now, I know that code documentation is not
welcoming towards newcomers; often it assumes knowledge you
may not yet have. I am also not telling you to abandon your
queries into stackoverflow or the like. Rather; the only way
to break out of endless stackoverflow or google queries as
to "how do I X?" is to be able to read and understand
documentation and source code. As our teaching philosophy
is to learn by doing that is exactly what we should do.

Advice for future you can be put aside for now. Immediately 
applicable advice is as follows:

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
+ Go through the [API reference](https://numpy.org/doc/stable/reference/index.html). This is the exhaustive list of stuff contained within `numpy`.


I hope you can see a plan emerging for applying a given
package to a problem you are working on. We first examine
the types of objects made available in that package and
ask if any of them are suitable for our use. Then we do
the same for methods of those objects, as as functions
provided by the package.

Hopefully you can at least inform your queries with the
correct names of objects and functions -- which should 
help a great deal.

+ [ ] Create the Game of Life (again) this time solve
  the edge case to some degree. Use `numpy`.
+ [ ] Write a stackoverflow question of an issue you
  run into. Provide an answer as well (if you can). 