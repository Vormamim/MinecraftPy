# MinecraftPy — Teacher Lesson Plans

**Course:** Beginner Python with Minecraft Education (MakeCode Python)
**Total Duration:** 20 hours (20 × 1-hour sessions)
**Year Level:** Stage 4 (Years 7–8)

---

## Curriculum Outcomes

| Code | Outcome |
|---|---|
| **TE4-DIG-01** | Demonstrates technological literacy to safely interact in digital environments |
| **TE4-DIG-02** | Uses data and digital systems to code, design and produce projects |

All 20 lesson plans below are designed to address **both outcomes** concurrently. TE4-DIG-01 is foregrounded in the setup and digital citizenship moments embedded throughout each lesson. TE4-DIG-02 is the primary driver of all coding and project work.

---

## Course Structure at a Glance

| Hour | Topic | Student File | Focus Outcome |
|---|---|---|---|
| 1 | Getting Started: Setup & Digital Environment | `00_setup.md` | TE4-DIG-01, TE4-DIG-02 |
| 2 | Sequencing — Core Concepts | `01_sequencing.md` | TE4-DIG-02 |
| 3 | Sequencing — Practice & Extension | `01_sequencing.md` | TE4-DIG-02 |
| 4 | Placing Blocks — Core Concepts | `02_placing_blocks.md` | TE4-DIG-02 |
| 5 | Placing Blocks — Practice & Extension | `02_placing_blocks.md` | TE4-DIG-02 |
| 6 | Loops — Core Concepts | `03_loops.md` | TE4-DIG-02 |
| 7 | Loops — Practice & Extension | `03_loops.md` | TE4-DIG-02 |
| 8 | Nested Loops — Core Concepts | `04_nested_loops.md` | TE4-DIG-02 |
| 9 | Nested Loops — Practice & Extension | `04_nested_loops.md` | TE4-DIG-02 |
| 10 | Variables — Concepts & Practice | `05_variables.md` | TE4-DIG-02 |
| 11 | Mid-Course Consolidation & Review | — | TE4-DIG-01, TE4-DIG-02 |
| 12 | Vertical Building — Core Concepts | `06_vertical_building.md` | TE4-DIG-02 |
| 13 | Vertical Building — Practice & Extension | `06_vertical_building.md` | TE4-DIG-02 |
| 14 | Conditionals — Core Concepts | `07_conditionals.md` | TE4-DIG-02 |
| 15 | Conditionals — Practice & Extension | `07_conditionals.md` | TE4-DIG-02 |
| 16 | Debugging — Concepts & Practice | `08_debugging.md` | TE4-DIG-01, TE4-DIG-02 |
| 17 | Debugging — Peer Review & Extension | `08_debugging.md` | TE4-DIG-01, TE4-DIG-02 |
| 18 | Guided Project — Planning & Start | `09_guided_project.md` | TE4-DIG-02 |
| 19 | Guided Project — Build & Refine | `09_guided_project.md` | TE4-DIG-02 |
| 20 | Final Project — Design, Build & Present | `10_final_project.md` | TE4-DIG-01, TE4-DIG-02 |

---

## Lesson Plan 1 — Getting Started: Setup & Digital Environment

**Duration:** 1 hour
**Student File:** `00_setup.md`
**Outcomes:** TE4-DIG-01, TE4-DIG-02

### Learning Intentions
- Students can open Minecraft Education, sign in with their school account, and create a flat world.
- Students can navigate the Code Builder interface and locate the Python editor.
- Students understand and can describe appropriate and safe use of the school digital environment.

### Resources
- Devices with Minecraft Education installed and licensed
- School Microsoft/Google accounts active for each student
- Student tracking document template (Word/Google Doc)

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Welcome and context-setting. Introduce the course purpose and the student rule: Run → Observe → Explain. | Establish expectations for the digital environment — appropriate use of school accounts, keeping work in OneDrive/Google Drive, not modifying other students' worlds. Address TE4-DIG-01. |
| 5–15 min | Guide the class through Steps 1–3 of the setup (open app, sign in, create flat world, open Code Builder). | Circulate and assist with login issues. Confirm all students are inside a flat world with Code Builder open. Flag any devices with software or licence issues. |
| 15–35 min | Guide the class through Steps 4–5 (select Python mode, locate the Agent, run a first command). | Monitor that all students are in Python tab (not Blocks). Watch for students who cannot see their Agent — prompt the teleport command. Reinforce the Code Builder interface orientation. |
| 35–50 min | Students create their personal Word/Google Doc named `firstName_Surname_MinecraftPython` and save it to their OneDrive/Google Drive. Students explore freely — trying to move the Agent in different directions. | Confirm document naming and save location. Circulate and note which students are confidently experimenting and which are hesitant. This is a formative baseline observation. |
| 50–60 min | Class debrief. Ask 2–3 students to share what they discovered about Agent movement. Summarise the Code Builder interface. | Reinforce: digital citizenship — files stay in personal drives, accounts are for school use only. Preview next lesson. |

### Teacher Notes
- Licence or account failures must be resolved in the first 10 minutes — have IT support contact details ready.
- Some students will attempt to use Blocks mode out of familiarity; redirect them to Python mode firmly but positively.
- The teleport command (`/teleport @c @s`) should be written on the board for reference throughout the course.
- TE4-DIG-01 is best addressed here explicitly — the lesson opens a genuine conversation about safe, responsible use of school accounts and digital environments.

### Differentiation
- **Support:** Pair with a stronger peer for the setup steps; provide a printed step-by-step guide.
- **Extension:** Challenge to discover and name all 6 Agent movement directions before they are formally taught.

---

## Lesson Plan 2 — Sequencing: Core Concepts

**Duration:** 1 hour
**Student File:** `01_sequencing.md` (Theory, Code Example, Try It sections)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can explain what sequencing means in the context of programming.
- Students can predict what a short sequence of Agent commands will do before running it.
- Students can write and run a simple sequence that produces an L-shaped path.

### Resources
- Devices with Minecraft Education open (flat world + Code Builder)

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Review the Run → Observe → Explain rule. Ask: "What would happen if you put on your shoes before your socks?" Connect to sequencing. | Frame the concept before students open code. |
| 5–15 min | Introduce sequencing theory verbally with a worked example on the board (two programs showing different orders of `move` and `turn`). Do not restate the student theory section; use it as your reference. | Emphasise that Python reads top-to-bottom. Draw a simple flowchart showing line-by-line execution. |
| 15–40 min | Students type and run the code example. Students then complete the **Modify It** task (change the distance, make a Z-shape, change direction). | Circulate continuously. Check: Are students predicting before running? Prompt: "Before you click Run, what do you think the Agent will do?" Note students who are predicting accurately vs. running first and observing. |
| 40–55 min | Students begin the **Challenge** (L-shaped path with specific dimensions and a right turn). | Provide a hint if needed: "How many `move` and `turn` commands do you need?" |
| 55–60 min | Class share-out: 2–3 students describe their L-shaped path in words. | Reinforce vocabulary: sequence, execution, argument. |

### Teacher Notes
- The core misconception here is that students believe the direction `FORWARD` is always north — it is relative to the Agent's facing direction. Clarify this when circulating.
- The predict-before-run habit is essential to build now; it is the foundation of computational thinking across the rest of the course.

### Differentiation
- **Support:** Limit to the basic code example and one modification.
- **Extension:** Ask students to work through the Bloom's Taxonomy **Analyse** and **Create** questions in their tracking document.

---

## Lesson Plan 3 — Sequencing: Practice & Extension

**Duration:** 1 hour
**Student File:** `01_sequencing.md` (Questions, Challenge, extension)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can answer higher-order questions about sequencing in their tracking document.
- Students can design and test a sequence of commands that traces a letter shape.

### Resources
- Devices with Minecraft Education open
- Student tracking documents

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Quick review: ask a student to explain sequencing in one sentence. | Gauge retention from last lesson. |
| 5–20 min | Students respond to the **Remember**, **Understand**, and **Apply** questions in their tracking document. | Circulate and read responses. Use this as a formative check for comprehension before moving to higher-order tasks. |
| 20–45 min | Students work on the **Analyse**, **Evaluate**, and **Create** questions. The Create task (tracing a letter T) requires active coding. | Support students moving from written questions to code. Watch for students who write the code first without planning. Prompt: "Sketch the T on paper first." |
| 45–57 min | Students who finish early are invited to trace other letters using only `move` and `turn`. | This is open-ended extension — note which students demonstrate creative application without prompting. |
| 57–60 min | Checkpoint: students save their tracking document. Confirm files are saved to OneDrive/Google Drive. | TE4-DIG-01 moment — reinforce digital file management habits. |

### Teacher Notes
- This lesson deepens the same content. Avoid moving on to Lesson 2 material if students are still consolidating sequencing.
- Students who are confident should be encouraged to extend, not race ahead to the next topic.

### Differentiation
- **Support:** Focus on Remember, Understand, Apply questions only. Written code answers may be substituted with verbal explanation to teacher.
- **Extension:** Trace the letter of the student's first name using only `move` and `turn`.

---

## Lesson Plan 4 — Placing Blocks: Core Concepts

**Duration:** 1 hour
**Student File:** `02_placing_blocks.md` (Theory, Code Example, Try It sections)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can explain the purpose of `set_item()` and `place()` and describe each parameter.
- Students can write code that loads a block type and places it in a specified direction.
- Students can build a path of blocks by combining move and place commands.

### Resources
- Devices with Minecraft Education open

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Quick recall: ask students to name the previous concept. Ask: "What does the Agent leave behind when it moves?" (Answer: nothing, yet.) Connect to motivation for placing blocks. | |
| 5–15 min | Teacher-led explanation of the Agent's inventory slots, `set_item()`, and `place()`. Use a physical analogy: "Think of each slot like a labelled paint tin." | Focus on the 3 parameters of `set_item()` and the direction constants for `place()`. |
| 15–40 min | Students type and run the code example. Students then attempt **Modify It** tasks 1 (longer path) and 2 (different materials). | Monitor that students are loading blocks with `set_item()` before calling `place()`. A common mistake is to call `place()` without loading anything first. |
| 40–55 min | Students attempt **Modify It** task 3 (change `DOWN` to `FORWARD`) and describe the difference. | Ask: "What direction is the block placed now?" Reinforce conceptual understanding of the direction constants. |
| 55–60 min | Class debrief: students share observations about placing forward vs. placing down. | |

### Teacher Notes
- Students will likely run out of blocks mid-task if they forget to reload. This is a good learning moment: "What happened? How would you fix it?"
- Some students may notice the Agent must move to avoid placing blocks on top of each other — this is part of understanding how the Agent interacts with the 3D world.

### Differentiation
- **Support:** Reduce to one block type; focus on a 3-block path only.
- **Extension:** Attempt the full Challenge (3-block-wide, 4-block-long path) at the end of the lesson.

---

## Lesson Plan 5 — Placing Blocks: Practice & Extension

**Duration:** 1 hour
**Student File:** `02_placing_blocks.md` (Challenge, Bloom's questions)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can combine movement, turning, and block placement to build a multi-row path.
- Students can articulate the difference between `set_item()` and `place()` in writing.

### Resources
- Devices with Minecraft Education open
- Student tracking documents

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Review the three parameters of `set_item()`. Ask a student to demonstrate loading the Agent with stone blocks. | |
| 5–25 min | Students complete the **Challenge** (3-wide × 4-long path). Students may need to plan on paper first. | Prompt planning: "How many rows? How many blocks per row? How will you move to the next row?" This is a key scaffolding moment. |
| 25–50 min | Students respond to Bloom's **Remember**, **Understand**, and **Apply** questions in their tracking document. **Analyse** question may be done in code before writing the answer. | Monitor written responses. Look for depth of explanation in Understand responses. |
| 50–58 min | **Create** extension: design a cross-shaped path on the floor. Students who reach this point should be noted as working above expected level. | |
| 58–60 min | Save tracking documents. Preview: "Next lesson we learn how to stop writing the same line over and over." | Build anticipation for loops. |

### Teacher Notes
- The Challenge requires planning — students who jump straight to code without sketching a plan often produce incorrect results and feel frustrated. Scaffold planning explicitly.

### Differentiation
- **Support:** Provide a partially completed Challenge template showing the first row.
- **Extension:** Bloom's **Evaluate** and **Create** questions.

---

## Lesson Plan 6 — Loops: Core Concepts

**Duration:** 1 hour
**Student File:** `03_loops.md` (Theory, Code Example, Try It sections)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can explain what a `for` loop does and why it is useful.
- Students can read and write a `for` loop using `range()` with correct indentation.
- Students can use a loop to build a path of blocks without repeating code manually.

### Resources
- Devices with Minecraft Education open

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Pose the problem: "I want you to write code to place 20 blocks in a row. How many lines will you need?" Take answers, then reveal: "What if I told you it only takes 3?" | Create cognitive dissonance to motivate the concept. |
| 5–15 min | Teacher-led explanation of the `for` loop structure: `for i in range(n):` and indentation. Write one example on the board. Compare with and without a loop (20 vs. 3 lines). | Emphasise the colon and the 4-space indent. These are the two most common syntax errors for this lesson. |
| 15–45 min | Students type and run the code example. Students then complete **Modify It** tasks (longer path, change direction, add a turn inside the loop). | Monitor indentation closely — circulate and ask students to point to the code inside the loop vs. outside it. The spiral modification is intentionally surprising; encourage students to explain it. |
| 45–57 min | Students begin the **Challenge** (20-block path in 3 lines). | Verify students are using a loop with `range(20)`, not 20 separate lines. |
| 57–60 min | Debrief: "How does the loop work? What does `range(5)` give us?" | Consolidate vocabulary. |

### Teacher Notes
- The most common error is incorrect indentation — either no indent, or inconsistent indent. Reinforce that Python uses 4 spaces (not a tab, depending on editor settings in MakeCode).
- The loop variable `i` often confuses students who ask "what does `i` do?" — explain it is a counter that increases automatically, and they do not need to use it in the code body yet.

### Differentiation
- **Support:** Provide a loop template with the colon and indent pre-marked. Focus on changing only the `range()` value.
- **Extension:** Explore what happens when `range(n)` is changed to `range(1, 10)` — introduce start and end values (beyond the lesson scope, but an excellent stretch).

---

## Lesson Plan 7 — Loops: Practice & Extension

**Duration:** 1 hour
**Student File:** `03_loops.md` (Challenge, Bloom's questions)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can explain loop behaviour at the Understand and Analyse levels.
- Students can predict loop output and verify predictions by running code.

### Resources
- Devices with Minecraft Education open
- Student tracking documents

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Quick check: ask a student to read a loop aloud and say how many times it runs. | |
| 5–20 min | Students complete the **Remember**, **Understand**, and **Apply** Bloom's questions in their tracking document. | Look for students who struggle with the Understand question (explaining `range(8)` in their own words). These students may need one-on-one clarification. |
| 20–45 min | Students attempt the **Analyse** question (count blocks placed in a given loop) and verify by running it in Minecraft. Then complete the **Evaluate** question in writing. | The Evaluate question asks about advantages of loops vs. manual repetition — look for students who articulate efficiency and maintainability. |
| 45–57 min | Students attempt the **Create** question: a zigzag path using a loop. | This requires turning within a loop — students need to think about how direction changes compound over repetitions. |
| 57–60 min | Save tracking documents. | |

### Teacher Notes
- The zigzag Create task is cognitively demanding. Prompt students to "predict on paper first: after 2 repetitions, which direction is the Agent facing?"
- Students who are finding loops intuitive may be given the spiral challenge from the Modify section as additional extension.

### Differentiation
- **Support:** Remove the Create task; focus on the first three Bloom's levels only.
- **Extension:** Write a loop that builds a staircase (move forward and up each step).

---

## Lesson Plan 8 — Nested Loops: Core Concepts

**Duration:** 1 hour
**Student File:** `04_nested_loops.md` (Theory, Code Example, Try It sections)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can explain what a nested loop is using a concrete analogy.
- Students can read a nested loop and calculate how many total iterations occur.
- Students can write a nested loop with correct two-level indentation that builds a square.

### Resources
- Devices with Minecraft Education open

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Connect prior knowledge: "You can build a row with one loop. How would you build four rows?" Take student ideas. | |
| 5–15 min | Teacher-led explanation of nested loop structure using a grid analogy (rows and columns). Show the indentation levels on the board: outer = 4 spaces, inner body = 8 spaces, outer body after inner = 4 spaces. | Write a skeleton nested loop on the board and ask students to fill in the missing parts as a class. |
| 15–45 min | Students type and run the square code example. Students complete **Modify It** tasks (larger square, change to triangle, mirror direction). | After the larger square, ask: "How many total blocks were placed?" — reinforce multiplication of iterations (outer × inner). Monitor two-level indentation carefully; this is the most error-prone aspect. |
| 45–57 min | Students begin the **Challenge** (rectangle with different side lengths). | Prompt: "A rectangle has two pairs of equal sides. How can the loop variable `i` tell you which type of side you are building?" |
| 57–60 min | Debrief: ask students to describe outer vs. inner loop in one sentence each. | |

### Teacher Notes
- Students often accidentally indent the `agent.turn(LEFT)` inside the inner loop. The result is the Agent turns on every block rather than at the end of each side. Ask students to predict what the difference would be before correcting.
- The rectangle challenge is intentionally open-ended — the most elegant solution uses the `i` variable in a conditional, which previews a future lesson.

### Differentiation
- **Support:** Trace through the loop on paper step by step (iteration by iteration) before touching the computer.
- **Extension:** The **Analyse** Bloom's question (in the next lesson) requires careful nested loop tracing — introduce it here for advanced students.

---

## Lesson Plan 9 — Nested Loops: Practice & Extension

**Duration:** 1 hour
**Student File:** `04_nested_loops.md` (Challenge, Bloom's questions)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can trace a nested loop step by step and predict its output.
- Students can evaluate the advantage of nested loops over manually written code.

### Resources
- Devices with Minecraft Education open
- Student tracking documents

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Warm up: write a nested loop on the board and ask students to state how many total times the body runs. | |
| 5–25 min | Students complete **Remember**, **Understand**, and **Apply** Bloom's questions in their tracking documents. | Check that Apply responses (3-sided shape with 6-block sides) use correct loop ranges and indentation. |
| 25–50 min | Students complete the **Analyse** question (tracing the given code step by step and describing the result) and the **Evaluate** question (compare with manually written code). | This is the deepest analytical work in the lesson. Support by asking guiding questions: "What happens on the first run of the outer loop? On the second?" |
| 50–57 min | Students attempt the **Create** question (spiral path). Celebrate any creative attempts regardless of full accuracy. | |
| 57–60 min | Save tracking documents. | |

### Teacher Notes
- Students who complete the Evaluate question in depth — articulating code readability, scalability, and maintainability — are demonstrating above-standard understanding of software design principles.

### Differentiation
- **Support:** Reduce to Remember, Understand, and Apply only. Provide a completed Analyse trace as a worked example.
- **Extension:** Begin thinking about the rectangle challenge extension: how would you use `if i % 2 == 0` to alternate side lengths?

---

## Lesson Plan 10 — Variables: Concepts & Practice

**Duration:** 1 hour
**Student File:** `05_variables.md`
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can define a variable, assign a value, and explain its purpose.
- Students can use a variable in place of a hardcoded number inside a loop.
- Students can demonstrate how changing one variable at the top of a program changes all affected behaviour.

### Resources
- Devices with Minecraft Education open
- Student tracking documents

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Pose: "What if your client changed their mind and wanted the square to be size 10 instead of 5? Where would you need to change the code?" Reveal: with a variable, only one line changes. | |
| 5–15 min | Teacher-led explanation of variables as labelled containers. Show with vs. without variable versions of the nested loop. | Emphasise the `=` as assignment, not equality. Students will conflate these later with `==` in conditionals. Introduce now, reinforce later. |
| 15–40 min | Students type and run the variable code example. Students complete **Modify It** tasks (change size to 3, 10, 15; add a `sides` variable; rename the variable). | Monitor: when students rename the variable, do they rename it consistently in all places? This is the key learning about variable scope and naming. |
| 40–55 min | Students complete the **Challenge** (triangle, square, hexagon using two variables). Bloom's **Remember**, **Understand**, and **Apply** questions in their tracking document. | |
| 55–60 min | Save tracking documents. Preview: "Next lesson we review everything from the first half of the course." | |

### Teacher Notes
- This is the last concept-introduction lesson before the mid-course review. Check in with struggling students: can they build a square using nested loops and a variable without scaffolding? This is the consolidation target.
- The `sides` variable extension (Modify It task 2) is a powerful insight — changing one number at the top changes the entire shape. Students who grasp this have genuinely understood abstraction.

### Differentiation
- **Support:** Focus only on the `size` variable; skip the `sides` variable extension.
- **Extension:** Bloom's **Analyse**, **Evaluate**, and **Create** questions.

---

## Lesson Plan 11 — Mid-Course Consolidation & Review

**Duration:** 1 hour
**Student File:** None (teacher-directed review)
**Outcomes:** TE4-DIG-01, TE4-DIG-02

### Learning Intentions
- Students can demonstrate all concepts learned in Hours 1–10 without scaffolding.
- Students can identify gaps in their understanding and take steps to address them.
- Students reflect on their use of digital tools and reinforce safe, responsible habits.

### Resources
- Devices with Minecraft Education open
- Student tracking documents
- Teacher observation checklist (see rubric at end of document)

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Introduce the review session. Students have 45 minutes to build a free-choice structure using everything they know so far. Minimum requirements: one variable, one loop, one nested loop, correct use of `set_item()` and `place()`. | |
| 5–50 min | Students design and build independently without referring to lesson materials. | Circulate using the progress rubric to record observations. Note: Which students work confidently? Who is looking up syntax repeatedly? Who is experimenting beyond the minimum? Address TE4-DIG-01 by briefly asking each student: "Where is your tracking document saved? Can you show me?" |
| 50–57 min | Pair-share: students show their partner's structure and explain two Python concepts they used. | Assess verbal explanations; students who can explain to a peer have internalised the concept. |
| 57–60 min | Class reflection: "What do you feel most confident with? What do you want to improve?" Record on the board. | Use student responses to adjust pacing for the second half of the course. |

### Teacher Notes
- This session gives you the most complete formative picture of the class before the second half. Record observations against the rubric now — it will be the evidence base for your feedback before the final project.
- Students who cannot construct a simple loop without the student notes need targeted support in Hours 12–17.
- TE4-DIG-01: check that all students have their tracking documents saved and named correctly. Replace any files that have been deleted or lost.

### Differentiation
- **Support:** Allow use of student notes; reduce to a simple path-building task with one loop.
- **Extension:** Build a structure that uses loops, nested loops, variables, and a turn pattern that creates a geometric shape (e.g., hexagon, spiral).

---

## Lesson Plan 12 — Vertical Building: Core Concepts

**Duration:** 1 hour
**Student File:** `06_vertical_building.md` (Theory, Code Example, Try It sections)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can name all 6 directions the Agent can move and place blocks.
- Students can write a loop that builds a tower using the `UP` direction.
- Students can explain how combining vertical movement with a loop creates a 3D structure.

### Resources
- Devices with Minecraft Education open

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Review 2D movement directions from previous lessons. Ask: "What directions haven't we used yet?" Introduce `UP` and `DOWN` as the final two. | |
| 5–15 min | Teacher-led demonstration: build a tower by running the code example. The vertical effect in Minecraft is visually impactful — let students see it before they code it. | Emphasise the order: `place(DOWN)` *then* `move(UP, 1)`. Ask: "What would happen if we swapped those two lines?" |
| 15–40 min | Students type and run the tower code. Students complete **Modify It** tasks: taller tower (change `height`), replace `UP` with `FORWARD`, begin the wall extension. | The tower-to-pillar shift (Modify It task 2) reinforces that direction is always relative to Agent movement, not block placement direction. |
| 40–57 min | Students attempt the **Challenge** (hollow tower — square base repeated vertically). Prompt planning first: "How many loops will you need? What does each one control?" | |
| 57–60 min | Debrief: draw the two-loop structure on the board (height = outer, square = inner). | |

### Teacher Notes
- The hollow tower challenge requires three levels of loops (height, sides, blocks per side). Students who are not fully comfortable with two levels will need scaffolding here.
- The visual feedback from Minecraft is a significant motivator at this stage — structure are now three-dimensional and impressive. Use this to maintain engagement.

### Differentiation
- **Support:** Limit to a simple tower; skip the hollow tower challenge.
- **Extension:** Begin planning a pyramid (Bloom's Create question) as a design challenge.

---

## Lesson Plan 13 — Vertical Building: Practice & Extension

**Duration:** 1 hour
**Student File:** `06_vertical_building.md` (Challenge, Bloom's questions)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can analyse a given three-loop vertical building program and trace its output.
- Students can design and build a multi-variable 3D structure.

### Resources
- Devices with Minecraft Education open
- Student tracking documents

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Quick check: ask a student to verbally explain the order of `place(DOWN)` and `move(UP, 1)` in the tower loop. | |
| 5–25 min | Students complete **Remember**, **Understand**, and **Apply** Bloom's questions in their tracking document. | Check Apply responses (8-block tower using `tower_height` variable) for correct loop range and variable usage. |
| 25–50 min | Students work on the **Analyse** question (trace the given wall-building code) and the **Evaluate** question (compare loop vs. manual approach for towers). | The Analyse question is demanding — support students by asking them to trace just the first iteration of each loop before the full trace. |
| 50–57 min | Students begin the **Create** question (pyramid design). | Prompt design thinking: "How does the width of each layer change? Can you use the outer loop variable to control it?" |
| 57–60 min | Save tracking documents. Preview conditionals. | |

### Teacher Notes
- The pyramid is a genuine design challenge that requires students to use the loop counter variable (`i`) inside the loop body — a significant conceptual step. Treat this as extension, not expectation.

### Differentiation
- **Support:** Focus on Bloom's levels 1–3 only.
- **Extension:** Code and test the pyramid; describe the relationship between layer number and layer width.

---

## Lesson Plan 14 — Conditionals: Core Concepts

**Duration:** 1 hour
**Student File:** `07_conditionals.md` (Theory, Code Example, Try It sections)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can explain what a conditional does and when it is used.
- Students can write an `if/else` statement using a comparison operator.
- Students can demonstrate how changing a variable value triggers different code branches.

### Resources
- Devices with Minecraft Education open

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | "If it's raining, what do you do differently this morning?" Use the decision-making analogy to introduce conditionals. | |
| 5–15 min | Teacher-led explanation of `if`, `else`, `elif`, and comparison operators. Write a truth table for `>`, `<`, `==` on the board. | Differentiate between `=` (assignment) and `==` (comparison) — this will be the most common error in conditional code. |
| 15–40 min | Students type and run the code example (block type changes based on `size`). Students complete **Modify It** tasks (change size, change threshold, add `elif`). | The `elif` extension is significant: monitor that students understand the order of evaluation — the first true condition is the one that runs. |
| 40–57 min | Students attempt the **Challenge** (three-tier block type based on path length using `if/elif/else`). | |
| 57–60 min | Debrief: ask a student to read their `if/elif/else` chain aloud and explain which condition triggers each block type. | |

### Teacher Notes
- The `=` vs. `==` confusion is consistent and universal among beginner coders. Proactively address it before students encounter the error.
- Some students will try to nest a conditional inside a loop immediately. Encourage this experimentation — it previews Lesson 9 (guided project door gap).

### Differentiation
- **Support:** Limit to `if/else` only; skip `elif`.
- **Extension:** Introduce the concept of combining a conditional with a loop variable (`if i % 2 == 0`) to alternate block types.

---

## Lesson Plan 15 — Conditionals: Practice & Extension

**Duration:** 1 hour
**Student File:** `07_conditionals.md` (Challenge, Bloom's questions)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can trace a multi-branch conditional and predict which block type is loaded for a given input.
- Students can design a program where a single variable controls multiple aspects of a structure's appearance.

### Resources
- Devices with Minecraft Education open
- Student tracking documents

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Quick check: given `size = 7` and a specific `if/elif/else` chain on the board, ask students to state which branch runs. | |
| 5–20 min | Students complete **Remember**, **Understand**, and **Apply** Bloom's questions in their tracking document. | |
| 20–45 min | Students complete the **Analyse** question (predict block type for three different values), verify in Minecraft, then complete the **Evaluate** question (separate `if` statements vs. `if/elif/else`). | The Evaluate question is important — three separate `if` statements can cause multiple blocks to be loaded if conditions overlap. Help students discover this through testing, not just reading. |
| 45–57 min | Students work on the **Create** question (a theme-based structure with different block types per theme). | Encourage students to think about this as a preview of the final project — their final project must use conditionals. |
| 57–60 min | Save tracking documents. | |

### Teacher Notes
- Students who successfully explain the `if/elif/else` chain to a partner, including why order matters, are demonstrating above-standard understanding.

### Differentiation
- **Support:** Provide a worked example of the Analyse question before students attempt it independently.
- **Extension:** Add a fourth theme value to the Create structure and test it.

---

## Lesson Plan 16 — Debugging: Concepts & Practice

**Duration:** 1 hour
**Student File:** `08_debugging.md` (Theory, Broken Code, Try It sections)
**Outcomes:** TE4-DIG-01, TE4-DIG-02

### Learning Intentions
- Students can name and distinguish the three main error types: syntax, indentation, and logic.
- Students can read an error message, identify the line, and apply a fix.
- Students recognise that debugging is a normal, expected part of programming.

### Resources
- Devices with Minecraft Education open

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | "Has anyone ever had code that didn't work? Raise your hand." Normalise errors. Share the origin of the word "bug." | TE4-DIG-01: reinforce that debugging responsibly (not blindly deleting code) is part of safe and productive digital practice. |
| 5–15 min | Teacher-led overview of the three error types. Show an example of each on the board with its error message. | Teach the debugging process: Read → Locate → Fix → Run → Repeat. Write this on the board. |
| 15–45 min | Students work through the three broken code snippets. For each: predict the error type before running, run to see the message, fix it, and add a comment explaining what was wrong. | Circulate and observe: are students reading the error message, or changing code randomly? Students who read error messages carefully are developing productive debugging habits. |
| 45–57 min | Students introduce their own logic error (Modify It task 2) and describe the result in a comment. | Reinforce: logic errors are the hardest to find because Python does not report them — you must observe and reason. |
| 57–60 min | Debrief: "What is the difference between a syntax error and a logic error?" | |

### Teacher Notes
- Students who change random parts of code without reading error messages will reinforce bad habits. Intervene early with: "Before you change anything, what does the error message say?"
- TE4-DIG-01 connection: debugging requires careful, methodical interaction with the digital environment — guessing and randomly deleting code is a form of digital carelessness.

### Differentiation
- **Support:** Provide the error type as a hint before students attempt to find the bug.
- **Extension:** Bloom's **Create** question (write a debugging guide for beginners).

---

## Lesson Plan 17 — Debugging: Peer Review & Extension

**Duration:** 1 hour
**Student File:** `08_debugging.md` (Challenge, Bloom's questions)
**Outcomes:** TE4-DIG-01, TE4-DIG-02

### Learning Intentions
- Students can find and fix multiple bugs in an unfamiliar piece of code.
- Students can write clearly documented fixes for each error type.
- Students can explain their debugging process to a peer.

### Resources
- Devices with Minecraft Education open
- Student tracking documents

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Review error types. Pair students for the peer debugging challenge. | |
| 5–35 min | Students write their own 6–10 line program with 3 intentional bugs (at least one of each type). They swap with their partner and attempt to find and fix all three bugs. | Monitor that bugs are genuine (not trivially obvious). Circulate and observe the quality of comments that students write when fixing. |
| 35–50 min | Students respond to Bloom's **Remember**, **Understand**, and **Apply** questions in their tracking documents. | |
| 50–57 min | Students attempt the **Analyse** and **Evaluate** questions. The Evaluate question (reading errors vs. random changes) has direct real-world implications for professional practice. | |
| 57–60 min | Save tracking documents. Preview the guided project. | |

### Teacher Notes
- Peer debugging develops communication skills as well as coding skills — students must describe errors clearly to their partner. This is an excellent informal assessment of verbal understanding.
- TE4-DIG-01: writing code that others will read is a form of responsible digital communication. Reinforce that code comments are part of good digital practice.

### Differentiation
- **Support:** Reduce to finding and fixing 2 bugs (one syntax, one indentation only).
- **Extension:** Bloom's **Create** (write a debugging guide); this can be added to their tracking document as a study resource.

---

## Lesson Plan 18 — Guided Project: Planning & Start

**Duration:** 1 hour
**Student File:** `09_guided_project.md` (Theory, Code Example — Floor section)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can apply all prior concepts in combination to begin a multi-section program.
- Students can plan a project by breaking it into steps before coding.
- Students can build and test the floor section of a house base independently.

### Resources
- Devices with Minecraft Education open
- Student tracking documents

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Review the concepts covered so far. Ask: "How many Python concepts have you learned?" Connect them: sequencing, blocks, loops, nested loops, variables, 3D movement, conditionals, debugging. | |
| 5–15 min | Teacher-led overview of the guided project plan: what a house base looks like, what the two main sections are (floor and walls), and the importance of planning before coding. | Introduce the Plan Before You Code habit: describe → break down → identify concepts → write → test incrementally. |
| 15–45 min | Students work through the planning phase. They then code and test **Step 1 only** (the floor), using the `size` variable and nested loop. | Students must run and verify the floor before moving to the walls. Monitor that they are testing incrementally, not trying to write the full program at once. |
| 45–57 min | Students who have a verified floor begin thinking about how to adapt the floor loop for walls (`FORWARD` instead of `DOWN`). They should sketch the approach, not yet code it. | |
| 57–60 min | Debrief: "What changes when you move from floor to wall building?" | |

### Teacher Notes
- Incremental testing is the most important professional practice to establish in this lesson. Students who write all the code first, then run it, will struggle when problems arise.
- The variable `size` should already be familiar from Lesson 5 — reinforce that this is not a new concept, just a new application.

### Differentiation
- **Support:** Provide the floor code with one blank variable value for students to determine.
- **Extension:** Students begin designing the door gap modification from the Modify It section.

---

## Lesson Plan 19 — Guided Project: Build & Refine

**Duration:** 1 hour
**Student File:** `09_guided_project.md` (Code Example — Walls section, Modify It, Challenge)
**Outcomes:** TE4-DIG-02

### Learning Intentions
- Students can extend a working floor program to add walls using a third level of loops.
- Students can modify a complete structure by changing variables.
- Students can use a conditional inside a loop to create a gap in a wall (door).

### Resources
- Devices with Minecraft Education open
- Student tracking documents

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Review floor code from last lesson. Ask: "What is the only difference between the floor loop and the wall loop?" (The direction: `DOWN` vs. `FORWARD`.) | |
| 5–30 min | Students add the walls section to their existing code. They should test after adding the outermost height loop. | Monitor the three-loop structure carefully — this is the most complex nested structure in the course. Students who attempt to write all three loops at once often make indentation errors. Prompt: "Test with `wall_height = 1` first." |
| 30–50 min | Students complete **Modify It** tasks: change size and height, add the door gap conditional, change wall material. | The door gap task is the highest-difficulty modification in the course — it combines a nested conditional inside three levels of loops. Students who achieve this independently are at an advanced level. |
| 50–57 min | Students attempt the **Challenge**: add a roof using a filled square loop. | This is extension. Prompt: "How is the roof different from the floor? What's the difference between a square outline and a filled square?" |
| 57–60 min | Save code and tracking document. Preview the final project. | |

### Teacher Notes
- This is the most technically demanding coding session in the course. Expect a wide spread of progress. Some students will complete the full house with roof; others may still be working on walls. Both are acceptable.
- Use this lesson's observations to identify students who will need additional scaffolding in the final project.

### Differentiation
- **Support:** Provide the walls loop structure as a scaffold; students only need to fill in variables.
- **Extension:** Add the roof section and window gaps using conditionals on both layer and position.

---

## Lesson Plan 20 — Final Project: Design, Build & Present

**Duration:** 1 hour
**Student File:** `10_final_project.md`
**Outcomes:** TE4-DIG-01, TE4-DIG-02

### Learning Intentions
- Students can select and design a final project that meets all specified code requirements.
- Students can complete a planning document (sketch, concept table, pseudocode) before coding.
- Students can begin implementing their own original structure using all learned concepts.

> **Note:** The final project is designed to extend beyond this single lesson — it is the culmination of the course and students should continue building and complete their PowerPoint presentation in their own time or in subsequent timetabled sessions as allocated by the school. This lesson launches the project and ensures all students have a sound plan before coding begins.

### Resources
- Devices with Minecraft Education open
- Student tracking documents
- Project planning template (optional: provide the requirements table from `10_final_project.md` as a printed planning sheet)

### Lesson Timing

| Time | Activity | Teacher Focus |
|---|---|---|
| 0–5 min | Introduce the final project. Review the requirements (2+ variables, 1+ loop, 1+ nested loop, 1+ conditional, 1+ 3D element, well-commented code). Confirm the assessment format: PowerPoint presentation. | TE4-DIG-01: reinforce digital presentation standards — original work, properly attributed assets, saved to personal drives. |
| 5–20 min | Students complete the three planning steps: sketch the structure, fill in the concept table, and write pseudocode. No coding until the plan is complete. | Circulate and approve plans. A plan is ready when: the structure is described, all required concepts are accounted for, and pseudocode outlines the main steps. Do not allow students to start coding without an approved plan. |
| 20–50 min | Students begin implementing their code based on their plan. They should code and test in sections, not all at once. | Monitor incremental testing. Prompt: "Test your floor first. Does it work? Now add walls." Reinforce the debugging process when errors occur. |
| 50–57 min | Students save code and update tracking documents. Confirm all files are saved to cloud storage. | TE4-DIG-01: final check that all course work is saved and named correctly. |
| 57–60 min | Close the course: celebrate what students have learned. Connect Python skills to real-world programming. | |

### Teacher Notes
- The planning gate (no coding without an approved plan) is non-negotiable. Students who skip planning produce incomplete, disorganised code and become frustrated.
- TE4-DIG-01 is prominent here: digital presentation, file management, and original work expectations must be clearly stated before the PowerPoint is begun.
- If the school timetable allows additional sessions beyond these 20 hours, they should be used for project completion, peer feedback, and presentations.

### Differentiation
- **Support:** Provide a partially completed planning template; limit requirements to one variable, one loop, and one conditional.
- **Extension:** Option D (own idea) with a more complex structure; attempt the Bloom's Create reflection from the student sheet.

---

---

# Progress Monitoring Rubric

## Purpose

This rubric is for **teacher use only** — it supports formative and summative monitoring of student progress throughout the 20-hour course. Use it during circulating observations, the mid-course consolidation (Hour 11), and the final project assessment (Hours 18–20).

---

## TE4-DIG-01 — Demonstrates technological literacy to safely interact in digital environments

| Indicator | Working Towards | Meeting Expectations | Extending Beyond |
|---|---|---|---|
| **Account and file management** | Rarely saves work independently; frequently loses files; needs reminders to use school account. | Consistently saves work to OneDrive/Google Drive using the correct naming convention with occasional prompts. | Independently maintains organised files; proactively manages versions of their code. |
| **Safe and responsible use** | Occasionally uses the digital environment inappropriately (e.g. accessing unrelated content, modifying others' worlds). | Uses Minecraft Education and Code Builder appropriately for learning purposes throughout the course. | Actively models responsible use; supports peers in using the environment correctly. |
| **Understanding of digital environments** | Cannot describe the difference between Code Builder and standard Python or explain why the environment matters. | Can explain that MakeCode Python runs inside Minecraft Education and that the Code Builder interface controls code execution. | Articulates the relationship between digital tools, environments, and outputs; can compare MakeCode Python to broader Python contexts. |
| **Troubleshooting digital tools** | Stops working when a technical issue occurs; requires teacher intervention for any problem. | Attempts common fixes independently (e.g. teleporting the Agent, checking Python tab, re-reading error messages). | Systematically diagnoses digital problems and explains the resolution process to peers. |

---

## TE4-DIG-02 — Uses data and digital systems to code, design and produce projects

### Strand 1: Coding Concepts

| Concept | Working Towards | Meeting Expectations | Extending Beyond |
|---|---|---|---|
| **Sequencing** | Cannot reliably predict the order of execution; places commands in incorrect order. | Writes sequences of `move()` and `turn()` commands that produce the intended path; predicts order of execution before running. | Designs complex multi-step sequences; explains why order affects outcome at a conceptual level. |
| **Placing Blocks** | Frequently forgets `set_item()` before `place()`; cannot explain the purpose of each parameter. | Correctly uses `set_item()` with all three parameters and `place()` with a direction to build a path. | Uses multiple block types, slots, and directions strategically in a single program. |
| **Loops** | Cannot write a `for` loop independently; indentation errors are frequent; does not predict loop count. | Writes a `for` loop with correct syntax and indentation that repeats a block-placing action the intended number of times. | Uses the loop variable `i` inside the loop body; explains `range()` at the conceptual level; designs efficient loops for complex patterns. |
| **Nested Loops** | Cannot distinguish outer from inner loop; indentation is incorrect at the second level. | Writes a nested loop that builds a square outline with correct two-level indentation; calculates total iterations correctly. | Uses nested loops to build complex shapes (rectangle, triangle, spiral); traces nested loops step-by-step accurately. |
| **Variables** | Hardcodes values rather than using variables; cannot explain why a variable is useful. | Declares a variable at the top of a program and uses it in a loop to control size or behaviour; can change the value and explain the effect. | Uses multiple variables to control different aspects of a program; names variables meaningfully; explains abstraction informally. |
| **3D Movement** | Cannot distinguish `UP`/`DOWN` from horizontal directions; places blocks in wrong direction. | Uses `UP` direction with a loop to build a tower; combines vertical and horizontal loops to build walls. | Combines 3D movement, variables, and nested loops to build multi-storey structures; plans 3D structures using pseudocode. |
| **Conditionals** | Cannot write an `if` statement; confuses `=` with `==`; cannot predict which branch runs for a given value. | Writes an `if/else` conditional that changes block type based on a variable; predicts the correct branch for given values. | Uses `if/elif/else` chains with multiple conditions; uses conditionals inside loops to create structural variations (e.g. gaps, alternating materials). |
| **Debugging** | Does not read error messages; changes code randomly without reasoning; unable to distinguish error types. | Reads an error message, identifies the error type and line, and applies a targeted fix; distinguishes syntax, indentation, and logic errors. | Consistently debugs using the Read → Locate → Fix → Run process; detects logic errors through observation and reasoning; writes clear comments explaining fixes. |

---

### Strand 2: Design and Project Process

| Indicator | Working Towards | Meeting Expectations | Extending Beyond |
|---|---|---|---|
| **Planning before coding** | Starts coding immediately without planning; code lacks structure or comments. | Sketches or describes the intended structure before coding; uses comments to label code sections. | Writes pseudocode that maps each step to a Python concept; revises plans based on testing. |
| **Incremental testing** | Writes large blocks of code before testing; cannot identify where an error originates. | Runs and checks code after each major section; verifies one component works before adding the next. | Systematically tests with boundary values (e.g. `size = 1`, `size = 100`); records and explains observations. |
| **Code quality** | Code is uncommented, inconsistently indented, and difficult to read. | Code is consistently indented and includes comments explaining each main section. | Code uses meaningful variable names, clear structure, and comments that explain both *what* and *why*. |
| **Project completion** | Final project does not meet minimum requirements; multiple required concepts are absent. | Final project includes all required elements (2+ variables, 1+ loop, 1+ nested loop, 1+ conditional, 1+ 3D element) and builds as expected. | Final project exceeds requirements; demonstrates creative application of multiple concepts; includes extensions such as door gaps, alternating materials, or compound 3D structures. |
| **Reflection and communication** | Cannot explain what their code does or why they made particular choices. | Can describe what their program does and identify where each required concept appears, in spoken or written form. | Articulates the design decisions behind their code; identifies what they would change or extend; connects course learning to broader programming contexts. |

---

## Using the Rubric

- **Formative (ongoing):** Use the Strand 1 rows during classroom circulations to note individual progress against each concept. A brief anecdotal note per student per lesson is sufficient.
- **Mid-course (Hour 11):** Use the full rubric to record a mid-point snapshot for each student. Share findings with students as written or verbal feedback before the second half of the course.
- **Summative (Hours 18–20):** Apply the Strand 2 rows to the Guided Project and Final Project outputs. The PowerPoint presentation (Final Project) provides evidence for the Reflection and Communication row.
- **Reporting:** The rubric descriptors map directly to the language in TE4-DIG-01 and TE4-DIG-02. Use the *Meeting Expectations* column as the standard for a grade-level achievement result; *Working Towards* indicates below standard; *Extending Beyond* indicates above standard.
