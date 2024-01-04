## Description

You entrusted Petya, who works as a packer, with the responsible task of stacking boxes of different sizes
one into another, and the instructions were the following:
* The boxes must fit into each other (the total size of the boxes lying next to each other does not
exceed the size of the box in which they are put) — otherwise, they will get damaged.
* To put box B into box A, you must first open A and then open B.
* To close the box, you must first close all the boxes that are in it.
* If there are several boxes next to each other, then you need to close them in the order in which they
were opened.

Petya has already ruined a lot of boxes, but you decided to give him one last chance.

Check if Petya has packed the boxes correctly.

The nesting depth d(x) of box x that is not inside another box is 1. The nesting depth d(x) of box x that
is inside box y is d(y) + 1.

Check if Petya has packed the boxes correctly and find the maximum nesting depth among all the boxes.

### Input

The first line contains a single integer n (1 ≤ n ≤ 10 000) — the number of boxes.

Each of the following 2n lines contains a character: ‘O’ (open, i.e., Petya opens the box) or ‘C’ (close, i.e.,
Petya closes the box), and an integer s (1 ≤ s ≤ 100 000), which denotes the size of the box.

### Output

Print “Well done!” and an integer denoting the maximum nesting depth of the boxes if Petya has packed
the boxes correctly, or “You are fired!” otherwise.