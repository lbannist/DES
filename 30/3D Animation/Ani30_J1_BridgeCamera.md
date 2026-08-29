# 3D Animation 12 – The Bridge & The Camera

## Unit 4: Real-Time Sequencing & Technical Animation — Challenge J1

**Time:** 1 Week (3–4 Class Periods)
**Due Date:** *[insert due date]*

*Brings together your rigged character (Unit 1), textures (Unit 3), and Unreal fundamentals (Unit 2).*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Export a rigged character correctly from Blender for use as a Skeletal Mesh in Unreal
- Import a character into Unreal and assign it materials/textures built earlier this year
- Create a Level Sequence, add a Cine Camera, and animate a basic camera track that frames the character
- Compare how a character reads under Blender's render versus Unreal's real-time lighting

---

## 💭 Production Question

### What has to survive the trip from Blender to Unreal for a rigged, textured character to still look like your character?

---

## Checkpoint 1 — Character Export Prep (Day 1)

**✏️ Prepare Your Rig for Export**

1. Open your Challenge G1/G4 character and confirm the armature and mesh are both clean — no leftover unused bones, no unapplied modifiers that would break on export.
2. Unlike exporting a static prop, do **not** apply the armature's transforms the same way — check that your rig has a clear root bone at the origin, since Unreal needs this to read the skeleton correctly.
3. In the FBX export settings, make sure "Armature" and the relevant animation/action data are included in the export (check "Bake Animation" if you're exporting an existing action like a walk cycle).
4. Export your rigged character as an FBX, using a clear, version-numbered filename.

**Requirements**

- Armature and mesh exported cleanly with a proper root bone
- Animation/action data included in the export if applicable
- File named clearly with a version number

---

## Checkpoint 2 — Importing as a Skeletal Mesh (Day 1–2)

**✏️ Bring Your Character into Unreal**

1. In Unreal's Content Browser, import your FBX — check that it imports as a Skeletal Mesh (not a Static Mesh), which confirms the armature came through correctly.
2. Open the imported Skeletal Mesh and check the Skeleton tree matches your Blender armature's bone structure.
3. Create or reuse a Material (drawing on your Challenge H1 Material Instance skills) using your Challenge I-series textures, and assign it to the Skeletal Mesh's material slots.
4. Place your character in a test level and confirm it appears correctly — textured, at the right scale, with no missing material slots showing the default grey/checker material.

**Requirements**

- Character correctly imported as a Skeletal Mesh
- Skeleton structure matches the original Blender armature
- Unit 3 textures/materials correctly assigned to all material slots
- No missing materials or scale issues in the test level

---

## Checkpoint 3 — Sequencer Camera Setup (Day 2–3)

**✏️ Frame Your Character with a Camera**

1. Create a new Level Sequence and add a Cine Camera Actor to it as a track.
2. Pose your character (if it has a static pose or simple animation available) so there's something worth framing.
3. Keyframe the camera's position/rotation to create a simple, deliberate camera move — a slow push-in, an arc around the character, or a reveal from an interesting angle.
4. Adjust the Cine Camera's Focal Length and Depth of Field for a considered, presentation-quality shot rather than a default flat view.

**Requirements**

- A Level Sequence with an animated camera track
- Camera movement is deliberate and framed with intent, not a random default angle
- Focal length/depth of field adjusted for a presentation-quality look

---

## Checkpoint 4 — Real-Time Lighting Comparison (Day 3)

**✏️ Compare Blender vs. Unreal**

1. Render a still of your character in Blender (reusing earlier lighting setups if helpful) and a still of the same character in your Unreal scene, from a similar angle.
2. Compare the two side by side — note differences in how materials, shadows, and overall mood read between the offline Blender render and Unreal's real-time lighting.
3. Adjust your Unreal lighting if something reads noticeably worse than it did in Blender (e.g., a material that looked correct in Blender but appears too flat or too shiny in Unreal).

**Requirements**

- A side-by-side comparison render/screenshot produced
- At least two specific differences identified between the two renders
- Any significant discrepancy addressed with a lighting or material adjustment in Unreal

---

## Checkpoint 5 — Reflection

**✏️ Answer:**

1. What went wrong (if anything) the first time you exported/imported your rig, and how did you fix it?
2. What was the biggest visual difference between your Blender render and your Unreal real-time render?
3. How did framing a shot in Sequencer feel different from framing a shot in Blender's camera view?
4. What are you hoping to do with this character's movement in Challenge J2?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Exported FBX (character + skeleton)**

Filename: `LastName_ANI3030_J1_CharacterExport.fbx`

**Unreal Project Folder (zipped)**

Filename: `LastName_ANI3030_J1_UnrealProject.zip`

**Sequencer Camera Render**

Filename: `LastName_ANI3030_J1_CameraSequence.mp4`

**Blender vs. Unreal Comparison Renders**

Filename: `LastName_ANI3030_J1_Comparison_Blender.png`, `_Unreal.png`

**Reflection Document**

Filename: `LastName_ANI3030_J1_Reflection.pdf`

---

## 📊 Assessment Criteria

**Export & Import Pipeline (30%)**

- Rig exported cleanly with a proper root bone and correct armature data
- Character correctly imported as a Skeletal Mesh with a matching skeleton
- No broken bones, scale issues, or missing skeleton data

**Material Assignment (20%)**

- Unit 3 textures/materials correctly applied to all material slots
- No default/missing material slots visible in the final scene
- Materials read correctly at the character's in-engine scale

**Sequencer Camera Work (30%)**

- Camera movement is deliberate and well-composed
- Focal length/depth of field used with clear intent
- Shot quality is presentation-ready, not a default/flat angle

**Lighting Comparison & Reflection (20%)**

- Clear, specific comparison made between Blender and Unreal renders
- At least two genuine differences identified and explained
- Reflection shows real engagement with the export/import troubleshooting process

---

## 💡 Key Lesson

Getting a rigged, textured character correctly into a real-time engine is the single most failure-prone step in this whole pipeline — small mistakes here (a bad root bone, a missing material) cascade into every assignment that follows this one. Getting it right now means Challenges J2 and J3 can focus on the actually interesting parts: making that character move and perform.
