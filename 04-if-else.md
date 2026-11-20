# If-else

## What it is
`if` runs a block of code when a condition is true and `else` runs when it is false. Python only picks one path.

## Basic if-else
```python
temp = int(input("Temperature: "))
if temp >= 0:
    print("It does not freeze")
else:
    print("It freezes")
```
Typing `5` prints `It does not freeze`. Typing `-3` prints `It freezes`.

## Nested if-else (three options)
```python
score = 65
if score >= 80:
    print("Very good")
else:
    if score >= 50:
        print("Enough")
    else:
        print("Weak")
```
This prints `Enough`.

## Comparing two variables
```python
a = 9
b = 2
if a > b:
    print("A is bigger")
else:
    if b > a:
        print("B is bigger")
    else:
        print("They are equal")
```

## Even or odd
```python
n = int(input("Number: "))
if n % 2 == 0:
    print("Even")
else:
    print("Odd")
```

## How it works
- `>=` means "at least" and `>` means "bigger than".
- `else` has no condition, just a colon.
- Code inside `if` or `else` is indented by 4 spaces and a nested `if` adds 4 more.
- In a nested if-else, I check the highest value first.

## Common mistakes
- Forgetting `:` after `if` or `else`.
- Using `=` instead of `==` in a condition.
- Forgetting the 4 spaces inside `if`.
- Putting a condition on `else` (`else x < 0:`) because `else` never takes one.
- Using `>` when the task says "at least" instead of `>=`.