# codeforce-4A-Watermelon

## Link : https://codeforces.com/problemset/problem/4/A

## Problem Statment:

One hot summer day Pete and his friend Billy decided to buy a watermelon. They chose the biggest and the ripest one, in their opinion. After that the watermelon was weighed, and the scales showed w kilos. They rushed home, dying of thirst, and decided to divide the berry, however they faced a hard problem.

Pete and Billy are great fans of even numbers, that's why they want to divide the watermelon in such a way that each of the two parts weighs even number of kilos, at the same time it is not obligatory that the parts are equal. The boys are extremely tired and want to start their meal as soon as possible, that's why you should help them and find out, if they can divide the watermelon in the way they want. For sure, each of them should get a part of positive weight.

### Input
The first (and the only) input line contains integer number w (1 ≤ w ≤ 100) — the weight of the watermelon bought by the boys.

### Output
Print YES, if the boys can divide the watermelon into two parts, each of them weighing even number of kilos; and NO in the opposite case.

### Examples
input : 8
output : YES
### Note

For example, the boys can divide the watermelon into two parts of 2 and 6 kilos respectively (another variant — two parts of 4 and 4 kilos).



## Explanation
If you add two even numbers together, you always get an even number — so
right away, if `w` is odd, there's no way to split it into two even parts.
That part's easy. But just because `w` is even doesn't mean we're done. The
smallest even number greater than zero is 2, so the smallest possible split
is `2 + 2 = 4`. That means `w = 2` is a special case that fails — even
though 2 is technically even, the only way to split it would be `0 + 2`,
and 0 doesn't count since each part has to be positive. So really, the rule
comes down to this: the watermelon can be split the way the boys want as
long as `w` is even and at least 4.

## Algorithm

1. Read the integer `w`.
2. If `w` is even and `w > 2`, print `YES`.
3. Otherwise, print `NO`.








