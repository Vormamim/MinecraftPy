# Lesson 9 — Guided Project: Building a House Base

---

## Learning Objectives

By the end of this lesson you will be able to:

- Combine sequencing, loops, nested loops, variables, 3D movement, and conditionals in one program
- Explain how each concept contributes to a larger project
- Modify a complete program to change the structure's appearance
- Identify how to extend a flat floor design into 3D walls

---

## Theory: Putting It All Together

You have now learned all the core Python concepts in this course:

| Concept | What It Does in This Project |
|---|---|
| **Sequencing** | Each block of code runs in order — floor first, then walls |
| **Placing blocks** | `agent.set_item()` and `agent.place()` fill the world with blocks |
| **Loops** | Repeat block-placing actions without writing repetitive code |
| **Nested loops** | Build square shapes — one loop per side, one loop per block |
| **Variables** | Store `size` and `wall_height` so you can change the house with one edit |
| **3D movement** | `agent.move(UP, 1)` raises the Agent to build each new wall layer |
| **Conditionals** | Can be used to skip certain blocks (e.g. leave a gap for a door) |

A real program is not just one concept — it is all these concepts working together. This guided project shows you how to combine them to build something meaningful.

### Plan Before You Code

Before writing any code for a large project, it helps to plan:

1. **Describe** what you want to build (a house base with walls).
2. **Break it down** into steps: floor, then walls, then any extra details.
3. **Identify** which Python concepts each step will use.
4. **Write** the code step by step, testing each section as you go.

---

## Code Example

```python
# Set the size of the house base
size = 6

# --- STEP 1: Build the square floor ---
for i in range(4):
    for j in range(size):
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    agent.turn(LEFT)

# --- STEP 2: Build the walls ---
# Set the wall height using a variable
wall_height = 4

# Repeat once per wall layer (moving up each time)
for layer in range(wall_height):
    # Trace the square outline to build all 4 walls
    for i in range(4):
        for j in range(size):
            agent.place(FORWARD)
            agent.move(FORWARD, 1)
        agent.turn(LEFT)
    # Move up one block to begin the next layer
    agent.move(UP, 1)
```

### What Each Section Does

**Step 1 — Floor:**
- The nested loop traces a square outline on the ground.
- The outer loop (4 times) handles each side.
- The inner loop (size times) places blocks along each side.
- The Agent places blocks **below** itself while moving forward.

**Step 2 — Walls:**
- The outermost loop (wall_height times) repeats the square trace for each wall layer.
- Inside it, the same nested loop structure traces the square, but this time places blocks **in front** (FORWARD) to build vertical walls.
- After each complete square trace, the Agent moves up 1 block to start the next layer.

---

## Try It

1. Open Code Builder and type the code above, including the comments.
2. Run **Step 1 only** first — comment out the walls section and check that the floor looks correct.
3. Once the floor works, uncomment the walls section and run the full program.
4. Step back in Minecraft to see the full structure.
5. Apply the **Run → Observe → Explain** rule: does the structure look like a house base with walls?

---

## Modify It

Try each of these changes:

1. **Change the size** — set `size = 8` and `wall_height = 3`. How does the house change? Does it look more like a cottage or a warehouse?
2. **Add a door gap** — inside the wall-building inner loop, use a conditional to skip one block on one wall. For example:
   ```python
   for j in range(size):
       # Leave a gap for the door on the first side of the first layer
       if layer == 0 and i == 0 and j == size // 2:
           agent.move(FORWARD, 1)  # skip placing a block here
       else:
           agent.place(FORWARD)
           agent.move(FORWARD, 1)
   ```
3. **Change the wall material** — add a variable called `wall_material` and use it in `agent.set_item()` to change what the walls are made of. Try `WOOD`, `STONE`, or `GLASS`.

---

## Challenge

Extend the house to include a **roof** — a flat ceiling placed on top of the walls.

To build the roof:
1. After the walls are finished, the Agent should be at the top level.
2. Use the same nested loop square pattern to fill the top completely (not just the outline).
3. This means the inner loop should place a block and move forward, and you need to cover the entire area — think about how to add a second direction to fill the inside row by row.

Use variables to control the size and try to keep your code clean and readable with comments.

---

## Bloom's Taxonomy Check

🧠 **Remember** — Which Python concept is used to make sure the floor is built before the walls in this program?

💡 **Understand** — Explain in your own words why `wall_height` is stored as a variable rather than typing `4` directly into the loop.

🔧 **Apply** — Change the program so that the house is `10` blocks wide and `6` blocks tall. Which two lines do you need to edit?

🔍 **Analyse** — The wall-building section has three levels of loops. Identify which loop controls:
- The number of wall layers
- The number of sides per layer
- The number of blocks per side

⚖️ **Evaluate** — The floor code and the wall code use similar loop structures but place blocks in different directions (`DOWN` vs `FORWARD`). Why does the direction make a difference? What would happen to the structure if you accidentally used the wrong direction?

🚀 **Create** — Design a plan (in writing or as a sketch) for a **more complex structure** — for example, a castle with towers at each corner, or a building with a sloped roof. Which Python concepts would you use for each part? You will build this in the final lesson.

---

## Key Vocabulary

| Term | Definition |
|---|---|
| **Project** | A larger program that combines multiple concepts to achieve a goal |
| **Layer** | One horizontal level of a 3D structure, added by moving the Agent up |
| **Structure** | A 3D object built by placing blocks in a programmed pattern |
| **Pseudocode** | Writing out the steps of a program in plain English before writing actual code |

---

## What's Next

You have completed all the lessons. In the final lesson you will use everything you have learned to design and build your **own Minecraft structure** — and present it as a PowerPoint to show what you have achieved.

➡️ **Next: [Lesson 10 — Final Project: Build Your World](10_final_project.md)**
