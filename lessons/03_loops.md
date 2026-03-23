# Lesson 3 — Loops: Doing Things Repeatedly

---

## Learning Objectives

By the end of this lesson you will be able to:

- Explain what a `for` loop is and why it is useful
- Use `range()` to control how many times a loop repeats
- Describe the role of the loop variable `i`
- Use correct indentation to show which code is inside the loop
- Write a loop that builds a path of blocks

---

## Theory: What Is a Loop?

Imagine you have a rubber stamp and you need to stamp the same pattern 10 times on a piece of paper. You could stamp it once, pick up the stamp, move it, stamp again... and repeat that 10 times. Or you could set up a machine that does the stamping automatically 10 times in a row.

A **loop** in Python is like that machine. Instead of writing the same lines of code over and over, you write them once and tell Python how many times to repeat them.

Without a loop, building a 10-block path looks like this:

```python
agent.place(DOWN)
agent.move(FORWARD, 1)
agent.place(DOWN)
agent.move(FORWARD, 1)
agent.place(DOWN)
agent.move(FORWARD, 1)
# ... and so on, 10 times
```

That is 20 lines of code just to build a path! With a loop, you can do the same thing in 3 lines.

### The `for` Loop

A `for` loop in Python repeats a block of code a set number of times. Here is the structure:

```python
for i in range(n):
    # code to repeat
```

- `for` — the keyword that starts the loop
- `i` — the **loop variable** (a counter that goes up by 1 each time); you can name it anything, but `i` is the convention
- `range(n)` — produces the numbers 0, 1, 2, ... up to (but not including) n; so `range(5)` gives 5 repetitions
- The **colon** `:` at the end of the `for` line is required
- The **indented lines** below are the code that repeats; Python uses indentation (spaces at the start) to know which lines are inside the loop

### What Is Indentation?

Indentation means adding spaces at the start of a line to show it belongs inside the loop. In Python, the standard is **4 spaces**. If your indentation is wrong, Python will give you an error.

```python
for i in range(3):
    agent.place(DOWN)    # ← indented: inside the loop (repeats 3 times)
    agent.move(FORWARD, 1)  # ← indented: inside the loop (repeats 3 times)
agent.turn(LEFT)         # ← not indented: outside the loop (runs once at the end)
```

---

## Code Example

```python
# Repeat the following 5 times
for i in range(5):
    # Place a block below the agent
    agent.place(DOWN)
    # Move forward 1 block
    agent.move(FORWARD, 1)
```

### What This Code Does

The loop runs 5 times. Each time it runs:
1. The Agent places a block below itself.
2. The Agent moves forward 1 block.

The result is a **5-block path** placed on the floor — using only 3 lines of code instead of 10.

---

## Try It

1. Open Code Builder and switch to the **Python** tab.
2. Type the code above exactly as shown, making sure the two lines inside the loop are indented.
3. Click **Run** and watch the Agent walk forward, placing blocks on the floor.
4. Apply the **Run → Observe → Explain** rule: how many blocks were placed?

---

## Modify It

Try each of these changes. Predict what will happen before you run each version:

1. **Build a longer path** — change `range(5)` to `range(10)`. How many blocks does the Agent place now?
2. **Change direction** — change `FORWARD` to `BACK`. In which direction does the path extend now?
3. **Add a turn inside the loop** — add `agent.turn(LEFT)` as a third indented line inside the loop. What shape does the Agent trace? (Hint: it will be a spiral!)

---

## Challenge

Write a single `for` loop that builds a path of **20 blocks** going forward. Keep your code as short as possible — you should only need 3 lines of code.

---

## Bloom's Taxonomy Check

🧠 **Remember** — What keyword do you use to start a `for` loop in Python?

💡 **Understand** — In your own words, explain what `range(8)` means and how many times the loop will repeat.

🔧 **Apply** — Write a `for` loop that moves the Agent forward 1 block and places a block below it, repeating 7 times.

🔍 **Analyse** — Look at this code. How many total blocks will be placed, and what will the pattern look like?
```python
for i in range(4):
    agent.place(DOWN)
    agent.move(FORWARD, 2)
```

⚖️ **Evaluate** — Compare writing the same instructions 10 times versus using a loop. What are the advantages of using a loop? Can you think of any situation where repeating the code manually might make more sense?

🚀 **Create** — Write a loop that builds a **zigzag path**. The Agent should place a block, move forward, turn, place a block, move forward, and turn back the other way. Use a loop to repeat this pattern 5 times.

---

## Key Vocabulary

| Term | Definition |
|---|---|
| **Loop** | A programming structure that repeats a block of code a set number of times |
| **`for` loop** | A type of loop that repeats for each value produced by `range()` |
| **`range(n)`** | A function that produces the numbers 0 to n−1, causing the loop to repeat n times |
| **Indentation** | Spaces at the start of a line that tell Python which code belongs inside the loop |

---

## What's Next

You can now build straight paths with loops. In the next lesson, you will learn how to use a **loop inside another loop** to build more complex shapes like squares and grids.

➡️ **Next: [Lesson 4 — Nested Loops: Patterns and Shapes](04_nested_loops.md)**
