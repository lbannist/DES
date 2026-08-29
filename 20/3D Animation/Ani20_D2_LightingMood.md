# 3D Animation 11 – Lighting Theory & Mood

## Unit 2: Environment, Lighting & Rendering — Challenge D2

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenge D1.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Set up classic three-point lighting (key, fill, rim)
- Use HDRI environment textures for realistic ambient light and reflections
- Adjust color temperature intentionally to shift mood
- Simulate different times of day through lighting choices alone

---

## 💭 Production Question

### Using the exact same environment, how many different moods can lighting alone create?

---

## Checkpoint 1 — Three-Point Lighting Setup (Day 1)

**📖 Key, Fill, and Rim**

1. Add a Key light (your main, brightest light source) and position it at roughly a 45-degree angle to your subject.
2. Add a Fill light (softer, dimmer, opposite side from the key) to soften the shadows the key light creates — set its Strength noticeably lower than the key.
3. Add a Rim light (positioned behind or to the side of the subject, aimed back toward the camera) to create a highlight edge that separates the subject from the background.
4. Render a test image and identify each light's contribution by temporarily disabling each one (click the light bulb icon next to each light in the Outliner) and re-rendering.

**Questions to answer:**

1. What job does each of the three lights (key, fill, rim) do differently?
2. What happened to the image when you disabled the fill light? The rim light?

---

## Checkpoint 2 — HDRI & World Lighting (Days 1–2)

**✏️ Add HDRI Environment Lighting**

1. Go to World Properties and change the Color input from a flat color to an Environment Texture.
2. Load an HDRI image (check with your teacher for available class HDRIs, or use a free/education-appropriate source).
3. Rotate the HDRI (using the Mapping node, or the World's rotation controls) until the lighting direction complements your three-point setup rather than fighting it.
4. Adjust the HDRI's Strength value and compare renders at a few different strengths to see how it affects overall ambient light and reflections.
5. Turn off your three-point lights temporarily and render using only the HDRI — note how much of the lighting work the HDRI alone can do.

**Requirements**

- HDRI environment texture applied and rotated intentionally
- HDRI strength adjusted and compared at more than one value
- Clear understanding shown of what the HDRI contributes versus the three-point lights

---

## Checkpoint 3 — Mood & Time-of-Day Variations (Days 2–3)

**✏️ Create Three Distinct Moods**

1. Using the same base scene, create three different lighting setups representing different moods or times of day (e.g., warm sunset, cool overcast day, dramatic moonlit night).
2. For each, adjust light color temperature (warmer oranges/yellows vs. cooler blues), light strength, and HDRI choice/rotation as needed.
3. Render one image per mood, keeping the camera angle identical across all three so the only variable is lighting.
4. Compare all three renders side by side and check that each mood is clearly distinguishable from the others.

**Requirements**

- Three distinct lighting moods created from the same base scene and camera angle
- Color temperature clearly and intentionally adjusted between moods
- Each mood is clearly identifiable/describable at a glance

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. What did disabling each light in the three-point setup teach you about its specific job?
2. How much of your final look came from the three-point lights versus the HDRI?
3. Which of your three mood variations do you think is strongest, and why?
4. What would you do differently if you had to create a fourth, completely different mood from this same scene?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI2020_D2_Lighting.blend`

**Three-Point Light Breakdown Renders (key only, key+fill, key+fill+rim)**

Filename: `LastName_ANI2020_D2_Breakdown_01.png` through `_03.png`

**Three Mood Renders**

Filename: `LastName_ANI2020_D2_Mood_Sunset.png`, `_Overcast.png`, `_Night.png` (or your chosen mood names)

**Reflection Document**

Filename: `LastName_ANI2020_D2_Reflection.pdf`

---

## 📊 Assessment Criteria

**Three-Point Lighting Setup (25%)**

- Key, fill, and rim lights each clearly present and doing their intended job
- Fill light noticeably softer/dimmer than the key light
- Rim light creates a visible separating highlight on the subject
- Breakdown renders clearly demonstrate each light's individual contribution

**HDRI & World Lighting (25%)**

- HDRI applied and rotated to complement the lighting setup
- Strength tested and compared at more than one value
- HDRI-only test render shows clear understanding of its contribution
- HDRI choice/rotation supports the scene's intended mood

**Mood Variation (30%)**

- Three genuinely distinct, identifiable moods created
- Color temperature clearly and intentionally shifted between moods
- Camera angle held constant so lighting is the only variable
- All three renders are technically clean (no blown highlights or unreadable black areas, unless intentional)

**Reflection (20%)**

- Thoughtful, specific reflection on the process
- Clear, accurate explanation of each three-point light's role
- Honest assessment of which mood variation was strongest and why
- Concrete idea for a fourth mood variation

---

## 💡 Key Lesson

The same three-point framework used here is the industry-standard starting point for almost all lighting work — in Blender, in live-action film, and eventually in Unreal Engine. Understanding what each light contributes means you can troubleshoot lighting problems instead of just guessing.
