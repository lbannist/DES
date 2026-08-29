# 3D Animation 12 – Content Organization & Material Instances

## Unit 2: Advanced Unreal Engine — Challenge H1

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Gr11's Unreal intro (Challenges F3–F5).*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Organize a multi-asset Unreal project using a clear Content Browser folder structure
- Import multiple assets efficiently into one organized pipeline
- Create and use Material Instances to adjust materials without duplicating shader graphs

---

## 💭 Production Question

### How do you keep a growing Unreal project from turning into an unmanageable mess?

---

## Checkpoint 1 — Multi-Asset Import & Organization (Day 1)

**✏️ Set Up Your Project Structure**

1. Create a new Unreal project (or continue your Gr11 Challenge F5 project) and set up a clear top-level folder structure in the Content Browser: `Meshes`, `Materials`, `Textures`, `Blueprints`, `Levels`.
2. Export and import at least 4–5 assets from your Blender work (props, environment pieces, or a character), following your Gr11 export/scale-correction process.
3. Sort each imported asset into its correct folder as it comes in, rather than leaving everything in the default import location.
4. Rename assets clearly and consistently (e.g., `SM_Rock_01` for a static mesh, `M_Rock_Base` for a material) — check with your teacher for any class-specific naming convention.

**Requirements**

- At least 4–5 assets imported and correctly organized into folders
- Consistent, clear naming applied to all imported assets
- Scale correctly verified for each asset

---

## Checkpoint 2 — Base Material Creation (Day 1–2)

**✏️ Build a Parent Material**

1. Create one master/parent Material with a reasonably complete node setup (Base Color, Roughness, Metallic, and a Normal map input) that could apply to multiple similar assets (e.g., a general "rock" material, or a general "metal prop" material).
2. Expose key parameters as Material Parameters (right-click a value node → Convert to Parameter) rather than hard-coding them — this is what makes Material Instances possible.
3. Apply this parent material to one of your imported assets and confirm it looks correct.

**Requirements**

- A parent material built with at least three exposed parameters
- Parent material successfully applied to at least one asset

---

## Checkpoint 3 — Material Instances (Days 2–3)

**✏️ Create and Use Instances**

1. Right-click your parent material and select "Create Material Instance."
2. Open the instance and adjust its exposed parameters (color, roughness value, texture swap) without touching the original parent material's node graph.
3. Apply this instance to a second, different asset and adjust its parameters independently from the first instance.
4. Create at least one more instance for a third asset, giving each instance a distinct look while all three share the same underlying parent material logic.
5. Make a small change to the parent material itself (e.g., add a new default input) and confirm that all instances update accordingly, demonstrating the benefit of this approach.

**Requirements**

- At least two Material Instances created from the same parent
- Each instance gives a visually distinct result via its exposed parameters
- A change to the parent material correctly propagates to all instances

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. How did organizing your Content Browser folders change how quickly you could find assets?
2. What's the practical benefit of a Material Instance over just duplicating a whole material and editing it?
3. What happened when you changed the parent material after creating instances?
4. How will this organizational approach help once your project grows larger in Challenge H4's final showcase scene?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Unreal Project Folder (zipped) or Screenshot Set**

Filename: `LastName_ANI3030_H1_UnrealProject.zip`

**Content Browser Organization Screenshot**

Filename: `LastName_ANI3030_H1_FolderStructure.png`

**Material Instance Comparison Screenshot**

Filename: `LastName_ANI3030_H1_MaterialInstances.png`

**Reflection Document**

Filename: `LastName_ANI3030_H1_Reflection.pdf`

---

## 📊 Assessment Criteria

**Project Organization (25%)**

- Clear, consistent folder structure in the Content Browser
- All imported assets correctly sorted into appropriate folders
- Consistent naming convention applied throughout
- Scale correctly verified for all imported assets

**Parent Material Construction (25%)**

- Parent material built with a reasonably complete PBR setup
- At least three parameters correctly exposed
- Parent material applied successfully to at least one asset

**Material Instance Use (35%)**

- At least two distinct Material Instances created from the same parent
- Each instance shows a genuinely different, intentional look
- Parent material update correctly propagates to all instances
- Instances used appropriately rather than duplicating whole materials unnecessarily

**Reflection (15%)**

- Thoughtful, specific reflection on the process
- Clear, accurate explanation of the Material Instance benefit
- Honest account of what happened when the parent material changed
- Concrete connection drawn to the upcoming Challenge H4 showcase scene

---

## 💡 Key Lesson

The habits built here — organized folders, consistent naming, parent materials with instances — are what keep a growing Unreal project maintainable. Skipping this now guarantees painful, avoidable chaos by the time your Challenge H4 showcase scene has dozens of assets in it.
