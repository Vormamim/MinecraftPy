# Lesson 4 — Nested Loops: Patterns and Shapes

---

## Learning Objectives

By the end of this lesson you will be able to:

- Explain what a nested loop is
- Describe how the outer loop and inner loop work together
- Use correct indentation for two levels of loops
- Write a nested loop that builds a square outline

---

## Theory: What Is a Nested Loop?

Think about how you fill in a grid on a piece of paper. For each **row**, you fill in every **column**. So you repeat the "fill a column" action many times, and you repeat the "move to next row" action many times too — one inside the other.

A **nested loop** is a loop that sits inside another loop. The outer loop runs first and controls the bigger repetition. For each single run of the outer loop, the inner loop runs all the way through from start to finish.

Here is the idea in plain English:

```
Repeat 4 times (outer loop — one per side of a square):
    Repeat 5 times (inner loop — place blocks along one side):
        Place a block and move forward
    Turn left (end of one side)
```

When the outer loop runs for the **first** time, the inner loop runs all 5 times. Then the Agent turns left. When the outer loop runs for the **second** time, the inner loop runs all 5 times again. And so on, until the outer loop has run 4 times — completing all 4 sides of a square.

### How Indentation Shows Loop Levels

Each level of nesting adds one more level of indentation:

```python
for i in range(4):          # outer loop — level 1
    for j in range(5):      # inner loop — level 2
        agent.place(DOWN)   # inside inner loop — level 3
        agent.move(FORWARD, 1)
    agent.turn(LEFT)        # inside outer loop, outside inner loop — level 2
```

- `agent.place(DOWN)` and `agent.move(FORWARD, 1)` are indented **8 spaces** (inside both loops — they repeat 4 × 5 = 20 times)
- `agent.turn(LEFT)` is indented **4 spaces** (inside the outer loop only — it repeats 4 times)

### The Loop Variables `i` and `j`

Just as you used `i` in the single loop, you now use `i` for the outer loop and `j` for the inner loop. These are just counter variables — Python increases them by 1 each time their loop repeats.

---

## Code Example

```python
# Repeat 4 times (once per side of a square)
for i in range(4):
    # For each side, place 5 blocks
    for j in range(5):
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    # Turn left at the end of each side
    agent.turn(LEFT)
```

### What This Code Does

- The outer loop runs **4 times** — once for each side of a square.
- The inner loop runs **5 times** for each side — placing 5 blocks and moving forward 5 spaces.
- After each side, the Agent turns left.
- Total blocks placed: **4 × 5 = 20**, forming a square outline.

---

## Try It

1. Open Code Builder and switch to the **Python** tab.
2. Type the code above, paying close attention to indentation — each level is 4 spaces.
3. Click **Run** and watch the Agent trace a square on the ground.
4. Apply the **Run → Observe → Explain** rule: how many sides did the Agent complete? Did the shape close back to the start?

---

## Modify It

Try each of these changes. Always predict the outcome before running:

1. **Make a larger square** — change the inner `range(5)` to `range(8)`. How does the shape change?
2. **Change the shape** — change the outer `range(4)` to `range(3)`. What shape does the Agent trace now? (Hint: think about how many turns you need to complete a triangle.)
3. **Mirror the shape** — change `LEFT` to `RIGHT`. Does the square trace in a different direction? Look carefully at the path.

---

## Challenge

Write a program using nested loops that builds a **rectangle** (not a square). A rectangle has two short sides and two long sides. You will need to think carefully about how to use two different range values.

> 💡 **Hint:** A rectangle has 4 sides, but two sides are longer than the other two. How could you use the outer loop variable `i` to decide whether to build a long side or a short side?

---

## Bloom's Taxonomy Check

🧠 **Remember** — How many times does the inner loop run in total if the outer loop uses `range(4)` and the inner loop uses `range(5)`?

💡 **Understand** — Explain in your own words what `agent.turn(LEFT)` is doing when it is placed inside the outer loop but outside the inner loop.

🔧 **Apply** — Write a nested loop that builds a **3-sided shape** (triangle-like path) with each side being 6 blocks long.

🔍 **Analyse** — Look at this code. Describe step by step what the Agent will do:
```python
for i in range(2):
    for j in range(3):
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    agent.turn(RIGHT)
    agent.move(FORWARD, 1)
```

⚖️ **Evaluate** — Could you build a square without using a nested loop? If yes, write the code. Which version is better? Why?

🚀 **Create** — Design and build a **spiral path** using nested loops or a loop with carefully chosen movements. Test your code and describe the pattern it creates.

---

## Key Vocabulary

| Term | Definition |
|---|---|
| **Nested loop** | A loop that is placed inside another loop |
| **Outer loop** | The loop on the outside; it controls how many times the whole pattern repeats |
| **Inner loop** | The loop on the inside; it runs completely for each single run of the outer loop |
| **Indentation level** | The number of spaces at the start of a line; each nested loop adds one more level (4 more spaces) |

---

## What's Next

Your code now works, but the numbers like `4` and `5` are written directly into the loops. What if you want to easily change the size? In the next lesson you will learn how to use **variables** to store values so you can change them in one place.

➡️ **Next: [Lesson 5 — Variables: Storing and Reusing Values](05_variables.md)**
