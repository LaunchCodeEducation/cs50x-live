##### Module 3
[Back to Class 2](../../class2)
# Studio: Multiplication and Exponents

### Part 1
In this studio, you will be writing code that performs multiplication and exponents recursively.

Since these two functions are separate from each other, we will use separate files for them. You may want to take a look at <a href="../../resources/spread-out">this resource about multiple files</a> before working on this studio.

As a starting point you are provided with some files for the exponentiation function. [expt.c](expt.html) includes starter code for the exponentiation function as well as some tests for multiplication and exponentiation in a main method.

You have also been supplied a [Makefile](Makefile.html), but if you try to run it you'll see that there are some issues:

```nohighlight
~/workspace $ make
g++ expt.c mult.c mult.h -o expt
g++: error: mult.c: No such file or directory
g++: error: mult.h: No such file or directory
```

The first line attempts to make the program. The next line shows what the makefile is trying to do: compile a program that consists of three files, `mult.c`, `mult.h`, and `expt.c`. Unfortunately we are missing two of those files: `mult.c` and `mult.h`.

### Part 2
Your first task should be to create those files. Let's start with `mult.h`. This is the header file for the multiplication function, and should include the function *prototype*. A prototype defines what a function uses for its inputs and outputs, but does _not_ define what the function does. It is used to tell other parts of your program what kinds of functions are available for use.

To keep things simple, our multiplication function will focus on integers. Our function should take two integers as input and return an integer as output. This should be enough information to construct your prototype.

Believe it or not, the header file is now complete! It may seem silly to have only a single line of code in the header file, but for this example it is sufficient. More complex programs will require more complex header files, but this is fine for now.

### Part 3
Let's move on to `mult.c`. This file should contain the entire multiplication function. Fortunately you have already written the function definition - that's what the prototype is! Go ahead and copy it into the `mult.c` file.

All that's left now is to write the function body - how do we want our multiplication function to behave? It would be easy to use the multiplication operator (`*`) and call it a day, but we're going to give you some restrictions to make this a little bit more challenging. Specifically, you are _not_ allowed to use the multiplication operator. You should perform multiplication using repeated addition instead. Also, you should acommplish this using *recursion*. That means loops are not allowed for this studio.

Your multiplication function should be able to handle both positive and negative integers. To make things easier, focus on only positive integers first. Once you are satisfied that multiplication works for positive values, see if you can tweak your code to make it work with negative values as well. Hint: it may be useful to create a second (perhaps non-recursive) function that checks whether the integers are positive or negative and proceeds accordingly. Be sure to ask for help if you get stuck!

As always, it is important to test your code. It may be a good idea to write a simple `main` method in `mult.c` that you can use to test your `mult` function.

### Part 4
Once you are satisfied with your multiplication function, it is time to turn our attention to exponentiation. Exponentiation can be thought of as repeated multiplication, much like multiplication can be thought of as repeated addition. Like with the `mult` function, however, you are faced with some restrictions. The multiplication operator is still not allowed. Instead you should use the recursive `mult` function that you wrote. In order to do this, we need to tell the exponentiation function what the multiplication function looks like. We can do this by referring to the header file that we created.

Header files are referenced with the `#include` statement. So to include our header file in `expt.c`, we would type `#include "mult.c"`. Go ahead and add this to the `expt.c` file now.

You are now ready to use your multiplication function to compute exponents. Your solution should be recursive, so loops are still not allowed. Make sure to use your `mult` function to perform multiplication! Anywhere that you would normally use `*` should be replaced with a function call to `mult`.

You should now be able to use `make` to run the provided test cases and check your work. Notice that for `expt`, the base (the first number) can be negative, but the exponent (the second number) cannot.

*You can grab a copy of these instructions from Helpful Resources <a href="../../../../../../..//helpful-resources/modules/module-3.html#class-2-studio-multiplication-and-exponents" target="_blank">here</a>. They are formatted as comments so that you can put it at the top of your program in the CS50 IDE. Remember the compiler ignores any comments, so this won't affect your program! You can start writing your code right after the comments.