# Digit DP

## Base conditions for DP:
- 2 numbers
- left and right pointers
- how many between L and R satisfy conditions X

### example 1:
- L		= 10,
- R		= 22,
- ans	= *simple*

### example 2:
- L		= 10,
- R		= 10^50,
- ans	= *much harder*

## queston:
using digit DP, count the total number of digit 1 appearing in all non-negative integers less than or equal to n.

### condition:
- 0 <= digit <= n

### logic:
- some numbers' index position; (dex)
- the current digit in that index position; (digit)
- if the current digit in the index position is <= n[dex][digit]; (at_limit)

### composited:
- `dp[dex] [digit] [at_limit: bool] [one's_count]` = count of 1's in `numbers <= n`, up to the index i

