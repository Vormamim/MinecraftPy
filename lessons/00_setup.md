---
icon: pickaxe
---

# Getting Started with Minecraft Education & Code Builder

Welcome! Before you write your first line of Python, you need to get your workspace ready. This guide walks you through everything you need to do to set up Minecraft Education and the Code Builder so you can start programming straight away.

***

## What You Will Need

* **Minecraft Education** installed on your device
* A school email address to sign in
* A blank Word Doc called **firstName\_Surname\_MinecraftPython** (you'll use this later)
* A flat world (you will create this below)

***

## Step-by-Step Setup

### Step 1 — Open Minecraft Education

1. Find the **Minecraft Education** icon on your desktop or in your apps list.
2. Double-click to open it.
3. Sign in with your Microsoft account if prompted.

### Step 2 — Create a Flat World

A flat world gives you a blank, level surface to build on — perfect for coding projects.

1. On the home screen, click **Play**.
2. Click **Create New World**.
3. Select the world type from <mark style="background-color:$success;">**Advanced**</mark>
4. Under **World Type**, select **Flat**
5. Give your world a name (e.g. _My Python World_).
6. Click **Play** to enter the world.

> 💡 **Tip:** A flat world removes hills and obstacles so your agent can move freely without getting stuck.

### Step 3 — Open Code Builder

Once you are inside your world:

1. Press the **C** key on your keyboard. The Code Builder panel will open on the right side of the screen.
2. If **C** does not work, look for the **Code Builder** icon in the toolbar at the top of the screen and click it.

### Step 4 — Select MakeCode → Python

<figure><img src="../.gitbook/assets/Screenshot 2026-03-24 103344.png" alt=""><figcaption></figcaption></figure>

1. In the Code Builder panel, click **New Project**.
2. Give your Code Project a name **helloMyWord**
3. From the drop down menu - select **Python Only**
4. Press **Create**
5. The first time, you must take the **Welcome! Editor Tour**
6. A new editor will open. At the top, you will see tabs for **Blocks** and **Python**.
7. Click the **Python** tab to <mark style="background-color:$success;">**switch to text-based Python coding.**</mark>

<figure><img src="../.gitbook/assets/Screenshot 2026-03-24 103535.png" alt=""><figcaption></figcaption></figure>

> 💡 **Tip:** If you accidentally switch to Blocks view, just click the Python drop down to change it. **We are not interested in using block code** for developing Python code.

### Step 5 — Find and Use the Agent

The **Agent** is your programmable helper inside Minecraft. It is a small robot that appears in your world and follows your Python instructions.

1. In the Code Builder Python editor, type a short command (e.g. `agent.move(FORWARD, 1)`) and click **Run**.
2. Look around in your Minecraft world — you should see the Agent appear and move.
3. If the Agent is not visible, walk around your spawn point; it usually appears nearby.

<figure><img src="../.gitbook/assets/Screenshot 2026-03-24 104223.png" alt=""><figcaption></figcaption></figure>

> 💡 **Tip:** If the Agent is stuck inside a block or they have gone missing, you can teleport it to you using the chat command. Open the chat and use the command for for teleport <mark style="background-color:$warning;">**'/teleport @c @s'**</mark> which means <mark style="background-color:$primary;">**teleport the agent (c) to myself (s)**</mark> and your robot will show up if you look around. It's easy to loose your Agent and sometimes.

***

## What Is the Agent?

The Agent is a programmable robot you control entirely through Python code. It can:

* **Move** in any of 6 directions: forward, back, left, right, up, and down
* **Place blocks** from its inventory into the world
* **Destroy blocks** in the world
* **Turn** left or right to change direction

<mark style="background-color:orange;">**You will use the Agent in every lesson in this course.**</mark>

***

## What Is MakeCode Python?

**MakeCode Python** is a beginner-friendly version of Python designed to work inside Minecraft Education. Here is how it compares to standard Python:

| Feature          | MakeCode Python                        | Standard Python            |
| ---------------- | -------------------------------------- | -------------------------- |
| Where it runs    | Inside Minecraft Education             | On your computer or online |
| Special commands | `agent.move()`, `agent.place()`, etc.  | No Minecraft commands      |
| Output           | You see changes in the Minecraft world | Text output in a terminal  |
| Complexity       | Simplified for beginners               | Full professional language |

In this course you will use **MakeCode Python** exclusively. Everything you learn here — sequencing, loops, variables, and conditionals — is real Python that you can take into other projects later.

***

## Navigating the Code Builder Interface

Here are the key parts of the Code Builder you will use:

| Part             | What It Does                                    |
| ---------------- | ----------------------------------------------- |
| **Code area**    | Where you type your Python code                 |
| **Run button**   | Sends your code to Minecraft and executes it    |
| **Stop button**  | Stops the code if it is running                 |
| **Reset button** | Resets the Agent back to its starting position  |
| **Error panel**  | Shows error messages if your code has a problem |

> 💡 **Tip:** Always read error messages carefully — they tell you exactly what went wrong and on which line.

***

## 📌 Student Rule

Every time you write code in this course, follow this three-step rule:

> **Run → Observe → Explain**
>
> 1. **Run** your code and watch what happens in Minecraft.
> 2. **Observe** the result carefully — what did the Agent do?
> 3. **Explain** what happened in your own words.

This habit will help you understand your code deeply, not just copy it.

***

## Troubleshooting Tips

| Problem                       | What to Try                                                            |
| ----------------------------- | ---------------------------------------------------------------------- |
| Code Builder won't open       | Make sure you are inside a world, then press **C**                     |
| Agent doesn't appear          | Run `/agent teleport` in the chat                                      |
| Code runs but nothing happens | Check that you are in the Python tab, not the Blocks tab               |
| Error message appears         | Read the message, find the line number, check spelling and punctuation |
| World is not flat             | Create a new world and choose **Flat** as the world type               |

***

## You Are Ready!

Once you can see the Code Builder in Python mode and your Agent is visible in the world, you are all set. Head to **Lesson 1 — Sequencing** to write your first commands.

➡️ **Next:** [**Lesson 1 — Sequencing: Your First Commands**](01_sequencing.md)
