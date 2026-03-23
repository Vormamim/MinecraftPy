# Lesson 1 — Sequencing: Your First Commands

---

## Learning Objectives

By the end of this lesson you will be able to:

- Explain what sequencing means in programming
- Predict the order in which lines of code will run
- Write a short Python program that moves the Agent in a specific pattern
- Modify a sequence of commands to produce a different path

---

## Theory: What Is Sequencing?

Imagine you are following a recipe to make a sandwich. You spread the butter *before* you add the filling. You add the filling *before* you close the bread. Each step happens in a specific order — and if you do them in the wrong order, the sandwich goes wrong.

**Sequencing** in programming works exactly the same way. When you write a Python program, the computer reads each line from **top to bottom**, one at a time, and carries out each instruction before moving to the next.

This means:
- The **first line** runs first.
- The **second line** runs second.
- And so on, all the way to the last line.

If you put your instructions in the wrong order, your program will do the wrong thing — just like making the sandwich in the wrong order.

### Why Does Order Matter?

Consider these two programs:

```python
# Program A
agent.turn(LEFT)
agent.move(FORWARD, 3)
```

```python
# Program B
agent.move(FORWARD, 3)
agent.turn(LEFT)
```

Both programs contain the same two lines, but because the order is different, the Agent ends up in a completely different place. **Order is everything in sequencing.**

---

## Code Example

```python
# Move the agent forward 3 blocks
agent.move(FORWARD, 3)
# Turn the agent left
agent.turn(LEFT)
# Move the agent forward 3 more blocks
agent.move(FORWARD, 3)
```

### What Each Line Does

| Line | What It Does |
|---|---|
| `agent.move(FORWARD, 3)` | Moves the Agent 3 blocks in the direction it is currently facing |
| `agent.turn(LEFT)` | Rotates the Agent 90 degrees to the left (it does not move, just turns) |
| `agent.move(FORWARD, 3)` | Moves the Agent 3 blocks in its new facing direction |

The Agent traces an **L-shaped path** — 3 blocks one way, then 3 blocks in a new direction.

---

## Try It

1. Open Code Builder in Minecraft Education (press **C**).
2. Make sure you are in the **Python** tab.
3. Type the code above exactly as shown.
4. Click **Run** and watch your Agent in the Minecraft world.
5. Follow the **Run → Observe → Explain** rule: what path did the Agent trace?

---

## Modify It

Try each of these changes one at a time. Before you run each version, **predict** what you think will happen:

1. **Change the distance** — replace both `3`s with `5`. What path does the Agent trace now?
2. **Make a Z-shape** — after the second `agent.move(FORWARD, 3)`, add `agent.turn(LEFT)` and then `agent.move(FORWARD, 3)`. What letter does this trace?
3. **Change direction** — replace `LEFT` with `RIGHT`. How does the path change compared to the original?

---

## Challenge

Write a program that makes the Agent trace an **L-shaped path** where:
- The long part of the L is **6 blocks**
- The short part of the L is **3 blocks**
- The Agent turns **right** (not left)

Write your code, run it, and check that the path looks correct.

---

## Bloom's Taxonomy Check

Work through these questions to check your understanding. Write your answers in your notebook or discuss them with a partner.

🧠 **Remember** — What direction does Python read and execute the lines of a program?

💡 **Understand** — In your own words, explain why the order of `agent.move()` and `agent.turn()` matters.

🔧 **Apply** — Write three lines of code that move the Agent forward 4 blocks, then turn right, then move forward 2 blocks.

🔍 **Analyse** — Look at this code. What will the Agent do, and where will it end up compared to where it started?
```python
agent.turn(LEFT)
agent.turn(LEFT)
agent.move(FORWARD, 5)
```

⚖️ **Evaluate** — Why is sequencing a useful concept even in everyday life? Give one real-world example where doing things in the wrong order causes a problem.

🚀 **Create** — Design a sequence of Agent commands that traces the letter **T** on the ground. Write the code and test it.

---

## Key Vocabulary

| Term | Definition |
|---|---|
| **Sequencing** | Running instructions one after another in a specific order |
| **Method** | A command you give to the Agent, e.g. `agent.move()` or `agent.turn()` |
| **Argument** | The value inside the brackets that tells the method what to do, e.g. `FORWARD` or `3` |
| **Execution** | The process of the computer carrying out your code instructions |

---

## What's Next

Now that you can move the Agent in a sequence, the next lesson will teach you how to make it **place blocks** as it moves, so you can build things in the Minecraft world.

➡️ **Next: [Lesson 2 — Placing Blocks: Changing the World](02_placing_blocks.md)**
