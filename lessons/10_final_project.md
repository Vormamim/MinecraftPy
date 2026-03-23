# Lesson 10 — Final Project: Build Your World

---

## Overview

This is your creative final assessment. There is no new code introduced in this lesson. Instead, you will use everything you have learned across all previous lessons to **design and build your own Minecraft structure using Python code**.

This is your chance to be creative, to show what you know, and to build something you are proud of.

---

## Project Requirements

Your finished project **must include all of the following**:

- ✅ At least **2 variables** (used to control size, height, or material)
- ✅ At least **one `for` loop**
- ✅ At least **one nested loop**
- ✅ At least **one `if/else` conditional**
- ✅ At least **one 3D building element** (use of `UP`, `DOWN`, or vertical movement)
- ✅ **Well-commented code** — every section should have a comment explaining what it does

---

## Project Options

Choose **ONE** of the options below, or invent your own idea (see Option D).

### Option A — Path Builder

Build an elaborate multi-directional path across the world.

Ideas to include:
- A path that turns and changes direction multiple times
- Different block materials for different sections (use conditionals)
- A variable that controls how many sections the path has
- A 3D ramp or elevated section (use vertical movement)

### Option B — Square Garden

Build a garden with a clear structure and different zones.

Ideas to include:
- A decorative border around the outside
- A central path down the middle
- A feature in the centre (a pond, a flower bed, a fountain base)
- Different block types for different zones (use conditionals)
- Borders that repeat using loops

### Option C — Tower Builder

Build a multi-story tower with details on each floor.

Ideas to include:
- A variable for the number of floors and the floor size
- Different block materials per floor (use a conditional or the loop variable)
- A flag or decoration at the top
- Windows or gaps on certain walls (use conditionals to skip blocks)

### Option D — Your Own Idea

Design your own structure. Before you start building, answer these questions:

1. What will your structure be? (Name it and describe it)
2. What will it look like? (Sketch it on paper or describe the shape)
3. Which Python concepts will you use, and where?
4. What variables will you need?

---

## Planning Section

Before you write any code, complete these three planning steps:

### Step 1 — Sketch Your Structure

Draw your structure on paper, or describe it in words. Think about:
- What is the shape (square, rectangle, L-shape, etc.)?
- How tall is it?
- Does it have multiple sections or floors?

### Step 2 — Plan Your Python Concepts

Fill in this table before you start coding:

| Python Concept | Where You Will Use It |
|---|---|
| Variable | e.g. `size = 8` to control the floor width |
| `for` loop | e.g. to build each row of the floor |
| Nested loop | e.g. to trace the square outline |
| `if/else` | e.g. to choose block type based on height |
| 3D movement (`UP`/`DOWN`) | e.g. to build each new floor layer |

### Step 3 — Write Pseudocode

Write your program in plain English **before** you write Python. For example:

```
Set size = 8 and height = 5
Load stone blocks into slot 1

Build the floor:
  Repeat 4 times (one per side):
    Repeat size times:
      Place block below, move forward
    Turn left

Build the walls:
  Repeat height times (one per layer):
    Repeat 4 times (one per side):
      Repeat size times:
        Place block forward, move forward
      Turn left
    Move up 1
```

Writing pseudocode first helps you think through the logic before dealing with Python syntax.

---

## Assessment — PowerPoint Presentation

You must create a **PowerPoint presentation** to share your project with the class. Your presentation must include the following slides:

### Slide 1 — Title Slide
- Your project name
- Your name
- The date

### Slide 2 — What I Built
- A screenshot of your finished Minecraft structure
- Or a description of what it looks like if you cannot take a screenshot
- 2–3 sentences describing what your structure is

### Slide 3 — My Code
- A screenshot or copy of your full Python code
- Highlight or circle the most important sections
- Include your comments so the reader can follow what each section does

### Slide 4 — Variables I Used
- List every variable in your code
- Explain what each variable controls
- Explain why you chose the value you used (e.g. "I chose `size = 8` because I wanted a large floor")

### Slide 5 — Loops I Used
- Show where your `for` loop(s) are in your code
- Explain what each loop repeats and how many times
- Explain what would happen if you removed the loop and wrote it out manually

### Slide 6 — Conditionals I Used
- Show your `if/else` statement
- Explain what decision it makes
- Explain what happens in each branch (the `if` case and the `else` case)

### Slide 7 — Bugs I Fixed
- Describe at least **one bug** you encountered while building your project
- Explain what type of error it was (syntax, indentation, or logic)
- Explain how you found it and what you did to fix it

### Slide 8 — What I Learned
- What was the most interesting part of this project?
- What was the most challenging part?
- What is one thing you understand now that you did not understand at the start of the course?

### Slide 9 — What I Would Change
- If you had more time, what would you add or improve?
- Is there a feature you planned but did not manage to build?
- What would the next version of your structure look like?

---

## Bloom's Taxonomy Reflection

Answer one question at each level. You can include these answers in your PowerPoint slides or hand them in separately in writing.

🧠 **Remember** — List every Python concept you used in your project (variables, loops, nested loops, conditionals, 3D movement, etc.).

💡 **Understand** — Explain in your own words what your complete program does. Describe what the Agent does from start to finish.

🔧 **Apply** — Show a specific section of your code where you used a loop. Explain clearly why the loop was needed and what would happen if it was not there.

🔍 **Analyse** — How does your `if/else` conditional statement change the structure that is built? What would the structure look like if you removed the conditional entirely?

⚖️ **Evaluate** — What would happen if you replaced all your variables with the actual numbers (e.g. replacing every `size` with `8`)? What would be the advantages and disadvantages of doing that?

🚀 **Create** — Describe one new feature you would add to your structure if you continued developing it. What Python code would you need to write? How would it change the final result?

---

## Tips for Success

- **Start simple** — build the basic structure first, then add details.
- **Test often** — run your code after each new section and check the result in Minecraft.
- **Use comments** — write a comment above every new section explaining what it does.
- **Debug calmly** — if something goes wrong, read the error message carefully, go to the line it points to, and think about what could be wrong.
- **Be creative** — there is no single right answer. Your structure is yours.

---

## Well Done!

You have completed the Minecraft Education Python course. You have learned:

- How to write and sequence Python commands
- How to place blocks and build structures
- How to use loops to repeat actions efficiently
- How to use nested loops to build 2D and 3D shapes
- How to use variables to make your code flexible
- How to build in 3D using vertical movement
- How to use conditionals to make decisions
- How to find and fix bugs

These are real programming skills that you can use far beyond Minecraft. Keep building, keep coding, and keep creating. 🚀
