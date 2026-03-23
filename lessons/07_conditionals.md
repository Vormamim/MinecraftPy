# Lesson 7 — Conditionals: Making Decisions

---

## Learning Objectives

By the end of this lesson you will be able to:

- Explain what a conditional statement is
- Use `if` and `else` to run different code depending on a condition
- Use comparison operators (`>`, `<`, `==`) to write conditions
- Write a program that chooses a block type based on a variable's value

---

## Theory: What Is a Conditional?

Think about getting dressed in the morning. You might think: *"If it is raining, I will take an umbrella. Otherwise, I will wear sunglasses."* You are making a **decision** based on a condition.

A **conditional** in Python works the same way. It checks whether something is true, and runs different code depending on the answer:

- **If** the condition is true → run one block of code
- **Else** (if the condition is false) → run a different block of code

This is how programs make decisions and behave differently depending on the situation.

### The `if` Statement

```python
if condition:
    # code that runs only if the condition is true
```

### The `if/else` Statement

```python
if condition:
    # code that runs if the condition is true
else:
    # code that runs if the condition is false
```

### The `elif` Statement (Optional Extra)

You can also check multiple conditions using `elif` (short for "else if"):

```python
if size > 10:
    # large
elif size > 5:
    # medium
else:
    # small
```

### Comparison Operators

These operators compare two values and return either **True** or **False**:

| Operator | Meaning | Example |
|---|---|---|
| `>` | Greater than | `size > 5` → True if size is 6, 7, 8... |
| `<` | Less than | `size < 5` → True if size is 4, 3, 2... |
| `==` | Equal to | `size == 5` → True only if size is exactly 5 |
| `>=` | Greater than or equal to | `size >= 5` → True if size is 5, 6, 7... |
| `<=` | Less than or equal to | `size <= 5` → True if size is 5, 4, 3... |
| `!=` | Not equal to | `size != 5` → True if size is anything except 5 |

### Indentation in Conditionals

Just like loops, the code inside an `if` or `else` block must be **indented** with 4 spaces:

```python
if size > 5:
    agent.set_item(GOLD_BLOCK, 64, 1)   # ← indented: runs only if condition is true
else:
    agent.set_item(STONE, 64, 1)         # ← indented: runs only if condition is false
```

---

## Code Example

```python
# Set the size of the path
size = 6

# Choose a block type based on the size
if size > 5:
    # Use gold blocks for large sizes
    agent.set_item(GOLD_BLOCK, 64, 1)
else:
    # Use stone for smaller sizes
    agent.set_item(STONE, 64, 1)

# Build the path
for i in range(size):
    agent.place(DOWN)
    agent.move(FORWARD, 1)
```

### What This Code Does

1. `size` is set to `6`.
2. The `if` statement checks: is `6 > 5`? Yes — so the Agent loads **gold blocks**.
3. The loop builds a path of `size` (6) blocks using gold.

If you change `size` to `3`:
- The `if` checks: is `3 > 5`? No — so it goes to `else` and loads **stone blocks**.
- The loop builds a 3-block stone path.

---

## Try It

1. Open Code Builder and type the code above.
2. Click **Run** with `size = 6` and observe the block type used.
3. Change `size = 6` to `size = 3` and run again. Does the block type change?
4. Apply the **Run → Observe → Explain** rule: what decision is the `if` statement making?

---

## Modify It

Try each of these changes:

1. **Change the size** — set `size = 3` and observe that stone is used. Set `size = 8` and observe that gold is used. The block type changes automatically.
2. **Change the threshold** — change `> 5` to `> 10`. Now what value of `size` is needed to trigger gold blocks?
3. **Add a third option** — add an `elif` condition between the `if` and `else` to handle a medium size. For example:
   ```python
   if size > 10:
       agent.set_item(GOLD_BLOCK, 64, 1)
   elif size > 5:
       agent.set_item(WOOD, 64, 1)
   else:
       agent.set_item(STONE, 64, 1)
   ```

---

## Challenge

Write a program that builds a path with **different block types for odd and even sizes**:

- If `size` is greater than 6 (large path) → use **diamond blocks**
- If `size` is between 3 and 6 (medium path) → use **wood blocks**
- If `size` is 3 or less (small path) → use **stone blocks**

Use `if`, `elif`, and `else` to handle all three cases. Test your program with at least three different values of `size`.

---

## Bloom's Taxonomy Check

🧠 **Remember** — What are the two keywords used to create a basic conditional in Python?

💡 **Understand** — In your own words, explain what the `else` block does. When does the code inside `else` run?

🔧 **Apply** — Write an `if/else` statement that sets the Agent's block to `GOLD_BLOCK` if `height > 8`, and `STONE` otherwise.

🔍 **Analyse** — Look at this code. For each value of `size` below, say which block type will be loaded:
```python
if size > 10:
    agent.set_item(GOLD_BLOCK, 64, 1)
elif size > 5:
    agent.set_item(WOOD, 64, 1)
else:
    agent.set_item(STONE, 64, 1)
```
- `size = 12`
- `size = 7`
- `size = 2`

⚖️ **Evaluate** — A student uses three separate `if` statements instead of one `if/elif/else` chain. Could this cause problems? Give an example where the results would be different.

🚀 **Create** — Design a program where the Agent builds a structure that **looks different depending on a single variable**. For example, set a variable called `theme` and use conditionals to choose different block types and sizes for each theme value. Test at least two themes.

---

## Key Vocabulary

| Term | Definition |
|---|---|
| **Conditional** | A statement that runs different code depending on whether a condition is true or false |
| **`if`** | Keyword that starts a conditional check |
| **`else`** | Keyword for code that runs when the `if` condition is false |
| **Comparison operator** | A symbol like `>`, `<`, or `==` that compares two values and returns True or False |

---

## What's Next

Your programs can now make decisions. Before the final project, the next lesson covers **debugging** — finding and fixing errors in your code, which is an essential skill for every programmer.

➡️ **Next: [Lesson 8 — Debugging: Finding and Fixing Errors](08_debugging.md)**
