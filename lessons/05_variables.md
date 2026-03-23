# Lesson 5 — Variables: Storing and Reusing Values

---

## Learning Objectives

By the end of this lesson you will be able to:

- Explain what a variable is and why it is useful
- Create a variable and assign a value to it
- Use a variable inside a loop to control behaviour
- Explain how changing one variable changes the whole program

---

## Theory: What Is a Variable?

Imagine you have a labelled box. You write **"size"** on the outside of the box, and you put the number **6** inside it. Whenever your program needs to know the size, it looks inside the "size" box and uses that number.

A **variable** in Python is exactly that — a named container that holds a value. You can:
- **Create** a variable by writing its name and assigning a value with `=`
- **Use** a variable by writing its name wherever you need the value
- **Change** the value by assigning a new one

### Creating and Using a Variable

```python
size = 6    # Create a variable called 'size' and store the value 6 in it
```

Now whenever Python sees `size` in your code, it uses the number `6`.

### Why Use Variables?

Without variables, if you want to change the size of your square, you have to find and change every single number in the code. With a variable, you change the number **once** at the top, and the whole program updates automatically.

**Without a variable:**
```python
for i in range(4):
    for j in range(6):   # ← change this...
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    agent.turn(LEFT)
```

**With a variable:**
```python
size = 6   # ← change ONLY this — the rest updates automatically
for i in range(4):
    for j in range(size):
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    agent.turn(LEFT)
```

### Naming Variables

Good variable names make your code easier to understand:
- Use lowercase letters and underscores for spaces: `square_width`, `wall_height`
- Make the name describe what the value represents: `size` not `x`
- Avoid single letters (except for loop counters like `i` and `j`)

---

## Code Example

```python
# Store the size of the square in a variable
size = 6

# Use the variable to control the loop
for i in range(4):
    for j in range(size):
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    agent.turn(LEFT)
```

### What This Code Does

1. The variable `size` is set to `6`.
2. The outer loop runs 4 times (once per side of the square).
3. The inner loop uses `size` — so it runs 6 times per side.
4. Each inner loop repetition places a block and moves forward.
5. At the end of each side, the Agent turns left.

The result is a square with sides **6 blocks long**.

---

## Try It

1. Open Code Builder and type the code above.
2. Click **Run** and observe the square the Agent builds.
3. Now change `size = 6` to `size = 3` and run again.
4. Then try `size = 10` and `size = 15`.
5. Apply the **Run → Observe → Explain** rule each time: how does changing `size` change the shape?

---

## Modify It

Try each of these changes:

1. **Change the size** — set `size` to `3`, then `10`, then `15`. Observe how the square changes each time without touching the loop code.
2. **Add a second variable** — create a variable called `sides` and use it in the outer loop: `for i in range(sides):`. Set `sides = 3` and see what shape you get. Try `sides = 6`.
3. **Rename the variable** — rename `size` to `square_width` throughout the code. Does the program still work? Does the new name make the code easier to read?

---

## Challenge

Use **two variables** — one called `size` and one called `sides` — to build different shapes:

- A triangle (3 sides, each 4 blocks long)
- A square (4 sides, each 6 blocks long)
- A hexagon (6 sides, each 4 blocks long)

Write a single program where you only need to change `size` and `sides` at the top to switch between shapes. Test each configuration and check that the shapes look correct.

---

## Bloom's Taxonomy Check

🧠 **Remember** — What symbol do you use in Python to assign a value to a variable?

💡 **Understand** — Explain in your own words why using a variable like `size` is better than writing the number `6` directly into the loop.

🔧 **Apply** — Write a program that uses a variable called `path_length` set to `12` to build a path of that many blocks.

🔍 **Analyse** — Look at this code. What will happen if you change `size = 4` to `size = 7`? List every place in the code that will be affected.
```python
size = 4
for i in range(4):
    for j in range(size):
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    agent.turn(LEFT)
```

⚖️ **Evaluate** — A student writes their code using the number `5` in 8 different places instead of a variable. What problems could this cause? How do variables solve this problem?

🚀 **Create** — Design a program that uses at least **three variables** to control different aspects of a shape — for example, the number of sides, the length of each side, and the block type. Build and test your shape.

---

## Key Vocabulary

| Term | Definition |
|---|---|
| **Variable** | A named container in a program that stores a value |
| **Assignment** | Giving a variable a value using the `=` symbol, e.g. `size = 6` |
| **Value** | The data stored inside a variable, e.g. the number `6` |
| **Flexibility** | The ability to change one variable at the top and have the whole program update |

---

## What's Next

You can now build shapes on a flat floor. In the next lesson you will move into **3D space**, using the `UP` direction to build towers and walls that rise off the ground.

➡️ **Next: [Lesson 6 — Vertical Building: Working in 3D](06_vertical_building.md)**
