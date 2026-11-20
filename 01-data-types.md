# Data Types

## What they actually do
Data types are labels Python puts on values so it knows how to treat them—whether something can be used in math, treated as text, or read as a true/false flag.

## The four main types

| Type | What it holds | Example |
|---|---|---|
| `int` | Whole numbers (no decimals) | `8` |
| `float` | Numbers with a decimal point | `3.5` |
| `str` | Text wrapped in quotes | `"A"` |
| `bool` | Logic flags (`True` or `False`) | `True` |

## Checking what type something is
Not sure what Python thinks a value is? Check it with `type()`:

```python
print(type(8))
print(type(3.5))
print(type("A"))
print(type(True))
```

## `input()` and converting types
`input()` always returns text (`str`) even when someone types `42`. Trying to do `"42" + 1` throws an error so convert it first with `int()` or `float()`:

```python
x = int(input("Number: "))
```

## Easy traps to watch out for
- **Decimals use a dot not a comma:** Write `3.5` not `3,5`.
- **Quotes make it text:** `"8"` looks like a number but Python treats it like text.
- **Capitalize booleans:** Always write `True` and `False` with a capital first letter.