#growth

Yet another obfuscated MATLAB code.


### Contents
- growth.m - the obfuscated code
- unobfusver.m - the unobfuscated version

### Explanation
This program demonstrates several techniques for 
functional programming in MATLAB using anonymous functions.
This code runs only by executing a single anonymous function,
without touching the global workspace at all,
and also without the help of external libraries.

When executed, this code outputs a figure of a forest, consisting of 9 trees.
The number of trees to draw could be changed by changing the constant 9
in the end of the code.

In this code, the following features are implemented/used:

- recursion (and loops)
- conditionals (and lazy evaluation)
- local variables ('let' clause)
- execution of multiple statements

Technical details

- Recursion is implemented by using the Y combinator.
- Loops are implemented by tail recursion.
- Conditionals are implemented by evaluating a function chosen from a list,
    where the index number is given by a formula consisting of relational operators.
- Lazy evaluation is performed by wrapping an expression with @()
    and then applying feval at a desired timing.
- Local variables are implemented by passing constants to a function through its arguments.

