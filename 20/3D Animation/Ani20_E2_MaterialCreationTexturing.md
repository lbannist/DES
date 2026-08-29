# 3D Animation 11 – Material Creation & Texturing

## Unit 3: Material Creation & Texturing — Challenge E2

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenge E1. *

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Understand and adjust Base Color, Roughness, and Metallic inputs on the Principled BSDF
- Use Normal maps to fake surface detail without adding geometry
- Build at least two clearly different PBR materials (e.g., metal and non-metal)

---

## 💭 Production Question

### How do a handful of numbers convince your eye that something is metal, plastic, or fabric?

---

## Checkpoint 1 — Roughness & Metallic Study (Day 1)

**📖 Isolated Parameter Test**

1. Create a simple test scene: a sphere lit with an HDRI or simple three-point setup so reflections are visible.
2. Set Metallic to 0 and test several Roughness values (e.g., 0.1, 0.5, 0.9) — render or view each and note how the reflection changes from sharp/mirror-like to soft/diffuse.
3. Now set Metallic to 1 and repeat the same Roughness tests — compare how metallic surfaces respond differently to roughness than non-metallic ones.
4. Write down, in your own words, what Roughness and Metallic each control.

**Questions to answer:**

1. What does Roughness control, in plain language?
2. What's the visual difference between a rough metal and a smooth metal?
3. What's the visual difference between a rough non-metal and a smooth non-metal?

---

## Checkpoint 2 — Normal Maps (Days 1–2)

**✏️ Fake Detail with a Normal Map**

1. Find or generate a simple normal map texture (a bumpy/brick/fabric normal map is fine for practice — check with your teacher for an approved source).
2. Add an Image Texture node, load the normal map, and connect it through a Normal Map node into the Principled BSDF's Normal input (do not plug it directly into Base Color).
3. Render your object and rotate the view/lighting to see how the fake surface detail catches light differently as the angle changes.
4. Compare this result to the same object with no normal map at all — note what's gained, and what's NOT actually there (the geometry itself hasn't changed).

**Requirements**

- Normal map correctly connected through a Normal Map node (not plugged in directly)
- Before/after comparison clearly shows the added surface detail
- Understanding shown that normal maps fake detail rather than adding real geometry

---

## Checkpoint 3 — Building Two Contrasting Materials (Days 2–3)

**✏️ Metal vs. Non-Metal**

1. Choose two real-world materials to recreate — one metal (e.g., brushed steel, gold, chrome) and one non-metal (e.g., plastic, wood, cloth).
2. For the metal material, set Metallic to 1 and choose a Roughness value that matches your reference's shininess; adjust Base Color to an appropriate metallic tint.
3. For the non-metal material, keep Metallic at 0 and set Base Color and Roughness to match your reference's look.
4. Add a Normal map to at least one of the two materials to add appropriate surface detail (brushed metal grain, fabric weave, wood grain).
5. Apply both materials to test objects and render them side by side under the same lighting.

**Requirements**

- Two clearly contrasting materials built (one metal, one non-metal)
- Each material's Roughness/Metallic/Base Color values chosen with reference in mind
- At least one material uses a Normal map for added detail

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. What Roughness value did you find most convincing for your metal material, and why?
2. What was the biggest visual difference between your metal and non-metal materials?
3. How did the Normal map change the perceived detail of your object without changing its actual geometry?
4. Which of your two materials do you think reads more convincingly as "real," and why?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI2020_E2_PBRMaterials.blend`

**Roughness/Metallic Comparison Renders**

Filename: `LastName_ANI2020_E2_RoughnessTest.png`

**Normal Map Before/After Renders**

Filename: `LastName_ANI2020_E2_NormalMap_Before.png`, `_After.png`

**Final Metal/Non-Metal Comparison Render**

Filename: `LastName_ANI2020_E2_MaterialComparison.png`

**Reflection Document**

Filename: `LastName_ANI2020_E2_Reflection.pdf`

---

## 📊 Assessment Criteria

**Roughness & Metallic Understanding (25%)**

- Multiple Roughness values tested and clearly compared
- Metallic on/off comparison clearly documented
- Written explanation of Roughness and Metallic is accurate and specific
- Final material choices reflect genuine understanding, not guesswork

**Normal Map Application (25%)**

- Normal map correctly connected through a Normal Map node
- Clear before/after comparison demonstrating the effect
- Detail added is appropriate to the material being represented
- Understanding shown that normal maps do not add real geometry

**Material Contrast (30%)**

- Two clearly different, convincing materials built
- Metal material reads believably as metal; non-metal reads believably as non-metal
- Material values are clearly informed by real-world reference
- Side-by-side comparison render clearly shows the contrast

**Reflection (20%)**

- Thoughtful, specific reflection on the process
- Clear, accurate explanation of Roughness's visual effect
- Honest assessment of which material was more convincing and why
- Specific connection drawn between reference and final material values

---

## 💡 Key Lesson

PBR materials work because they mimic how light actually behaves on different surfaces — a handful of well-chosen values (Roughness, Metallic, Normal) can convince the eye far more effectively than adding extra geometry or detail. This same PBR thinking carries directly into Substance Painter workflows in Grade 12.
