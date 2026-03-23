# Lesson 2 — Placing Blocks: Changing the World

---

## Learning Objectives

By the end of this lesson you will be able to:

- Explain what `agent.set_item()` and `agent.place()` do
- Describe what a block slot is and how it works
- Use direction constants such as `DOWN`, `FORWARD`, and `UP`
- Write code that makes the Agent lay a path of blocks

---

## Theory: How Does the Agent Place Blocks?

So far you have moved the Agent around, but it hasn't left any trace in the world. In this lesson you will give the Agent blocks to carry and teach it to place them.

Think of the Agent like a builder carrying a toolbelt. The toolbelt has numbered **slots** (slot 1, slot 2, slot 3, and so on). Each slot can hold a different type of block. Before the Agent can place any blocks, you must:

1. **Load a slot** with a block type and a quantity using `agent.set_item()`.
2. **Tell the Agent to place** a block from its active slot using `agent.place()`.

### `agent.set_item(block_type, quantity, slot)`

This method fills one of the Agent's slots with blocks.

| Parameter | What It Means | Example |
|---|---|---|
| `block_type` | The type of block to load | `STONE`, `GRASS`, `WOOD`, `GLASS` |
| `quantity` | How many blocks to load | `64` (a full stack) |
| `slot` | Which slot number to put them in | `1` |

Example: `agent.set_item(STONE, 64, 1)` — fills slot 1 with 64 stone blocks.

### `agent.place(direction)`

This method places one block from the active slot in the direction you specify.

| Direction | Where the Block Is Placed |
|---|---|
| `DOWN` | Directly below the Agent |
| `FORWARD` | Directly in front of the Agent |
| `UP` | Directly above the Agent |
| `BACK` | Directly behind the Agent |
| `LEFT` | Directly to the left of the Agent |
| `RIGHT` | Directly to the right of the Agent |

### Why Place Blocks Below?

When you use `agent.place(DOWN)` and then move forward, the Agent lays a block on the ground at its current position and then steps onto the next tile. This creates a **path on the floor** — like painting a floor as you walk across it.

---

## Code Example

```python
# Give the agent 64 stone blocks in slot 1
agent.set_item(STONE, 64, 1)
# Place a block below the agent
agent.place(DOWN)
# Move forward 1 block
agent.move(FORWARD, 1)
# Place another block below
agent.place(DOWN)
```

### What This Code Does

1. The Agent loads its slot 1 with 64 stone blocks.
2. It places a stone block on the ground beneath it.
3. It moves forward one block.
4. It places another stone block on the ground at its new position.

The result is **two stone blocks** placed side by side on the floor.

---

## Try It

1. Open Code Builder and switch to the **Python** tab.
2. Type the code above exactly as shown.
3. Click **Run** and look at the ground near the Agent in Minecraft.
4. You should see two stone blocks placed on the floor.
5. Apply the **Run → Observe → Explain** rule: how many blocks were placed, and where?

---

## Modify It

Try each of these challenges. Predict the result before running:

1. **Build a longer path** — extend the code by repeating `agent.place(DOWN)` and `agent.move(FORWARD, 1)` to create a 5-block path.
2. **Swap the block type** — replace `STONE` with `GRASS`, `WOOD`, or `GLASS` and see how the path looks different.
3. **Place blocks in front** — change `agent.place(DOWN)` to `agent.place(FORWARD)`. What happens now? How is the result different?

---

## Challenge

Using only the commands you have learned so far (`agent.set_item()`, `agent.place()`, and `agent.move()`), write a program that builds a **3-block wide path** that is **4 blocks long**.

Think about how you will need to use `agent.turn()` from Lesson 1 to position the Agent correctly for each row.

---

## Bloom's Taxonomy Check

🧠 **Remember** — What are the three parameters in `agent.set_item()`, and what does each one control?

💡 **Understand** — Explain in your own words the difference between `agent.set_item()` and `agent.place()`. Why do you need both?

🔧 **Apply** — Write the code to give the Agent 64 glass blocks in slot 2 and then place one block above the Agent.

🔍 **Analyse** — Look at this code. How many blocks will be placed, and in what pattern?
```python
agent.set_item(WOOD, 64, 1)
agent.place(DOWN)
agent.move(FORWARD, 1)
agent.place(DOWN)
agent.move(FORWARD, 1)
agent.place(DOWN)
```

⚖️ **Evaluate** — What is the advantage of loading 64 blocks at once rather than loading 1 block at a time? Can you think of a situation where loading a smaller quantity might be useful?

🚀 **Create** — Design a program that builds a simple **cross (+) shape** on the floor using stone blocks. Write and test the code.

---

## Key Vocabulary

| Term | Definition |
|---|---|
| **`set_item()`** | A method that loads a block type into one of the Agent's inventory slots |
| **`place()`** | A method that places a block from the Agent's active slot in a given direction |
| **Block slot** | A numbered storage space in the Agent's inventory (slot 1, 2, 3, etc.) |
| **Direction constant** | A keyword like `DOWN`, `FORWARD`, or `UP` that tells the Agent which way to interact with the world |

---

## What's Next

Repeating `agent.place(DOWN)` and `agent.move(FORWARD, 1)` over and over is tedious. In the next lesson you will learn how to use a **loop** to do this automatically.

➡️ **Next: [Lesson 3 — Loops: Doing Things Repeatedly](03_loops.md)**
