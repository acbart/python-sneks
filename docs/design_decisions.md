This section will document design decisions that were made in developing the course.

# Why don't you teach X?

[**Why don't you teach Objects/Classes/OO more?**](#why-not-oo)

Two lessons were dedicated to writing classes, but this didn't seem like enough. It's likely that an entire module needs to be dedicated to this topic. Instead, we approach objects from more of a "use" side than a "create" side. 

[**Why don't you teach Functional Programming more?**](#why-not-functional)

We tried having a single day dedicated to them, and there wasn't enough time. You could probably replace one of the project weeks with a week on FP.

[**Why don't you teach Sets?**](#why-not-sets)

We had a lesson on it, but it wasn't important enough material to keep it around. You could probably put it back in without any problems.

[**Why don't you teach Recursion?**](#why-not-recursion)

Recursion is de-emphasized in Python compared to other forms of iteration. In particular, the language does not perform optimizations like tail recursion and has a relatively small call stack limit. Although some research indicates recursion might be easier to learn than other forms of iteration, there is also some evidence that teaching recursion first makes it harder to learn iteration later.

[**Why do you De-emphasize While loops?**](#why-not-while-loops)

While loops are extremely uncommon compared to For loops in Python. They are also rife with opportunities for students to get caught in infinite loops. Finally, the Python wiki itself suggests they are uncommon: https://wiki.python.org/moin/WhileLoop