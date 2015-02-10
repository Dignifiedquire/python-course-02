---
title: "Arrays, Queues and Stacks"
files: []
layout: 2-panels-tree

---
> TODO: Remove military references, add diagrams, unify usage of lists/array

Arrays, queues and stacks are the three most popular data structures in computer
science. All of them store items of a similar nature to be processed in a similar
way. These data structures lend themselves well to iteration (looping) and automation,
as well as restricting input and output values, which assists validation.

The differences between them are in the level of access. Arrays allow access to
all of their elements in any order. Their size is usually fixed in advance (but
can be resized at runtime) and arrays are slow and take up more memory – the price
to pay for the convenience of full access. A mechanical analogy would be that of a
revolver – by spinning the drum, any individual bullet can be "accessed" and the
bullets are clearly visible all at once. Similarly, any array element can be
overwritten, deleted, copied, etc.

Queues differ from arrays as only two end items, one at the "head", the other
at the "tail" are accessible to the program. We "feed" (push) items into the
queue on one end, and read/process items (pop) from another end. This saves
memory and speeds up the process as only two memory locations need to be open
to the rest of the program. The downsides include having to go through the
whole queue before a newly-added element can be processed. To continue with
our firearms analogy, queue would be like a belt-driven machine gun from the
WWI.

Stacks are even more restricted. Only one "end" is accessible to the program,
resulting in Last-in-First-Out order of processing. The analogy would be a
pistol magazine, where the first bullet loaded will be the last to come out.
Stacks are very fast and are used extensively in the CPU.


---
title: First List Operations
files: []
layout: 2-panels-tree
step: "01"

---
Let's take a look at creating a list in Python.

```python
names = ["Bob", "Jack", "Sonya"]
```

This creates a list with three elements. Now if we want to get back an element
of that list we can access it by using the **index**.

```python
print(names[0])
```

would print `Bob`, as it is the name at index `0`. Simlarly we can access the other
names like this:

```python
print(names[1]) # Jack
print(names[2]) # Sonya
```

## Challenge

Open [01.py](open_file "01/01.py") and write a function that prints all names
in the `names` list using a loop.