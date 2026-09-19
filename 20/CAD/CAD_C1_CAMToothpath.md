# CAD 11 – Manufacturing-Ready Modeling

## Unit C: Manufacturing-Ready Modeling — Challenge C1

**Time:** 1–1.5 Weeks (4 Class Periods)
**Due Date:** *[insert due date]*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Model a genuinely machinable solid part, including threads, chamfers, and hex flats
- Set up a work coordinate system (WCS) appropriate to a cylindrical part
- Generate and simulate a complete CAM toolpath before it would ever reach a machine
- Understand the connection between a solid model's features and how those features actually get cut

---

## 💭 Production Question

### What has to change in how you model a part once you know a machine — not just a viewer — has to read it?

---

## Checkpoint 1 — Modeling the Part (Day 1)

**✏️ Build the Spark Plug Solid Model**

1. Follow the provided spark plug tutorial series to model the part, including the external thread, hex flats, and chamfers.
2. Pay attention to how each feature is built, not just the end result — you'll need to model similar features independently in later challenges.
3. Check your model's critical dimensions against the tutorial's reference values.

**Requirements**

- Complete solid model matching the tutorial's part
- Threads, hex flats, and chamfers all present and correctly dimensioned
- Model organized in a clean, logically named timeline

---

## Checkpoint 2 — CAM Setup & Toolpath Generation (Days 2–3)

**✏️ Move from Model to Machine**

1. Set up stock and place the work coordinate system (WCS) appropriately for a cylindrical part.
2. Generate toolpaths in this order: facing, 2D contour for the hex flats, then thread milling or single-point threading for the external thread.
3. Set feeds and speeds appropriate to the stock material you're using.
4. Run a full toolpath simulation and check for collisions or gouges before considering the toolpath finished.
5. Post-process the toolpath to the router's actual controller.

**Requirements**

- Toolpaths generated for facing, hex flats, and threading
- Feeds and speeds set and justified for the chosen stock
- Full simulation run with no collisions or gouges
- Posted G-code file included in your submission

---

## Checkpoint 3 — Reflection

**✏️ Answer:**

1. Which feature (threads, hex flats, or chamfers) was hardest to model correctly, and why?
2. What did the toolpath simulation catch that you wouldn't have noticed just looking at the model?
3. If you had to cut this part in a different material, what would you need to change and why?
4. What's one thing about "designing for manufacturing" that surprised you in this challenge?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Fusion 360 Project File**

Filename: `LastName_C1_SparkPlug.f3d`

**CAM Setup / Toolpath File**

Filename: `LastName_C1_SparkPlug_CAM.f3d` (or included in the same file if CAM is in the same document)

**Posted G-Code**

Filename: `LastName_C1_SparkPlug.nc`

**Reflection Document**

Filename: `LastName_C1_Reflection.pdf`

---

## 📊 Assessment Criteria

**Solid Modeling (30%)**

- Threads, hex flats, and chamfers modeled correctly and to dimension
- Clean, logically organized timeline

**CAM Setup & Toolpath (35%)**

- Correct WCS placement and stock setup
- Appropriate feeds/speeds for stock material
- Clean simulation with no collisions or gouges

**Technical Execution (15%)**

- Successfully posted, machine-ready G-code

**Reflection (20%)**

- Clear articulation of modeling and CAM challenges
- Honest account of what the simulation revealed

---

## 💡 Key Lesson

A model that looks correct on screen isn't the same as a model that's ready to be cut — that gap only closes once you've set up the stock, simulated the toolpath, and caught the collision before the machine would have.
