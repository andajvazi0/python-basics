# Operators

## What they are
Operators are symbols that do something with values like adding, comparing, or saving them.

## Arithmetic operators

| Operator | What it does | Example | Result |
|---|---|---|---|
| `+` | adds numbers or joins text | `2 + 3` | `5` |
| `-` | subtracts | `5 - 2` | `3` |
| `*` | multiplies | `4 * 3` | `12` |
| `/` | divides (always a float) | `12 / 3` | `4.0` |
| `//` | floor division (whole part) | `19 // 4` | `4` |
| `%` | remainder | `19 % 4` | `3` |
| `**` | power | `3 ** 3` | `27` |

## Floor division and remainder
`//` shows how many times one number fits into another and `%` shows what is left over.
```python
print(19 // 4)   # 4
print(19 % 4)    # 3
```
Check: `19 = 4 * 4 + 3`.

```python
print(25 // 7)   # 3
print(25 % 7)    # 4
print(11 // 3)   # 3
print(11 % 3)    # 2
```

## Power
`a ** b` means `a` multiplied by itself `b` times.
```python
print(3 ** 3)    # 27  (3 * 3 * 3)
print(4 ** 3)    # 64
print(10 ** 3)   # 1000
```

## Even or odd
If dividing by 2 leaves a remainder of 0 the number is even.
```python
n = 8
if n % 2 == 0:
    print("Even")
```

## Comparison operators

| Operator | Meaning |
|---|---|
| `==` | equal to |
| `>` | bigger than |
| `>=` | bigger than or equal to ("at least") |
| `<` | smaller than |

## Assignment operator
`=` saves a value into a variable. `x = 5` is not the same as `x == 5`.

## Order of operations
1. `**`
2. `*`, `/`, `//`, `%`
3. `+`, `-`

Parentheses `( )` always run first.
```python
print(2 ** 5 + 10 // 3)   # 32 + 3 = 35
```

## Common mistakes
- `10 ** 2` gives `100` not `5`. `**` is for powers not division.
- `%` gives the remainder not the quotient.
- `/` always gives a decimal (`4.0`) while `//` gives a whole number.
- Using `=` instead of `==` when checking equality.