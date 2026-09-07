# Code Kata
A set of repeatable, memorizable coding routines which cover a wide breath of fundamentals and allow you to learn language syntax without getting caught up in implementation. (The colors are just for fun, the order isn't neccesarily in order of mastery or difficulty.) The katas from green onwards are meant to problem language paradigms, forcing you to come into contact with core language design decisions.

## white
FooBar e.g.
```
1
2
Foo
4
Bar
...
14
FooBar
16
...
```

## yellow
CSV Parser

`./yellow.exe y_in.csv output.csv`
- Parses input csv, a table of non-negative integers
- Outputs `sum, product` for each row (products don't exceed $2^{64} - 1$)

## orange
Word Frequency Analyzer

`./orange.exe o_in.txt`
- Parses input text (upper/lowercase letter, periods, commas, spaces. Commas and periods always have spaces after them, and never have spaces before them. There are no double spaces.)
- Compute case-insensitive word frequency, output top 100 words sorted with descending count, e.g.
```
the 132
and 102
a 76
... (97 more)
```

## green
Graph BFS

```./green g_in.txt``` 

g_in.txt has $200$ rows each in the format of `val neighbor_count n1 n2 n3 ...`
Where neighbors are 0-indexed, (thus a node with a neighbor 0 would share an edge with the first row node). The graph will be connected.

BFS starting at the 0th node (row 1), and output node values in order of depth, for nodes of equal depth output in ascending order of value.

```
56
12
35
89
3
3
7
21
33
35
...
```

The purpose of this kata is to explore how the language handles structs/classes (or whatever they are called in your language), thus do not implement the graph via a global adjacency matrix.
