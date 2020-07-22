# String

In C++ a string is a 1-D array of characters. Since strings are formed by array of characters, they are both similar.

### Contents

1. [Edit distance](#1-edit-distance)
2. [Heaps algorithm](#2-heaps-algorithm)
3. [Knuth morris pratt](#3-knuth-morris-pratt)
4. [Longest common subsequence](#4-longest-common-subsequence)
5. [Shunting yard](#5-shunting-yard)

---

## 1. Edit Distance

This algorithm finds the minimum number of edits which are required to convert string1 to string2. Edit here means either insert, remove or replace. The algorithm implemented here uses dynamic programming.

### Usage

```c++
MatrixChainMultiplier chain_multiplier = MatrixChainMultiplier({40, 30, 20, 10, 30});

// ull is a type alias for `unsigned long long`
ull optimal_cost = chain_multiplier.optimal_cost();     // 30000

std::string optimal_parenthesization = chain_multiplier.optimal_parenthesization();
// ((A(BC))D)
```

## Complexity

Time               | Space
-------------------|-------------------
_O(M*N)_           | _O(M*N)_

Where M and N are the lengths of the two strings.

## 2. Heaps algorithm

