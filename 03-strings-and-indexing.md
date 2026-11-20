# Strings and Indexing

## What it is
A string is just text. Every letter or symbol inside it has a spot and I can grab a single character by its spot using square brackets.

## Positions
You can count from the front starting at `0` or from the back starting at `-1`.

| character | P | Y | T | H | O | N |
|---|---|---|---|---|---|---|
| from start | 0 | 1 | 2 | 3 | 4 | 5 |
| from end | -6 | -5 | -4 | -3 | -2 | -1 |

```python
word = "PYTHON"
print(word[0])    # P
print(word[-1])   # N
print(word[-2])   # O
```

## Reversing a word
I grab the characters from the end and glue them together with `+`:
```python
word = "PYTHON"
if word == "PYTHON":
    print(word[-1] + word[-2] + word[-3]
        + word[-4] + word[-5] + word[-6])
```
This prints `NOHTYP`.

For a 4-letter word like `"KODI"` I use `[-1]` down to `[-4]` and get `IDOK`.

## How it works
- `word[-1]` gives the last character `word[-2]` gives the one before it and so on.
- `+` joins strings together so `"N" + "O"` gives `"NO"`.
- You join as many pieces as there are letters in the word.
- `if word == "PYTHON":` checks if the word matches `"PYTHON"`.

## Common mistakes
- Thinking `-1` is the first letter. `-1` is the last one since `0` is already the first.
- Going out of range like `word[-8]` on a 7-letter word which causes an `IndexError`.
- Writing `=` instead of `==` inside the `if`.
- Missing the 4 spaces before `print` inside the `if`.