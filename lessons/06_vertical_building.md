# Lesson 6 — Vertical Building: Working in 3D

---

## Learning Objectives

By the end of this lesson you will be able to:

- Name all 6 directions the Agent can move
- Explain how combining vertical movement with loops creates 3D structures
- Write a loop that builds a tower using the `UP` direction
- Combine a horizontal loop and a vertical loop to build a wall

---

## Theory: Moving in 3D Space

So far, all your Agent's movement has been on a flat surface — left, right, forward, and back. But Minecraft is a **3D world**, which means you can also move **up** and **down**.

The Agent can move in **6 directions**:

| Direction | What It Means |
|---|---|
| `FORWARD` | One block in the direction the Agent is facing |
| `BACK` | One block behind the Agent |
| `LEFT` | One block to the Agent's left |
| `RIGHT` | One block to the Agent's right |
| `UP` | One block upward |
| `DOWN` | One block downward |

### Building Upward

If you place a block below the Agent and then move the Agent **up**, you build a stack. Repeating this in a loop creates a **tower**.

Here is the idea in plain English:

```
Repeat for each level of the tower:
    Place a block below the agent
    Move the agent up 1 block
```

Each repetition adds one block to the stack and moves the Agent up to the next level.

### Building a Wall

A wall is a 3D structure that is both **wide** (horizontal) and **tall** (vertical). To build one, you need **two loops** — one for the width and one for the height. You nest them together:

```
Repeat for each layer of the wall (height):
    Repeat for each block in the row (width):
        Place a block forward
        Move forward
    Move the agent back to the start of the row
    Move the agent up
```

### Why Variables Help in 3D

With variables you can store `height` and `width` at the top of your code and change them instantly. This is even more important in 3D, where structures can become large quickly.

---

## Code Example

```python
# Set the tower height using a variable
height = 5

# Build a tower by moving up and placing blocks
for i in range(height):
    agent.place(DOWN)
    agent.move(UP, 1)
```

### What This Code Does

1. The variable `height` is set to `5`.
2. The loop runs 5 times.
3. Each time: the Agent places a block below itself, then moves up 1 block.
4. The result is a **5-block tower** rising from the ground.

---

## Try It

1. Open Code Builder and type the code above.
2. Click **Run** and look at the Minecraft world — you should see a tower rising up.
3. Step back in Minecraft to get a good view of the tower.
4. Apply the **Run → Observe → Explain** rule: how tall is the tower? Where did the Agent end up?

---

## Modify It

Try each of these changes:

1. **Make a taller tower** — change `height` to `10`. How does the tower change?
2. **Change direction** — replace `agent.move(UP, 1)` with `agent.move(FORWARD, 1)`. What does the Agent build now instead of a tower? How is it different?
3. **Build a wall** — write a program using two nested loops:
   - The **outer** loop controls the height (repeat `height` times).
   - The **inner** loop controls the width (repeat `width` times, placing a block forward and moving forward each time).
   - After the inner loop, move the Agent back to the start of the row and up 1 block.

---

## Challenge

Build a **hollow tower** — a square base that repeats vertically for 5 layers.

Here is the plan:
1. Use your nested loop square code from Lesson 4 to trace a square outline on the floor.
2. Wrap that code in a third outer loop that repeats it `height` times.
3. After each complete square, move the Agent up 1 block before building the next layer.

Use variables for `height` and `size` to control the tower easily.

---

## Bloom's Taxonomy Check

🧠 **Remember** — List all 6 directions the Agent can move in Minecraft.

💡 **Understand** — Explain in your own words why you use `agent.place(DOWN)` before `agent.move(UP, 1)` when building a tower. What would happen if you swapped the order?

🔧 **Apply** — Write a loop that builds a **8-block tall tower** using a variable called `tower_height`.

🔍 **Analyse** — Look at this code. What will the Agent build, and where will it end up after the code runs?
```python
height = 4
width = 6
for layer in range(height):
    for i in range(width):
        agent.place(FORWARD)
        agent.move(FORWARD, 1)
    agent.move(BACK, width)
    agent.move(UP, 1)
```

⚖️ **Evaluate** — Compare building a tower using a loop versus writing out each step individually. What are the advantages and disadvantages of each approach?

🚀 **Create** — Design and build a **pyramid** — a structure where each layer is one block smaller than the one below it. Use variables and loops to control the size. Describe how you would approach this problem before writing the code.

---

## Key Vocabulary

| Term | Definition |
|---|---|
| **3D** | Three-dimensional — having width, depth, and height |
| **`UP` / `DOWN`** | Direction constants that move the Agent vertically |
| **Tower** | A structure built by repeatedly placing a block and moving upward |
| **Layer** | One horizontal level of a 3D structure |

---

## What's Next

You have now combined variables and 3D movement to build real structures. In the next lesson you will learn how to make your program **make decisions** using `if` and `else` conditionals.

➡️ **Next: [Lesson 7 — Conditionals: Making Decisions](07_conditionals.md)**
