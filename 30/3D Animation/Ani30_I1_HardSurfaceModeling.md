# 3D Animation 12 – Hard-Surface Modelling Fundamentals

## Unit 3: Hard-Surface Modeling, Texturing & Look Development — Challenge I1


**Time:** 1.5 Weeks (4 Class Periods)
**Due Date:** *[insert due date]*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Use the Bevel modifier and manual bevels to create clean edge highlights
- Use Boolean operations to cut and combine hard-surface shapes
- Control edge flow so Subdivision Surface behaves predictably on hard-surface geometry
- Kit-bash a game-ready prop from a small library of reusable shapes

---

## 💭 Production Question

### What makes a hard-surface prop read as "manufactured" rather than sculpted?

---

## Checkpoint 1 — Reference & Bevel Practice (Day 1)

**📖 Hard-Surface Reference Study**

1. Find 2–3 reference images of a prop type you want to build (a weapon, vehicle part, mechanical device, or sci-fi/industrial object).
2. Identify visible edge highlights in the reference — these come from small bevels catching light, not sharp, knife-edge geometry.
3. On a simple test cube, add a Bevel modifier and adjust the Amount and Segments values, then render a test image to see how the bevel catches light differently than a sharp edge.
4. Try adding a manual bevel (Ctrl+B in Edit Mode) on a specific edge instead of the whole object, and compare the control this gives you versus the modifier applied to everything.

**Questions to answer:**

1. Why do professional hard-surface models almost always have small bevels, even on "sharp" edges?
2. What's the difference between using the Bevel modifier globally versus beveling specific edges manually?

---

## Checkpoint 2 — Boolean Operations (Days 1–2)

**✏️ Cut and Combine Shapes**

1. Model a base shape for your prop (a body, a housing, a main structural piece).
2. Add a second "cutter" shape and use a Boolean modifier set to Difference to carve details (vents, panel lines, screw holes, cutouts).
3. Try a Boolean Union on a separate pair of shapes to merge two forms seamlessly (e.g., attaching a grip or handle to the main body).
4. Check the resulting geometry in Edit Mode for Boolean artifacts (stray faces, non-manifold edges) and clean up using Merge by Distance or manual cleanup as needed.
5. Add bevels (modifier or manual) to the new edges created by your Boolean operations so they don't look sharp/unfinished.

**Requirements**

- At least one Boolean Difference and one Boolean Union operation used
- Resulting geometry checked and cleaned of artifacts
- New edges from Boolean operations given appropriate bevels

---

## Checkpoint 3 — Edge Flow for Subdivision (Days 2–3)

**✏️ Control Subdivision Behavior**

1. Add a Subdivision Surface modifier to a hard-surface piece and observe how it currently rounds off edges you want to stay sharp.
2. Add supporting edge loops close to sharp edges (using Loop Cut) to hold that sharpness under subdivision — closer loops mean sharper resulting edges.
3. Compare a piece with too few supporting loops (overly rounded/melted-looking) to one with correctly placed loops (crisp, intentional edges).
4. Adjust until your hard-surface piece reads as crisp and manufactured, not soft and blobby.

**Requirements**

- Subdivision Surface modifier applied to at least one piece
- Supporting edge loops correctly placed to maintain intended sharp edges
- Clear before/after comparison showing the effect of edge loop placement

---

## Checkpoint 4 — Kit-Bashing Assembly (Day 4)

**✏️ Build a Reusable Kit and Assemble Your Prop**

1. Model at least 3 small reusable "kit" pieces (a bolt, a vent panel, a pipe section, a greeble block) separate from your main prop.
2. Duplicate and attach these kit pieces onto your main prop's surface to add detail quickly, rather than modeling every small detail individually.
3. Check scale and placement so kit pieces look intentional, not randomly scattered.
4. Do a final bevel/cleanup pass across the whole assembled prop.

**Requirements**

- At least 3 reusable kit pieces created and used more than once across the prop
- Kit pieces placed with intentional scale and positioning
- Final prop shows a cohesive, "manufactured" hard-surface look

---

## Checkpoint 5 — Reflection

**✏️ Answer:**

1. What was the trickiest Boolean operation to get clean results from, and how did you fix it?
2. How did edge loop placement change the way your model responded to Subdivision Surface?
3. Which kit-bashed detail piece ended up being the most useful across your prop?
4. How ready do you feel to bring this prop into Substance Painter for Challenge I3?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI3030_I1_HardSurfaceProp.blend`

**Kit Piece Library Screenshot**

Filename: `LastName_ANI3030_I1_KitPieces.png`

**Final Prop Renders (2 angles)**

Filename: `LastName_ANI3030_I1_FinalRender_01.png`, `_02.png`

**Reflection Document**

Filename: `LastName_ANI3030_I1_Reflection.pdf`

---

## 📊 Assessment Criteria

**Bevel & Edge Detail (20%)**

- Bevels correctly applied (modifier and/or manual) to create realistic edge highlights
- Bevel amount/segments appropriate to the scale of the prop
- Edges read as intentional, not accidentally sharp or overly rounded

**Boolean Operations (25%)**

- At least one clean Boolean Difference and one Boolean Union
- Resulting geometry checked and cleaned of artifacts
- New Boolean edges appropriately beveled

**Edge Flow & Subdivision Control (25%)**

- Supporting edge loops correctly placed to maintain sharp edges under subdivision
- Clear improvement shown between unsupported and supported geometry
- Overall silhouette reads as crisp and manufactured

**Kit-Bashing & Final Assembly (20%)**

- At least three reusable kit pieces created and reused
- Kit pieces placed with intentional scale and positioning
- Final prop reads as a cohesive, believable hard-surface object

**Reflection (10%)**

- Thoughtful, specific reflection on the process
- Honest account of the trickiest Boolean problem solved
- Clear connection drawn to the upcoming Substance Painter work

---

## 💡 Key Lesson

Hard-surface modeling is a completely different mindset from the organic character work earlier in the program — it's about precision, edge control, and reusable kit pieces rather than sculpted form. This is the exact skill set the 3D Digital Game Art Skills Alberta category expects competitors to have mastered.
