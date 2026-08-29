# 3D Animation 11 – Sculpting & Retopology

## Unit 1: Character Refinement, Storyboarding & Animation Principles — Challenge C1

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*

*Reinforces sculpting/UV skills first introduced in Gr10. Note: swap `ANI2020` in the filenames below for your actual course code.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Use sculpt brushes to add organic detail to a character (Draw, Clay Strip, Smooth, Crease)
- Use the Multires modifier and/or Dyntopo to sculpt at increasing levels of detail
- Retopologize a sculpted mesh back into a clean, animation-ready mesh
- Understand why sculpt detail and animation-ready topology are two different things

---

## 💭 Production Question

### How do you add real detail to a character without destroying its ability to move?

---

## Checkpoint 1 — Sculpting Warm-Up (Day 1)

**📖 Brush Practice**

1. Add a simple Sphere or Cube and add a Multires modifier (Modifier Properties → Add Modifier → Multires).
2. Click "Subdivide" on the Multires modifier 2–3 times to add sculptable resolution.
3. Enter Sculpt Mode and try the Draw brush (adds volume), Clay Strip (builds up flatter, blocky volume), Smooth (Shift while sculpting, or the Smooth brush), Crease (carves sharp lines), and Inflate (puffs out a surface).
4. Practice increasing and decreasing brush Strength and Radius using the tool settings or the F key (radius) and Shift+F (strength) shortcuts.
5. Try Dyntopo (Sculpt Mode → enable Dynamic Topology) on a separate test object and compare it to the Multires workflow — note how Dyntopo adds geometry on the fly wherever you sculpt, while Multires uses fixed subdivision levels.

**Questions to answer:**

1. What's the difference between the Multires and Dyntopo workflows?
2. What does the Crease brush do differently from the Draw brush?
3. When would you want more Multires subdivision levels versus fewer?

---

## Checkpoint 2 — Sculpt Pass on Your Character (Days 1–2)

**✏️ Add Detail to Your Character**

1. Open your Gr10 character (or a new base mesh approved by your teacher) and add a Multires modifier.
2. Subdivide the Multires modifier enough times to allow for the level of detail you want (usually 2–4 levels for a Grade 11 project — more levels = slower but more detail).
3. Using Draw and Clay Strip, block in larger secondary forms — muscle masses, clothing folds, larger surface details.
4. Switch to a higher Multires level and use Crease and smaller Draw brushes for finer details — wrinkles, seams, small surface texture.
5. Use the Smooth brush regularly to blend transitions and avoid overly bumpy, noisy surfaces.
6. Periodically drop back to Multires level 0 (the original low-poly cage) to check that the base silhouette still reads correctly under all the added detail.

**Requirements**

- Multires or Dyntopo used to add at least two distinct levels of detail (large forms and fine detail)
- Sculpted detail is intentional and supports the character concept, not random noise
- Base silhouette remains readable underneath the added detail

---

## Checkpoint 3 — Retopology (Days 2–3)

**✏️ Rebuild a Clean Mesh**

1. Add a new mesh object (a Plane or a duplicate of your low-poly base) to use as your retopology starting point.
2. Add a Shrinkwrap modifier to this new object, targeting your sculpted high-detail mesh, so any geometry you build automatically snaps to the sculpt's surface.
3. Using the Poly Build tool (or manual Extrude/Merge in Edit Mode with snapping enabled), build a clean, evenly-spaced mesh over the sculpt, following the surface's major forms.
4. Pay special attention to edge flow around areas that will need to bend or deform (joints, face, mouth) — loops should flow around these areas, not through them at odd angles.
5. Once your retopologized mesh covers the sculpt, apply the Shrinkwrap modifier so the new mesh is baked into place.
6. Compare your new retopologized mesh's poly count to your original sculpt's poly count — it should be dramatically lower while still capturing the major shapes.

**Requirements**

- Clean, evenly-spaced retopologized mesh built over the sculpt
- Edge flow follows deformation areas (joints, face) sensibly
- Final poly count is animation-appropriate, not sculpt-resolution

---

## Checkpoint 4 — Deformation Test (Day 3)

**✏️ Test Your New Mesh**

1. Add a simple test armature (a few bones is enough — doesn't need to be your full rig) to your retopologized mesh.
2. Parent the mesh to the armature with Automatic Weights.
3. Pose-test a joint area (an elbow, a knee, or the face if applicable) and check that the retopologized mesh deforms cleanly — this is the real test of whether your retopology worked.
4. If deformation looks bad in a specific spot, go back into Edit Mode and adjust edge flow in that area, then re-test.

**Requirements**

- At least one joint area tested for clean deformation
- Any deformation problems found are documented and, where possible, fixed

---

## Checkpoint 5 — Reflection

**✏️ Answer:**

1. What was the biggest difference between sculpting freely and modeling with topology in mind?
2. Where did your retopology attempt struggle the most, and why?
3. How did the deformation test change your understanding of "good" topology?
4. If you sculpted this character again, what would you do differently at the blocking stage?
5. How does this relate back to the edge-loop placement you practiced in Grade 10?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI2020_C1_SculptRetopo.blend`

**Sculpt Detail Renders (2, showing before/after sculpt pass)**

Filename: `LastName_ANI2020_C1_Sculpt_Before.png`, `LastName_ANI2020_C1_Sculpt_After.png`

**Deformation Test Screenshot**

Filename: `LastName_ANI2020_C1_DeformTest.png`

**Reflection Document**

Filename: `LastName_ANI2020_C1_Reflection.pdf`

---

## 📊 Assessment Criteria

**Sculpting Quality (30%)**

- Detail added at multiple distinct levels (large forms and fine detail)
- Sculpted detail supports the character concept rather than looking random
- Effective use of at least three different brush types
- Base silhouette remains readable underneath the sculpted detail

**Retopology Quality (35%)**

- Clean, evenly-spaced mesh built over the sculpt
- Edge flow sensibly follows joints and deformation areas
- Poly count dramatically reduced from sculpt resolution to an animation-appropriate level
- No stray, overlapping, or non-manifold geometry left in the final mesh

**Deformation Testing (20%)**

- At least one joint area tested with a simple armature
- Deformation problems identified honestly, not glossed over
- Evidence of at least one fix attempted based on test results
- Clear before/after comparison documented

**Reflection (15%)**

- Thoughtful, specific reflection on the sculpt-to-retopology process
- Honest identification of the hardest part of retopology
- Clear connection drawn back to Grade 10 edge-loop concepts
- Concrete idea for improving the blocking stage next time

---

## 💡 Key Lesson

Sculpting and retopology are two separate skills that solve two separate problems: sculpting is about expression and detail, retopology is about function and performance. Professional characters almost always go through both steps — this is your first real practice with that full pipeline.
