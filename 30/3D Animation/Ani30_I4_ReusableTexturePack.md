# 3D Animation 12 – Reusable Texture Pack: Build Once, Deploy Anywhere

## Unit 3: Hard-Surface Modeling, Texturing & Look Development — Challenge I4 (Unit Capstone)

**Stream:** Differentiated — Animation stream and Game Art stream, converging on the same portable deliverable
**Time:** 1.5–2 Weeks (5–6 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenges I1–I3.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Design a cohesive, themed set of 4–6 materials meant to be reused, not built for one single object
- Produce portable, real texture image files (not just a Blender-only procedural setup) that can be dropped into a new Blender project or Unreal level
- Build a reusable master material (Blender) and/or parent material with instances (Unreal) so the pack can be applied quickly to new geometry
- Prove the pack's portability by actually deploying it — ideally to redress their Challenge H4 level

This is the unit capstone — the goal is a real, deployable asset pack, not a one-off textured object. A good pack here means you could reskin your H4 level into a completely different-feeling place just by swapping materials.

---

## 💭 Production Question

### What separates a material you built for one object from a material pack someone else could pick up and use on a project you've never seen?

---

## Checkpoint 1 — Pack Concept & Planning (Day 1)

**📖 Plan a Cohesive Pack**

1. Choose a clear visual theme for your pack — ideally one that would suit your Challenge H4 level's genre, or a contrasting theme you could use to reskin it into something different (e.g., "Rusted Industrial," "Alien Ruins," "Clean Sci-Fi Lab," "Damp Stone Dungeon").
2. Gather 3–5 reference images that define the theme clearly.
3. Plan 4–6 distinct materials your pack needs to feel complete and usable — think in terms of what a level actually needs: a wall material, a floor material, a trim/detail material, a prop material, and an accent material (something emissive or distinct, like a warning light or glowing panel).
4. For each planned material, note whether it will be built via advanced Blender shading (Animation stream) or Substance Painter (Game Art stream), and what makes it visually distinct from the others in the pack.

**Requirements**

- A clear, describable theme
- 4–6 planned materials, each with a distinct role (wall, floor, trim, prop, accent, etc.)
- Reference gathered to guide the pack's consistent look

---

## Checkpoint 2 — Building & Exporting Portable Textures (Days 2–4)

**✏️ Create Real, Portable Texture Files**

**Animation stream:**
1. Build each material using Blender's Shader Editor, reusing Node Groups from Challenge I2 where it saves time across similar materials.
2. Apply each material to a simple reference object (a plane or cube) — this becomes your "bake target."
3. Use Blender's Bake panel (Render Properties → Bake, Cycles required for baking) to bake each material's Base Color, Roughness, Metallic, and Normal into real image files. This turns a Blender-only procedural setup into something portable to any engine.
4. Save each baked texture with clear, consistent naming (e.g., `Metal_Rusted_BaseColor.png`, `Metal_Rusted_Normal.png`, `Metal_Rusted_Roughness.png`).

**Game Art stream:**
1. Texture each material on a simple reference object (a plane or cube) in Substance Painter, the same way you would a real asset in Challenge I3.
2. Export each material's full texture set using your Unreal-appropriate channel-packing preset from Challenge I3.
3. Save each exported texture set with clear, consistent naming matching your pack's material names.

**Requirements**

- All 4–6 planned materials have real, exported texture image files (not left as Blender-only procedural setups)
- Consistent naming convention applied across every material's files
- Each material is visually distinct and matches its planned role

---

## Checkpoint 3 — Building Reusable Master Materials (Days 4–5)

**✏️ Make the Pack Actually Plug-and-Play**

1. In Blender, build one master material using a Node Group (from Challenge I2) with exposed Base Color, Roughness, Metallic, and Normal texture inputs — this lets you plug in any of your pack's baked textures without rebuilding the node setup each time.
2. In Unreal, build one parent Material (using your Challenge H1 Material Instance skills) with the same exposed texture inputs, then create one Material Instance per pack material, plugging in your exported textures for each.
3. Test your master material/parent material by quickly swapping between two different pack materials on the same test object — this should take seconds, not minutes, if it's built correctly.

**Requirements**

- One reusable master material built in Blender using a Node Group with exposed texture inputs
- One parent Material with a Material Instance built in Unreal for each pack material
- Swapping between pack materials on a test object is fast and requires no node-graph rebuilding

---

## Checkpoint 4 — Deployment & Portability Test (Days 5–6)

**✏️ Prove It Actually Works Somewhere Else**

1. Open your Challenge H4 level (or a new Blender scene, if your teacher prefers a Blender-side test) and apply your new pack's materials to redress it — swap out existing wall/floor/prop materials for your pack's Material Instances.
2. Note how much of the level's mood changes just from this material swap, without touching any geometry or lighting.
3. If time allows, do a second quick test: apply the same pack to a completely different, simple test scene to confirm it isn't secretly dependent on anything specific to your H4 level.
4. Document how long the redress took, and whether anything didn't port over cleanly (a texture that looked stretched on new geometry, a scale mismatch, etc.).

**Requirements**

- Pack successfully applied to redress an existing level or scene
- Clear documentation (screenshots, before/after) of the mood change achieved through material swapping alone
- Any portability issues encountered are honestly documented, along with how (or whether) they were resolved

---

## Checkpoint 5 — Packaging & Documentation (Day 6)

**✏️ Package Your Pack for Someone Else to Use**

1. Organize your final folder structure clearly: a `Textures` folder (or per-material subfolders), a `Materials` folder for your Blender master material and Unreal parent material/instances.
2. Create a simple one-page pack sheet — a pack name, your theme description, and a thumbnail grid showing all 4–6 materials with their names, as if this were a product page for an asset store.
3. Write a short note on intended use (what kind of level/scene this pack suits).

**Requirements**

- Clean, organized folder structure
- A one-page pack sheet with thumbnails and names for every material
- A short intended-use note

---

## Checkpoint 6 — Reflection

**✏️ Answer:**

1. What made a material "reusable" versus just "good" — what specifically did you have to think about differently?
2. What happened when you deployed the pack onto your H4 level — did anything not port over cleanly, and how did you handle it?
3. Which single material in your pack do you think is the most versatile, and why?
4. If you built a second pack next month, what would you do differently based on this experience?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File (master material + baked textures)**

Filename: `LastName_ANI3030_I4_TexturePack.blend`

**Exported Texture Files (organized folder)**

Filename: `LastName_ANI3030_I4_Textures/` (folder containing all material texture sets, clearly named)

**Unreal Project or Material/Instance Export**

Filename: `LastName_ANI3030_I4_UnrealMaterials.zip`

**Deployment Test Screenshots (before/after redress)**

Filename: `LastName_ANI3030_I4_Deploy_Before.png`, `_After.png`

**Pack Sheet**

Filename: `LastName_ANI3030_I4_PackSheet.pdf`

**Reflection Document**

Filename: `LastName_ANI3030_I4_Reflection.pdf`

---

## 📊 Assessment Criteria

**Pack Concept & Cohesion (10%)**

- Clear, describable theme
- 4–6 materials each with a distinct, sensible role
- Materials feel like they belong together as one cohesive pack

**Texture Creation & Portability (25%)**

- All materials exported as real, portable texture image files
- Consistent naming convention applied throughout
- Texture quality is clean, with no baking or export artifacts
- Each material is visually distinct and matches its planned role

**Master Material / Instance Setup (25%)**

- Reusable master material built in Blender with exposed texture inputs
- Parent Material and Instances correctly built in Unreal
- Swapping between pack materials is fast and requires no rebuilding
- Setup is genuinely reusable, not just technically functional once

**Deployment & Portability Test (15%)**

- Pack successfully applied to redress an existing level or scene
- Clear before/after documentation of the mood change achieved
- Portability issues honestly documented and addressed where possible

**Documentation & Packaging (10%)**

- Clean, organized folder structure
- Clear, professional-looking pack sheet with thumbnails
- Intended use clearly described

**Reflection (15%)**

- Thoughtful, specific reflection on the whole process
- Clear articulation of what "reusable" actually required
- Honest account of any portability issues and how they were resolved
- Specific idea for improving a future pack

---

## 💡 Key Lesson

A single beautiful material is a nice exercise. A pack of materials someone else — or future you, on a different project — can pick up and deploy in minutes is an actual production asset. This is exactly the kind of thinking that lets your Challenge H4 level become three or four completely different-feeling levels just by swapping in a new pack, with zero new modeling required.
