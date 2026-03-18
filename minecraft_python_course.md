# Minecraft Education Python Course (10 Hours)
**Beginner Course – In-Game Python Only (MakeCode Python)**

---

## Course Overview

This course introduces students to **basic Python concepts** using the **Minecraft Education Code Builder (MakeCode Python)** environment.

Students will learn:
- Sequencing
- Loops
- Variables
- Conditionals
- Debugging
- Basic computational thinking

---

## Setup (Complete Before Lesson 1)

1. Open **Minecraft Education**
2. Create a **Flat World**
3. Press **C** to open Code Builder
4. Select **MakeCode → Python**
5. Ensure the **Agent** is available

---

## Student Rule

Run code → Observe → Explain what happened

---

# Hour 1 — Sequencing (First Commands)

## Goal
Understand that code runs in order.

## Code
```python
agent.move(FORWARD, 3)
agent.turn(LEFT)
agent.move(FORWARD, 3)
```

## Tasks
- Run the code
- Change `3` to `5`
- Predict the outcome before running

## Challenge
Create an L-shaped path

## Key Concept
Code executes line by line

---

# Hour 2 — Placing Blocks

## Goal
Interact with the world using code

## Code
```python
agent.set_item(STONE, 64, 1)
agent.place(DOWN)
agent.move(FORWARD, 1)
agent.place(DOWN)
```

## Tasks
- Build a path of 5 blocks
- Try different materials (GRASS, WOOD, GLASS)

## Key Concept
Code creates visible changes in the world

---

# Hour 3 — Loops (Repetition)

## Goal
Use loops to reduce repeated code

## Code
```python
for i in range(5):
    agent.place(DOWN)
    agent.move(FORWARD, 1)
```

## Tasks
- Build a 10-block path using a loop

## Key Concept
Loops save time and reduce repetition

---

# Hour 4 — Squares (Nested Loops)

## Goal
Combine loops and movement

## Code
```python
for i in range(4):
    for j in range(5):
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    agent.turn(LEFT)
```

## Tasks
- Build a square
- Change the size (5 → 8)

## Key Concept
Nested loops create patterns

---

# Hour 5 — Variables

## Goal
Control behaviour using variables

## Code
```python
size = 6

for i in range(4):
    for j in range(size):
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    agent.turn(LEFT)
```

## Tasks
- Change `size` to 3, 10, 15

## Key Concept
Variables make code flexible

---

# Hour 6 — Vertical Building

## Goal
Work in 3D space

## Code
```python
height = 5

for i in range(height):
    agent.place(DOWN)
    agent.move(UP, 1)
```

## Tasks
- Build a tower
- Try different heights

## Key Concept
Code can control 3D structures

---

# Hour 7 — Conditionals (IF)

## Goal
Introduce decision-making

## Code
```python
size = 6

if size > 5:
    agent.set_item(GOLD_BLOCK, 64, 1)
else:
    agent.set_item(STONE, 64, 1)

for i in range(size):
    agent.place(DOWN)
    agent.move(FORWARD, 1)
```

## Tasks
- Change `size`
- Observe changes in block type

## Key Concept
Programs can make decisions

---

# Hour 8 — Debugging

## Goal
Identify and fix errors

## Broken Code
```python
for i in range(5)
    agent.move(FORWARD, 1)
```

## Tasks
- Fix syntax errors
- Explain what was wrong

## Common Errors
- Missing brackets
- Incorrect indentation
- Misspelled variables

## Key Concept
Debugging is part of programming

---

# Hour 9 — Guided Project (House Base)

## Goal
Combine all concepts

## Code
```python
size = 6

for i in range(4):
    for j in range(size):
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    agent.turn(LEFT)
```

## Tasks
- Build a square base
- Modify size and materials
- Add walls using vertical loops

---

# Hour 10 — Final Project

## Choose ONE

### Option A
Path Builder

### Option B
Square Garden

### Option C
Tower Builder

---

## Requirements
Your project must include:
- A variable
- A loop
- An IF statement

---

## Reflection Questions

1. What does your code do?
2. What does your variable control?
3. Where did you use a loop?
4. What decision does your IF statement make?
5. What bug did you fix?

---

## Teacher Notes

- Keep lessons practical and visible
- Focus on prediction, testing, and explanation

---

## Course Outcome

By the end of this course, students will:
- Understand basic Python structure
- Apply logic to control a system
- Demonstrate computational thinking in a visual environment
