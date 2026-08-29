# 3D Animation 11 – Intro to Unreal Engine: Import Pipeline & Interface

## Unit 4: Physics Simulation & Intro to Unreal Engine — Challenge F3

**Time:** 1.5 Weeks (4 Class Periods)
**Due Date:** *[insert due date]*

*Builds on the naming/saving habits practiced in Challenges F1–F2.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Navigate the Unreal Engine 5 interface (viewport, Content Browser, Outliner)
- Set up a clear, organized Unreal project structure from the start
- Export a Blender asset and import it into Unreal correctly
- Understand and correct for the scale difference between Blender (meters) and Unreal (centimeters)
- Apply a basic material to an imported asset inside Unreal

---

## 💭 Production Question

### What has to go right for an asset to survive the trip from one piece of software into another?

---

## Checkpoint 1 — Unreal Interface Navigation & Project Setup (Day 1)

**📖 Interface Orientation**

1. Open Unreal Engine 5 and start a new, blank project.
2. Practice viewport navigation: right-click + WASD to fly around, middle-mouse drag to pan, scroll wheel to adjust fly speed.
3. In the Content Browser, set up a folder structure before importing anything — `Meshes`, `Materials`, `Textures` — the same organizational thinking you've been using for your Blender file names and objects in Challenges F1–F2, just applied to a new piece of software.
4. Explore the Outliner (top-right panel) and note how it's similar to (and different from) Blender's Outliner.
5. Open Project Settings and confirm your project's default unit scale (centimeters).

**Questions to answer:**

1. What similarities and differences do you notice between Unreal's interface and Blender's?
2. What unit does Unreal use by default, and how does that compare to Blender's default unit?

---

## Checkpoint 2 — Exporting from Blender (Days 1–2)

**✏️ Prepare and Export Your Asset**

1. Choose a simple, finished asset from earlier coursework — this can be one of your named, baked simulation objects from Challenge F1 or F2, or another simple prop.
2. In Blender, apply all modifiers and transforms (Object → Apply → All Transforms) so scale/rotation aren't hidden in the object's data when exported.
3. Double check the object's name in the Outliner is still clear (this is exactly the habit you practiced in F1–F2 — it pays off right now, since a vague name here becomes a vague name in Unreal too).
4. Export the asset as an FBX file (File → Export → FBX), saving it with a clear, version-numbered filename (e.g., `LastName_F3_Asset_v01.fbx`).
5. In the FBX export settings, check the Scale setting — note that Blender's default export scale may need adjustment to avoid a size mismatch once imported (Blender uses meters; Unreal uses centimeters, a 100x difference).

**Requirements**

- Asset transforms applied before export
- Asset clearly named and FBX exported with a clear, version-numbered filename
- Export scale setting deliberately checked, not left unexamined

---

## Checkpoint 3 — Importing into Unreal (Day 2–3)

**✏️ Import and Fix Scale**

1. In Unreal's Content Browser, right-click → Import, and select your exported FBX file, making sure it lands in your `Meshes` folder from Checkpoint 1.
2. Drag the imported asset into the viewport and compare its size to Unreal's default cube or a placeholder character — if it looks 100x too small or too large, this is the meters/centimeters mismatch from Checkpoint 2.
3. Fix the scale either by re-exporting from Blender with a corrected scale factor, or by adjusting the import scale settings in Unreal's FBX import dialog, or by scaling the object in Unreal directly — try at least one of these methods and note which felt most reliable.
4. Once scale is correct, reposition the asset sensibly in the level.

**Requirements**

- Asset successfully imported into Unreal, sorted into the correct folder
- Scale mismatch identified and corrected using at least one method
- Asset positioned sensibly at a believable real-world scale in the level

---

## Checkpoint 4 — Basic Material Application (Day 3–4)

**✏️ Apply a Material in Unreal**

1. In the Content Browser, create a new Material asset in your `Materials` folder (right-click → Material).
2. Double-click to open the Material Editor and set a Base Color, Roughness, and Metallic value using the same PBR thinking from your Material Creation & Texturing work.
3. Apply the new material to your imported asset by dragging it onto the object in the viewport.
4. If your Blender asset had textures, try importing the texture image into your `Textures` folder and connecting it to the material's Base Color input instead of a flat color.

**Requirements**

- A basic material created, correctly saved into the `Materials` folder, and applied inside Unreal
- Roughness/Metallic values set intentionally, not left at default
- Optional: an imported texture connected to the material

---

## Checkpoint 5 — Reflection

**✏️ Answer:**

1. What went wrong (if anything) the first time you imported your asset, and how did you fix it?
2. Which method of correcting the scale mismatch felt most reliable, and why?
3. How did the naming/saving habits from Challenges F1–F2 actually help once you got here — or where did you wish you'd been more careful?
4. How did building a material in Unreal compare to building one in Blender's Shader Editor?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Exported FBX File**

Filename: `LastName_ANI2020_F3_Asset.fbx`

**Unreal Project Folder (zipped) or Screenshot Set**

Filename: `LastName_ANI2020_F3_UnrealProject.zip` (or a folder of clearly labeled screenshots if your class doesn't submit full Unreal projects)

**Before/After Scale Fix Screenshots**

Filename: `LastName_ANI2020_F3_ScaleFix_Before.png`, `_After.png`

**Reflection Document**

Filename: `LastName_ANI2020_F3_Reflection.pdf`

---

## 📊 Assessment Criteria

**Interface Navigation & Project Setup (15%)**

- Comfortable basic navigation in the Unreal viewport
- Content Browser organized with a sensible folder structure before importing began
- Clear understanding shown of Unreal's default unit scale

**Export/Import Pipeline (35%)**

- Transforms correctly applied before export
- FBX exported and named clearly with a version number
- Asset successfully imported into Unreal and sorted into the correct folder
- Scale mismatch correctly identified and resolved

**Material Application (25%)**

- Material created, correctly organized, and applied inside Unreal
- Roughness/Metallic set with clear intent
- Optional texture import attempted where applicable

**Reflection (25%)**

- Thoughtful, specific reflection on the process
- Honest account of the scale-fix troubleshooting
- Clear, specific evaluation of whether the F1–F2 naming/saving habits actually paid off here
- Fair comparison between Blender's and Unreal's material workflows

---

## 💡 Key Lesson

The export/import pipeline is where a huge amount of real-world production trouble happens — scale mismatches, broken texture links, missing materials. Getting comfortable with this exact process now means the rest of this unit, and Grade 12's more advanced Unreal work, starts from a place of confidence, not confusion.
