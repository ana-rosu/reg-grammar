# Regular Grammar 
This algorithm checks if an input string belongs to a right linear regular grammar. It takes in an input file containing a given grammar and an input string.

> Productions are of the form A → a or A → aB or A → epsilon, where epsilon is "", A, B are nonterminal symbols and a is a terminal symbol.
## Example

Suppose you have a file.txt containing the following right linear grammar:

```python
S -> aA | dE
A -> aB | aS
B -> bC
C -> bD | bB
D -> cD | e | epsilon
E -> epsilon
```
and you want to check if the input string `aaaaaad` can be generated by this grammar.

The algorithm will output `The word aaaaaad is generated by the grammar.`

Explanation:
<br>`aaaaaad` can be derived from the given grammar:
<br>S-> aA -> aaS -> aaaA -> aaaaS -> aaaaaA -> aaaaaaS -> aaaaaadE -> aaaaaad
