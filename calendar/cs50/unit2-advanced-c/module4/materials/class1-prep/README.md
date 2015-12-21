##### Module 4

# Class 1 Prep

Before coming to [Class 1](../class1), please complete the following tasks:

##### More practice with Recursion

Task | Resource Type | Link  | Instructions
--------------|------|------|-------------
Watch | Doug's Playlist | <a href="https://www.youtube.com/watch?v=beqqGIdabrE&index=7&list=PLhQjrBD2T383tGruv374_Yee84qbXeJjq" target="_blank">Call Stack</a> | Watch these videos on the Call Stack, a fundamental concept in computer science that's especially helpful in understanding recursion.
Study | CS50 Study | <a href="https://study.cs50.net/recursion" target="_blank">recursion</a> | Review these materials detailing how recusion works
Rewatch | Lecture | <a href="https://www.youtube.com/watch?v=9WsyLL6KVBY" target="_blank">Week 4, (first 25 minutes)</a>  | THIS IS OPTIONAL. We already saw this last week, but if you want some more recursion material, this might help.

##### Leading up to Pointers:

Resource Type | Link | Task | Instructions
--------------|------|------|-------------
Lecture | <a href="https://www.youtube.com/watch?v=9WsyLL6KVBY" target="_blank">Week 4 (25 minutes in)</a> | Watch | only watch the second half
Lecture Notes | <a href="http://cdn.cs50.net/2015/fall/lectures/4/m/notes4m/notes4m.html#swap" target="_blank">Week 4 / Swap</a> | Read
Lecture Notes | <a href="http://cdn.cs50.net/2015/fall/lectures/4/m/notes4m/notes4m.html#debugging_with_cs50_ide" target="_blank">Week 4 / Debugging</a> | Read | steps through swap
Lecture Notes | <a href="http://cdn.cs50.net/2015/fall/lectures/4/m/notes4m/notes4m.html#pointers" target="_blank">Week 4 / Pointers</a> | Read | Under the hood, a `string` is just a `pointer` to a `char`. This means that the "value" inside a `string` variable is not actually the contents of the text. Instead it is a number pointing to the memory address where the text is truly located-- more specifically, where the first `char` is located.  
Walkthrough | <a href="https://www.youtube.com/watch?v=ETSddwPGjNM&list=PLhQjrBD2T382SQnebs5bf6BkngrHTbJKg&index=5" target="_blank">noswap</a> | Follow-Along |
Walkthrough | <a href="https://www.youtube.com/watch?v=Q9d8F9dXxbA&list=PLhQjrBD2T382SQnebs5bf6BkngrHTbJKg&index=1" target="_blank">compare-0</a> | comparing strings (broken) | Watch
Supplement | [Why Pointers](../supplementary-resources/why-pointers) | Read | TODO res: recap by summarizing the problem, why swap and compare dont work, but with pointers they will.


##### Pointers

Task | Type | Link | Notes
-----|------|------|------
Watch | Lecture | <a href="https://www.youtube.com/embed/uYiVtZHns-A?autoplay=1&rel=0&start=1545" target="_blank">Week 4 / Continued</a> | Just the second half. We'll do the first half in Class 2 Prep.
Read | Lecture Notes | <a href="http://cdn.cs50.net/2015/fall/lectures/4/w/notes4w/notes4w.html#strings_and_pointers" target="_blank">Week 4, continued / Strings and Pointers</a> |
Watch | Doug's Playlist | <a href="https://www.youtube.com/watch?v=yOdd3uYC--A&list=PLhQjrBD2T383tGruv374_Yee84qbXeJjq&index=2" target="_blank">Pointers</a> | prereqs: hex (a little)
Watch | Walkthrough | <a href="https://www.youtube.com/watch?v=jE_bs-QNj3c&index=2&list=PLhQjrBD2T382SQnebs5bf6BkngrHTbJKg" target="_blank">compare-1</a> | comparing strings (fixed)
Watch | Walkthrough | <a href="https://www.youtube.com/watch?v=1PoFw5_p0xk&index=6&list=PLhQjrBD2T382SQnebs5bf6BkngrHTbJKg" target="_blank">pointers</a> | print str one char at a time using pointers
Study | CS50 Study | <a href="https://study.cs50.net/pointers" target="_blank">pointers</a>
Do | Exercise | [Custom strcmp](./materials/exercises/custom-strcmp) | Practice using pointers by implementing your own version of the `strcmp` function
Watch | Short | <a href="https://www.youtube.com/watch?v=gv6i2CJm57Q&list=PLhQjrBD2T381pcj3Ph49iiDkrhZ9FHpHP&index=4" target="_blank">Pointers</a> | prereqs: dereferencing, malloc
Watch | Section | <a href="https://youtu.be/SppBaGROtX0?t=370" target="_blank">Jason Hirschorn on Pointers</a> | really good

##### malloc

Task | Type | Link | Notes
-----|------|------|------
Watch | Walkthrough | <a href="https://www.youtube.com/watch?v=6o-w4CIWP84&index=12&list=PLhQjrBD2T383fi16gN97XlrTwdxDq2QWZ" target="_blank">sizeof</a> | Learn about the `sizeof` operator. Harvard classifies this as belonging to Week 1, but we postponed it till now, since this is the context where you'll see `sizeof` being used.
Read | Lecture Notes | <a href="http://cdn.cs50.net/2015/fall/lectures/4/w/notes4w/notes4w.html#memory_allocation" target="_blank">Week 4, continued / Memory Allocation</a>
Watch | Doug's Playlist | <a href="https://www.youtube.com/watch?v=ywqB3ZTf8OE&list=PLhQjrBD2T383tGruv374_Yee84qbXeJjq&index=3" target="_blank">Dynamic Memory Allocation</a>
Watch | Walkthrough | <a href="https://www.youtube.com/watch?v=zwKBMSLYrk4&index=3&list=PLhQjrBD2T382SQnebs5bf6BkngrHTbJKg" target="_blank">copy-0</a> | copy a string (broken)
Watch | Walkthrough | <a href="https://www.youtube.com/watch?v=ebQSYaneMms&list=PLhQjrBD2T382SQnebs5bf6BkngrHTbJKg&index=4" target="_blank">copy-1</a> | copy string (fixed)
Do | Exercise | <a href="../exercises/double-copy" target="_blank">Double Copy</a> | This is a slight twist on the `copy-1` program you just wrote.
Watch | Short | <a href="https://www.youtube.com/watch?v=z3j-gK1u6Kg&index=6&list=PLhQjrBD2T381pcj3Ph49iiDkrhZ9FHpHP" target="_blank">Strings</a>
Do | Exercise | <a href="../exercises/swap-cycle" target="_blank">Swap Cycle</a> | TODO exc: make them implement a function like `swap`, but with 3 variables instead of 2, in which `y` takes the value from `x`, `z` from `y` and `x` from `z`.


