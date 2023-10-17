# Complexity

## Big O notation

Describes roughly how runtime of program changes with input size.
We remove constants and low order terms.

### Example

`O(5n + 1)` is the same as `O(n)`

## Motivating example

Why should we care?

>
> <https://open.kattis.com/problems/pauleigon>

### O((p + q) / n)

```py
n, p, q = map(int, input().split())
turn = "paul"
for _ in range(0, p + q, n):
    if turn == "paul":
        turn = "opponent"
    else:
        turn = "paul"
print(turn)
```

### O(1)

```py
n, p, q = map(int, input().split())
if (p + q) // n % 2:
    print("opponent")
else:
    print("paul")
```
