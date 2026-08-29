# 3D Animation 11 – Cloth Simulation

## Unit 4: Physics Simulation & Intro to Unreal Engine — Challenge F2

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenge F1.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Set up a Cloth simulation on a simple fabric-like object
- Adjust cloth presets and settings for different fabric weights/behaviors
- Combine cloth simulation with a collision object (e.g., a character or simple shape)
- Continue building the naming/saving habits started in Challenge F1, ahead of this unit's move into Unreal

---

## 💭 Production Question

### What makes fabric look heavy versus light, without changing its color or shape at rest?

---

## Checkpoint 1 — Basic Cloth Setup (Day 1)

**✏️ Simulate a Simple Cloth**

1. Add a Plane, subdivide it several times (right-click → Subdivide, repeated, or use the Subdivision Surface modifier for a smoother result) so it has enough geometry to fold realistically.
2. Set the plane as a Cloth object (Physics Properties → Cloth).
3. Add a simple collision object below/near it (a sphere or cube) and set that object as a Collision object (Physics Properties → Collision).
4. Play the simulation and watch the cloth fall and drape over the collision object.
5. If the cloth passes through the collision object, increase the Collision object's "Distance" or "Thickness" settings and re-test.

**Requirements**

- Cloth object correctly draping over a collision object
- No major clipping/pass-through between cloth and collision object
- Simulation plays back with believable draping behavior

---

## Checkpoint 2 — Cloth Presets & Fabric Weight (Days 1–2)

**✏️ Compare Fabric Types**

1. In the Cloth physics panel, try the built-in presets (Cotton, Silk, Denim, Leather, Rubber) from the Presets dropdown and re-run the simulation for each.
2. Compare how differently each preset behaves — silk should look light and flowy, denim/leather should look stiffer and heavier.
3. Choose two contrasting presets and render a short simulation of each for comparison.
4. If time allows, manually adjust individual settings (Mass, Stiffness, Damping) to create a custom fabric weight rather than relying only on presets.

**Requirements**

- At least two different cloth presets tested and compared
- Clear visual difference documented between a "light" and a "heavy" fabric behavior
- Optional: at least one manually customized setting beyond the presets

---

## Checkpoint 3 — Applied Cloth Example (Days 2–3)

**✏️ Apply Cloth to a Character/Object Detail**

1. Add a simple piece of clothing or fabric detail to one of your existing models (a cape on your Challenge C1 character, a flag, a curtain, a tablecloth).
2. Set it up as a Cloth object, with your character or another appropriate object as its Collision target.
3. Animate a simple motion for the collision object (a character turning, a light breeze suggested by a Wind force field) and observe how the cloth reacts.
4. Adjust cloth settings as needed until the motion looks believable for the context (not too stiff, not too floaty for the material intended).
5. Save your file with a clear, version-numbered filename (e.g., `LastName_F2_ClothSim_v01.blend`), and rename the cloth object itself in the Outliner (e.g., `Cloth_Cape_01`) — the same habit from Challenge F1, kept up here.

**Requirements**

- Cloth applied to a genuine piece of clothing/fabric detail on an existing model
- Cloth reacts appropriately to the motion of its collision object
- Final settings are appropriate to the type of fabric being represented
- File and object clearly named/versioned

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. What was the visual difference between your two chosen cloth presets?
2. What happened when the collision object's Distance/Thickness setting was too low?
3. How did adding cloth to an existing model change how "real" that object felt?
4. Where else in your future projects could cloth simulation add believability?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI2020_F2_ClothSim.blend`

**Fabric Preset Comparison Renders (2)**

Filename: `LastName_ANI2020_F2_Preset_01.mp4`, `_02.mp4`

**Applied Cloth Example Render**

Filename: `LastName_ANI2020_F2_AppliedCloth.mp4`

**Reflection Document**

Filename: `LastName_ANI2020_F2_Reflection.pdf`

---

## 📊 Assessment Criteria

**Basic Cloth Setup (25%)**

- Cloth correctly drapes over a collision object
- No significant clipping between cloth and collision geometry
- Simulation plays back reliably

**Fabric Weight Comparison (25%)**

- At least two contrasting presets tested and compared
- Clear, documented visual difference between light and heavy fabric behavior
- Understanding shown of what settings control that difference

**Applied Cloth Example (35%)**

- Cloth applied meaningfully to an existing model's clothing/fabric detail
- Cloth reacts believably to the collision object's motion
- Settings chosen appropriately for the intended fabric type
- Result adds genuine visual believability to the model

**Reflection (15%)**

- Thoughtful, specific reflection on the process
- Clear explanation of the preset comparison results
- Honest account of any collision/clipping troubleshooting
- Specific idea for future use of cloth simulation

---

## 💡 Key Lesson

Cloth simulation is what separates a character that looks "posed" from one that looks like it's actually wearing something in a real environment — small details like this are often what separate strong competition pieces from merely competent ones.
