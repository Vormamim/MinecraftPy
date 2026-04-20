# Setup for the Website Remix

***

## Why this lesson set is different

The original website teaches Python in Minecraft by connecting normal Python to a Java server with the `mcpi` API and the RaspberryJuice plugin. That setup is not needed for this course.

In this remix you will use:

* **Minecraft Education**
* **Code Builder**
* **MakeCode Python**
* the built-in **Agent**, **player**, **blocks**, and **positions** tools

That means you can learn the same core programming ideas **without external libraries or mods**.

![Programming with Minecraft Python](../.gitbook/assets/ProgrammingWithMineCraftPython.png)

***

## Before you begin

You need:

* Minecraft Education installed
* a flat practice world
* Code Builder working in **Python Only** mode
* coordinates switched on in your world settings if possible

***

## Quick setup steps

1. Open **Minecraft Education**.
2. Create or open a **Flat** world.
3. Press **C** to open **Code Builder**.
4. Choose **New Project**.
5. Set the project type to **Python Only**.
6. Name your project something like `website_remix`.
7. Make sure your **Agent** appears when you run code.

***

## First test program

Run this short snippet to confirm your Minecraft Education tools are working:

```python
agent.teleport_to_player()
agent.move(FORWARD, 2)
agent.turn(LEFT)
agent.move(FORWARD, 2)
```

If the Agent moves in an L-shape, your setup is ready.

***

## How this remix matches the source website

| Original website idea      | Minecraft Education remix                       |
| -------------------------- | ----------------------------------------------- |
| Connect Python to a server | Open Code Builder inside Minecraft Education    |
| `mc.player.getPos()`       | Use in-game coordinates and `player.position()` |
| `mc.setBlock()`            | Use `blocks.place()` and `blocks.fill()`        |
| `mc.postToChat()`          | Use `player.say()` or in-world actions          |
| Plugin-based gameplay      | Built-in classroom-safe tools only              |

***

## Student rule

Every activity in this track uses the same rule:

> **Run → Observe → Explain**

1. Run the code.
2. Watch what happens in the world.
3. Explain what the program did and why.

***

## Challenge check

Change the test program so the Agent makes a **square corner** that is 4 blocks by 3 blocks instead of 2 by 2.

***

## What's next

The original site starts by finding your location and understanding coordinates. In the next lesson, you will do that in Minecraft Education using the built-in position tools.

➡️ **Next:** [Coordinates and Positions](01_coordinates_and_positions.md)
