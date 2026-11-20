# round()

## What it does
`round()` is a built-in function that rounds a number to a chosen number of decimal places.

## Syntax
```python
round(number, digits)
```

## Examples
```python
print(round(6.781, 2))    # 6.78
print(round(2.106, 2))    # 2.11
print(round(8.994, 2))    # 8.99
print(round(3.14159, 3))  # 3.142
```

## How it works
1. Keep the number of decimal digits I ask for.
2. Check the **next digit**.
3. If the next digit is 0-4 the last kept digit stays the same.
4. If the next digit is 5-9 the last kept digit goes up by 1.

| Number | Keep 2 digits | Next digit | Result |
|---|---|---|---|
| `6.781` | `6.78` | 1 | `6.78` |
| `2.106` | `2.10` | 6 | `2.11` |
| `8.994` | `8.99` | 4 | `8.99` |

## `round()` is a function not an operator
Operators are symbols between values like `+` `**` and `%`. Functions have a name and take arguments inside parentheses like `round()` `print()` and `input()`.

## Easy traps to watch out for
- **Cutting off digits without checking:** `round(3.14159, 3)` gives `3.142` not `3.141`.
- **Using a comma for decimals:** `3,14` is wrong so always use a dot like `3.14`.
- **Leaving out the second number:** `round(6.781)` rounds to a whole number (`7`) instead of 2 decimals.