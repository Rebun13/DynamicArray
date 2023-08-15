# DynamicArray

## Description

Declare a 2-dimensional array, _arr_, of _n_ empty arrays. All arrays are zero indexed.

Declare an integer, _lastAnswer, and initialize it to _0.

There are _2_ types of queries, given as an array of strings for you to parse:

1. Query: 1 x y
   - Let _idx = ((x ⊕ lastAnswer) % n)_.
   - Append the integer _y_ to _arr[idx]_.

2. Query: 2 x y
   - Let _idx = ((x ⊕ lastAnswer) % n_.
   - Assign the value _arr[idx][y % size(arr[idx])]_ to _lastAnswer_.
   - Store the new value of _lastAnswer_ to an answers array.

Note: ⊕ is the bitwise XOR operation,which corresponds to the ^ operator in most languages.

## Returns

- int[]: the results of each type 2 query in the order they are presented

## Inputs

- The first line contains two space-separated integers, _n_, the size of _arr_ to create, and _q_, the number of queries, respectively.
Each of the _q_ subsequent lines contains a query string, _queries[i]_.
