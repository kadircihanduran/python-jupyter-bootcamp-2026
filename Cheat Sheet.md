# Python & Jupyter Cheat Sheet
*A one-page reference for the 2026 Open Scholarship Bootcamp Python session.*

---

## Jupyter shortcuts

| Action | Shortcut |
|---|---|
| Run the current cell | **Shift + Enter** |
| Run cell, stay on it | **Ctrl + Enter** |
| Add a cell below | **B** (when cell is selected, not editing) |
| Delete a cell | **D D** (press D twice) |
| Restart everything | Kernel menu → *Restart Kernel* |

If something gets weird, **Restart Kernel** is your friend. It's like turning Python off and on again.

---

## Print and comments

```python
print("Hello!")          # show a value on screen
# anything after a # is a comment — Python ignores it
```

---

## Variables and the four basic types

```python
name     = "Ada"      # string  — text in quotes
age      = 28         # int     — whole number
height   = 1.65       # float   — decimal number
is_open  = True       # bool    — True or False (no quotes!)
```

`type(x)` tells you what kind of value `x` is.

---

## Math operators

| Operator | Meaning | Example |
|---|---|---|
| `+` `-` `*` `/` | add, subtract, multiply, divide | `5 + 3` → `8` |
| `**` | power | `2 ** 10` → `1024` |
| `%` | remainder (modulo) | `17 % 5` → `2` |

`x += 1` is shorthand for `x = x + 1`. Same idea works with `-=`, `*=`, `/=`.

---

## Strings (text)

```python
greeting = "Hello"
who      = "Ada"

greeting + ", " + who          # glue with +
f"Hello, {who}! You are {age}" # f-string — easier!

s = "Python is fun"
s.upper()           # "PYTHON IS FUN"
s.lower()           # "python is fun"
s.replace("fun", "great")
len(s)              # length
```

---

## Lists (collections)

```python
fruits = ["apple", "banana", "cherry"]

fruits[0]            # "apple"      — indexing starts at 0!
fruits[-1]           # "cherry"     — negative counts from the end
len(fruits)          # 3

fruits.append("date")        # add to the end
fruits.remove("banana")      # remove by value
```

---

## Comparisons → True/False

```python
5 > 3          # True
5 == 5         # True   ← compare with TWO equals
x = 5          # assign with ONE equal
"a" != "b"     # True   (not equal)
```

> The `=` vs `==` mix-up is the #1 beginner bug. `=` puts a value into a name. `==` asks "are these equal?"

---

## if / elif / else

```python
if temperature > 80:
    print("Hot!")
elif temperature > 60:
    print("Pleasant.")
else:
    print("Bundle up!")
```

The indented lines (4 spaces) belong to the block above. Indentation matters in Python.

---

## for loops

```python
for fruit in fruits:
    print(fruit)

for i in range(5):       # 0, 1, 2, 3, 4
    print(i)

for i in range(1, 11):   # 1 through 10
    print(i)
```

---

## Useful built-in functions

| Function | What it does |
|---|---|
| `print(x)` | display `x` |
| `len(x)` | length of a string or list |
| `sum(numbers)` | add up a list of numbers |
| `min(numbers)`, `max(numbers)` | smallest / largest |
| `type(x)` | what kind of value is `x` |
| `range(n)` | counts from 0 to n−1 |

---

## Reading an error message

When Python turns red, **read the LAST line first** — that's the actual problem. The lines above show *where* it happened.

```
NameError: name 'pritn' is not defined
```
→ You probably typed `pritn` instead of `print`. Look for typos.

```
IndentationError: expected an indented block
```
→ The line under your `if` / `for` / `def` needs to be indented (4 spaces).

```
TypeError: can only concatenate str (not "int") to str
```
→ You tried to mix text and a number with `+`. Wrap the number in `str(...)`, or use an f-string.

---

## Common beginner gotchas

- **Indexing starts at 0**, not 1. The first item of `my_list` is `my_list[0]`.
- **Indentation is part of the code.** Mixing tabs and spaces causes mysterious errors. Stick to spaces.
- **`=` is not `==`.** Assigning vs comparing.
- **Strings need quotes**, variable names don't. `print("name")` prints the word *name*; `print(name)` prints the value.
- **Cells share memory** until you restart the kernel. If a variable seems to have an old value, restart and re-run from the top.

---

## Where to look stuff up

- **Python docs:** https://docs.python.org/3/
- **Anything you forget:** Google "python how to ___" — the answer is almost always on Stack Overflow or the official docs.
- The two follow-up notebooks in this repo will reinforce everything above.
