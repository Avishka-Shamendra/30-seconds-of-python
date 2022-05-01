---
title: Coprime numbers
tags: math
expertise: beginner
firstSeen: 2022-05-01T07:28:59+0000
---

Checks if two numbers given are coprimes.

- Return `False` if at least of the numbers is less than or equal to `0`.
- Return `True` if both numbers are positive and greatest common divisor is `1`.
- Use inbuilt `math.gcd()` to check if the greatest common divsior is `1`.
- Return `False` in all other cases.


```py
from math import gcd

def are_coprimes(a,b):
  if(a<=0 or b<=0):
    return False
  if (gcd(a,b) == 1):
    return True
  return False
```

```py
print(are_coprimes(3,7)) # True
print(are_coprimes(3,15)) # False
```
