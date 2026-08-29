# 3D Animation 12 – Substance Painter Workflows

## Unit 3: Hard-Surface Modeling, Texturing & Look Development — Challenge I3

**Stream:** Skills Alberta 3D Digital Game Art track
**Time:** 1.5 Weeks (4 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenge I1's hard-surface prop.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Import a mesh and baked maps into Substance Painter
- Use Smart Materials and Smart Masks to speed up realistic texturing
- Hand-paint fine details using layers and masks
- Export a properly channel-packed texture set for use in Unreal Engine

---

## 💭 Production Question

### How do you make a game asset look "used" without it looking randomly dirty?

---

## Checkpoint 1 — Import & Baking (Day 1)

**📖 Set Up Your Project**

1. Export your Challenge I1 hard-surface prop from Blender as an FBX, making sure UVs are clean (revisit Gr11 Challenge C2 if needed).
2. Create a new project in Substance Painter, importing your mesh at the correct resolution/template settings for your prop's complexity.
3. Bake your texture maps (Normal, Ambient Occlusion, Curvature, Position) using Substance Painter's baking panel — this uses your high-to-low modeling detail (bevels, edge flow) to generate useful maps automatically.
4. Review the baked maps individually (toggle each on/off in the Texture Set list) and check for baking errors (black spots, seams, artifacts).

**Questions to answer:**

1. What does the Curvature map actually show, and why is it useful for adding wear later?
2. Did you find any baking errors, and if so, what caused them?

---

## Checkpoint 2 — Smart Materials & Masks (Days 1–2)

**✏️ Apply Base Materials**

1. Apply a Smart Material appropriate to your prop's base material (metal, plastic, painted surface) from Substance Painter's library.
2. Observe how the Smart Material automatically uses your baked Curvature and AO maps to place wear, dirt, and edge damage in believable locations.
3. Adjust the Smart Material's generator settings (edge wear amount, dirt amount) to fit your prop's intended condition (brand new vs. heavily used).
4. Add a second Smart Material layer for a different material area (e.g., a rubber grip, a different metal type) using layer masks to control where each material appears.

**Requirements**

- At least one Smart Material applied and adjusted from default settings
- A second material area added using layer masks
- Wear/dirt placement looks logical given the prop's shape (not randomly placed)

---

## Checkpoint 3 — Hand-Painted Detail Pass (Days 2–3)

**✏️ Add Custom Detail**

1. Add a new paint layer above your Smart Materials.
2. Hand-paint at least one custom detail not achievable by the Smart Materials alone — a stencil/decal, a specific scratch pattern, a maker's mark or serial number, localized paint chipping.
3. Use layer masks and blend modes to integrate your painted detail naturally with the material layers beneath it.
4. Zoom in and check that your painted details follow the UV seams correctly with no visible stretching or misalignment.

**Requirements**

- At least one genuine hand-painted detail added
- Detail integrated naturally with existing material layers via masks
- No visible UV seam issues in the painted areas

---

## Checkpoint 4 — Export for Unreal (Day 4)

**✏️ Export Your Texture Set**

1. Set up an export preset appropriate for Unreal Engine (Substance Painter includes an "Unreal Engine 4/5" export preset — check with your teacher which channel-packing convention your class uses).
2. Export your texture maps (Base Color, Normal, and a packed Occlusion/Roughness/Metallic map, or your class's specific convention).
3. Import the resulting textures into your Unreal project (from Unit 2) and apply them to your prop's material.
4. Confirm the prop looks correct in Unreal — check for inverted channels or incorrect map assignments if something looks wrong (e.g., roughness appearing inverted).

**Requirements**

- Textures exported using an Unreal-appropriate channel-packing preset
- Textures successfully imported and applied in Unreal
- Any channel/map assignment errors identified and corrected

---

## Checkpoint 5 — Reflection

**✏️ Answer:**

1. How did the baked Curvature/AO maps make your Smart Material wear placement look more believable than manually placing it would have?
2. What was your hand-painted detail, and why couldn't a Smart Material alone have achieved it?
3. What issue (if any) came up when your textures first appeared in Unreal, and how did you fix it?
4. How does this full Blender-to-Substance-Painter-to-Unreal pipeline compare to your Gr11 experience of just Blender-to-Unreal?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Substance Painter Project File**

Filename: `LastName_ANI3030_I3_SubstanceProject.spp`

**Exported Texture Set**

Filename: `LastName_ANI3030_I3_Textures/` (folder containing all exported maps)

**Final Textured Renders (from Substance Painter or Unreal, 2 angles)**

Filename: `LastName_ANI3030_I3_FinalRender_01.png`, `_02.png`

**Reflection Document**

Filename: `LastName_ANI3030_I3_Reflection.pdf`

---

## 📊 Assessment Criteria

**Baking Quality (20%)**

- Maps baked correctly with minimal errors
- Baking errors (if any) identified and addressed
- UV/mesh quality from Challenge I1 supports clean baking results

**Smart Material Application (25%)**

- At least one Smart Material applied and thoughtfully adjusted
- A second material area correctly masked and applied
- Wear/dirt placement looks logical and believable, not random

**Hand-Painted Detail (25%)**

- At least one genuine custom detail added
- Detail integrates naturally with surrounding material layers
- No visible UV seam or stretching issues in painted areas

**Export & Unreal Integration (20%)**

- Textures exported with an Unreal-appropriate preset
- Successfully imported and applied in Unreal
- Any channel/map errors identified and corrected

**Reflection (10%)**

- Thoughtful, specific reflection on the process
- Clear explanation of how baked maps improved wear placement
- Honest account of any Unreal integration troubleshooting

---

## 💡 Key Lesson

This is the exact pipeline used by working game artists — and the one Skills Alberta 3D Digital Game Art competitors need to execute quickly and reliably under competition time pressure: model with baking in mind, bake, texture with Smart Materials plus hand-painted detail, then export correctly for the target engine.
