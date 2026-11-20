# Input and Average

## What it does
`input()` reads what the user types. I use it to grab numbers, save them in variables, and find their average.

## Whole numbers
```python
a = int(input("Number: "))
b = int(input("Number: "))
c = int(input("Number: "))
print((a + b + c) / 3)
```
Typing `2`, `4`, and `6` prints `4.0`.

## Decimal numbers
```python
a = float(input("Number: "))
b = float(input("Number: "))
c = float(input("Number: "))
print((a + b + c) / 3)
```
Typing `2.5`, `3.5`, and `6.0` prints `4.0`.

## Saving the average in a variable
When I need the average again later I save it to a variable first:
```python
mean = (a + b + c) / 3
print(mean)
if mean >= 8:
    print("Good")
else:
    print("Bad")
```

## How it works
- `input()` always gives text so I wrap it in `int()` or `float()` to do math.
- `int()` is for whole numbers and `float()` is for decimals.
- `/` always returns a float so `4` comes out as `4.0`.

## Easy traps to watch out for
- **Missing parentheses:** `a + b + c / 3` only divides `c` by 3. Use `(a + b + c) / 3`.
- **Using `int()` on decimals:** Passing `2.5` into `int()` crashes the program so use `float()` instead.
- **Re-asking for input:** Reuse the `mean` variable you already saved instead of asking the user again.