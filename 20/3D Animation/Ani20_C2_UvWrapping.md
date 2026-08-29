# 3D Animation 11 – UV Unwrapping

## Unit 1: Character Refinement, Storyboarding & Animation Principles — Challenge C2

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*

*Reinforces UV skills first introduced in Gr10.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Mark seams deliberately based on natural breaks in a model
- Compare Smart UV Project against manual seam-and-unwrap workflows
- Check unwraps for stretching and overlap using a UV checker texture
- Pack UV islands efficiently to make good use of texture space

---

## 💭 Production Question

### Where would you cut this model if you wanted the seams to disappear?

---

## Checkpoint 1 — Seam Planning (Day 1)

**📖 Plan Your Seams**

1. Select your retopologized character from Challenge C1 (or another approved model) and study it in Edit Mode.
2. Identify natural "hidden" locations for seams — places that won't be very visible, like the underside of arms, the inseam of legs, behind the ears, or along a natural hairline.
3. Sketch or annotate a screenshot of your model showing where you plan to place seams, and why you chose those locations.
4. Predict which parts of your model will be hardest to unwrap without stretching (tight curves, areas with lots of small detail).

**Questions to answer:**

1. Why do "hidden" seam locations matter for a finished character?
2. Which part of your model do you predict will be hardest to unwrap cleanly, and why?

---

## Checkpoint 2 — Marking Seams & Unwrapping (Days 1–2)

**✏️ Unwrap Your Model**

1. In Edit Mode, select edge loops along your planned seam locations and mark them as seams (Edge menu → Mark Seam, or Ctrl+E → Mark Seam).
2. Select the whole mesh (A) and try Smart UV Project first (U → Smart UV Project) — open the UV Editor to see the result.
3. Now undo, and instead select the whole mesh and try U → Unwrap, using your marked seams — compare the result to the Smart UV Project version in the UV Editor.
4. Note which method gave cleaner, more predictable islands for your specific model.
5. If any single island looks messy or overly stretched, consider adding an additional seam in that specific area and re-unwrapping just that section.

**Requirements**

- Seams marked deliberately, not just auto-generated everywhere
- Both Smart UV Project and manual seam-and-unwrap attempted and compared
- Final unwrap uses whichever method produced cleaner results for this model

---

## Checkpoint 3 — UV Checker Test & Island Packing (Days 2–3)

**✏️ Check and Pack Your UVs**

1. Apply a UV checker texture (a grid or checkerboard image) to your model's material so you can see the UVs directly on the 3D surface.
2. Rotate around your model in the 3D viewport and look for areas where the checker pattern stretches, squishes, or distorts — these indicate UV problems.
3. Go back into the UV Editor and identify which island corresponds to each stretched area; adjust seams or manually relax/straighten the island as needed.
4. Once individual islands look clean, use UV → Pack Islands in the UV Editor to arrange all islands efficiently within the 0–1 UV space.
5. Check that islands aren't overlapping (unless intentionally mirrored, e.g., left/right symmetrical body parts sharing UV space) and that there's reasonable, even spacing between islands for later texture painting.

**Requirements**

- UV checker texture used to visually verify the unwrap
- Any significant stretching identified and corrected
- Islands packed efficiently with no unintended overlaps

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. Which method (Smart UV Project or manual seams) worked better for your model, and why?
2. Where did you find the most stretching, and how did you fix it?
3. What did the UV checker texture reveal that you couldn't see just by looking at the UV layout alone?
4. How did you decide where to place additional seams if your first attempt wasn't clean?
5. How will good UVs affect the texturing work you'll do in Challenge E-series (Material Creation & Texturing) later this year?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI2020_C2_UVUnwrap.blend`

**UV Layout Screenshot**

Filename: `LastName_ANI2020_C2_UVLayout.png`

**Checker Texture Test Renders (2, showing at least two viewing angles)**

Filename: `LastName_ANI2020_C2_CheckerTest_01.png`, `_02.png`

**Reflection Document**

Filename: `LastName_ANI2020_C2_Reflection.pdf`

---

## 📊 Assessment Criteria

**Seam Placement (25%)**

- Seams placed deliberately in hidden/logical locations
- Seams follow natural breaks in the model (limbs, clothing edges, hairline)
- Number of seams is reasonable — not excessive, not too few to unwrap cleanly
- Evidence of planning shown in Checkpoint 1 matches the final seam placement

**Unwrap Quality (30%)**

- Minimal visible stretching when checked with the UV checker texture
- Both unwrap methods attempted and compared before choosing a final approach
- UV islands are logically grouped and easy to navigate
- No flipped or inside-out UV islands

**Island Packing (25%)**

- Islands packed efficiently within the 0–1 UV space
- No unintended overlaps between islands
- Reasonable, even spacing between islands
- Efficient use of texture space without islands being too small to paint on accurately

**Reflection (20%)**

- Thoughtful, specific reflection on the process
- Clear explanation of where and why stretching occurred
- Honest comparison between the two unwrap methods tried
- Concrete connection drawn to upcoming texturing work

---

## 💡 Key Lesson

Every texture you paint or bake later this year is only as good as the UVs underneath it. A clean, well-planned unwrap now means fewer headaches — and much better-looking textures — in the Material Creation & Texturing unit.
