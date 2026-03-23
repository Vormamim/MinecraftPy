# Lesson 8 — Debugging: Finding and Fixing Errors

---

## Learning Objectives

By the end of this lesson you will be able to:

- Explain what a bug is and what debugging means
- Identify the 3 most common types of Python errors
- Read an error message and use it to find the problem
- Fix syntax errors, indentation errors, and logic errors in code

---

## Theory: What Is a Bug?

A **bug** is an error in your code that causes it to do the wrong thing — or not run at all. The word "bug" in computing goes back to 1947, when engineers found an actual moth stuck inside a computer causing it to malfunction!

**Debugging** is the process of finding bugs and fixing them. It is not a sign that you are bad at programming — every programmer debugs their code, all the time. Learning to debug well is just as important as learning to write code.

### The 3 Most Common Types of Errors

#### 1. Syntax Errors

A **syntax error** happens when you break Python's grammar rules — for example, forgetting a colon, misspelling a keyword, or missing a bracket.

Python will refuse to run your code at all if there is a syntax error, and it will show you an error message with the line number.

```python
# Bug: missing colon at the end of the for line
for i in range(5)
    agent.move(FORWARD, 1)
```

#### 2. Indentation Errors

An **indentation error** happens when the spaces at the start of a line are wrong — either missing or inconsistent. Python uses indentation to know which code belongs inside a loop or conditional.

```python
# Bug: the code inside the loop is not indented
for i in range(3):
agent.place(DOWN)
agent.move(FORWARD, 1)
```

#### 3. Logic Errors

A **logic error** happens when your code runs without crashing, but it does the **wrong thing**. Python cannot catch these for you — you have to find them by testing and observing.

```python
# Bug: misspelled method name — Python doesn't know what 'moov' is
agent.moov(FORWARD, 2)
```

### Reading Error Messages

When Python finds an error, it shows a message like this:

```
SyntaxError: invalid syntax on line 1
```

The message tells you:
- **What type of error** it is (SyntaxError, IndentationError, NameError, etc.)
- **Which line** the error was found on

Always read error messages carefully — they point you to the exact place where something went wrong.

### The Debugging Process

When your code has an error, follow these steps:

1. **Read** the error message — what type of error is it, and on which line?
2. **Go to** that line in your code and look for the problem.
3. **Fix** the error.
4. **Run** the code again.
5. **Repeat** if there are more errors.

---

## Broken Code to Fix

Below are three snippets of broken code. For each one, try to **spot the bug before running it**, then run it to see the error message, and finally fix it.

### Bug 1 — Missing Colon

```python
# Bug 1 – missing colon
for i in range(5)
    agent.move(FORWARD, 1)
```

> What is wrong? The `for` line is missing a `:` at the end.

### Bug 2 — Wrong Indentation

```python
# Bug 2 – wrong indentation
for i in range(3):
agent.place(DOWN)
agent.move(FORWARD, 1)
```

> What is wrong? The two lines inside the loop are not indented — Python does not know they belong to the loop.

### Bug 3 — Misspelled Method

```python
# Bug 3 – misspelled method
agent.moov(FORWARD, 2)
```

> What is wrong? `moov` is not a valid method — the correct spelling is `move`.

---

## Try It

1. Open Code Builder and type each broken snippet one at a time.
2. Click **Run** for each one and read the error message carefully.
3. Note which line the error is on and what type of error Python reports.
4. Apply the **Run → Observe → Explain** rule: what does the error message tell you?

---

## Modify It

1. **Fix each bug** — correct all three broken snippets and add a comment above each fix explaining what was wrong. For example:
   ```python
   # Fixed: added missing colon at end of for statement
   for i in range(5):
       agent.move(FORWARD, 1)
   ```
2. **Introduce a logic error** — write a working program but deliberately change a direction or number so the Agent does the wrong thing (for example, use `UP` instead of `FORWARD`). Run it and describe what went wrong in a comment.
3. **Read more error messages** — try deleting the brackets from `range(5)` and see what error you get. Try writing `IF` (capital letters) instead of `if`. Read each error message and explain what it means.

---

## Challenge

Write a short program (about 6–10 lines) that contains **3 intentional bugs** — at least one syntax error, one indentation error, and one logic error. Swap your broken code with a classmate. Each of you should:

1. Find and fix all 3 bugs in your classmate's code.
2. Add comments explaining what each bug was and how you fixed it.
3. Run the fixed code to verify it works correctly.

---

## Bloom's Taxonomy Check

🧠 **Remember** — What are the names of the 3 most common types of Python errors covered in this lesson?

💡 **Understand** — Explain in your own words the difference between a syntax error and a logic error. Which one is harder to find? Why?

🔧 **Apply** — Look at this code and identify the bug. Write the corrected version:
```python
size = 5
if size > 3
    agent.set_item(GOLD_BLOCK, 64, 1)
```

🔍 **Analyse** — A student's program runs without any error messages, but the Agent builds the path backwards. What type of error is this? How would you go about finding and fixing it?

⚖️ **Evaluate** — Why is it useful to read error messages carefully rather than just changing random parts of the code until it works? What are the risks of the "trial and error without reading" approach?

🚀 **Create** — Write a debugging guide (5–10 bullet points) that you could give to a student who is seeing a Python error for the first time. What steps should they follow? What should they look for?

---

## Key Vocabulary

| Term | Definition |
|---|---|
| **Bug** | An error in a program that causes it to behave incorrectly |
| **Debugging** | The process of finding and fixing bugs in a program |
| **Syntax error** | An error caused by breaking Python's grammar rules, such as a missing colon or bracket |
| **Indentation error** | An error caused by incorrect or missing indentation inside a loop or conditional |
| **Logic error** | An error where the code runs without crashing but produces the wrong result |

---

## What's Next

You can now write and fix Python code confidently. In the next lesson you will bring together everything you have learned to build a complete guided project — a house base — using sequencing, loops, variables, 3D movement, and conditionals all at once.

➡️ **Next: [Lesson 9 — Guided Project: Building a House Base](09_guided_project.md)**
