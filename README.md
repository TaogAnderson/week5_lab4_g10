# Lab 04 - SOP/POS and KMaps

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

We learned how to go from a truth table to physical input on a board and all the steps that make up this process. Prior to this when we were making truth tables and K-maps with inputs and outputs were things that existed in isolation but after this we see how they connect to physical lights and switches on a Basys-3.

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?
Because only 1 variable changes between the columns/rows on the edges. The reason you can group across any column or row next to each other is because only 1 of the variables is changing between them this is why 3 and 4 variable K-maps must me reorganized so that only 1 variable ever changes between rows and columns.

### Why are the names Sum of Products and Products of Sums?
Because Sum of Products sums (ors) groups of products (ands) together to represent the output in an equation. For Products of Sums it takes products (ands) of groups of sums (ors).

### Open the test.v file – how are we able to check that the signals match using XOR?
It XORs the naive against the minterms and maxterms, if the output is the same it will come out to 1 instead of the expected 0 for a match, so if it isn't 1 the minterm/maxterm output is correct. If it comes out to 1 it knows to alert us.
