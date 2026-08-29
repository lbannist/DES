# 3D Animation 11 – Render Engines & Settings

## Unit 2: Environment, Lighting & Rendering — Challenge D3

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenges D1–D2.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Compare Eevee and Cycles render engines and understand their trade-offs
- Adjust render samples and understand the trade-off between render time and quality
- Use basic render passes for compositing flexibility
- Manage output settings, including image sequences vs. direct video output

---

## 💭 Production Question

### Is a faster, "good enough" render always the wrong choice?

---

## Checkpoint 1 — Eevee vs. Cycles Comparison (Day 1)

**📖 Engine Comparison Test**

1. Using your Challenge D1/D2 environment, render the same camera angle once in Eevee and once in Cycles (Render Properties → Render Engine dropdown).
2. Time how long each render takes (note the time shown in the render window, or use a stopwatch).
3. Compare the two images side by side, looking specifically at reflections, shadows, and how light bounces around the scene.
4. Note at least two visual differences you can identify between the two engines' results.

**Questions to answer:**

1. Which engine was faster, and by roughly how much?
2. What visual differences did you notice between the two renders?
3. Based on this test, when would you choose Eevee over Cycles, or vice versa?

---

## Checkpoint 2 — Sample Settings & Render Time (Days 1–2)

**✏️ Test Sample Counts**

1. In Cycles, go to Render Properties → Sampling and note the current sample count.
2. Render your scene at a low sample count (e.g., 32) and note the render time and any visible noise/graininess.
3. Render the same scene at a higher sample count (e.g., 256 or higher) and note the render time and image quality.
4. Try Blender's Denoising option (enable it in the Sampling settings) at your lower sample count and compare the result to the un-denoised low-sample render.
5. Decide on a sample count that balances acceptable quality with a render time reasonable for your project's deadline.

**Requirements**

- At least two different sample counts tested and compared
- Denoising tested and compared to a non-denoised equivalent
- A final sample count chosen with a stated reason (quality vs. time trade-off)

---

## Checkpoint 3 — Render Passes & Output Management (Days 2–3)

**✏️ Set Up Render Passes and Output**

1. Go to View Layer Properties and enable at least two render passes beyond the default combined image (e.g., Shadow, Ambient Occlusion, or Diffuse/Glossy separately).
2. Render your scene and open the Compositor to view the separate passes (Shader Editor / Compositor tab, enable "Use Nodes").
3. Try a very simple compositing adjustment using one of the passes (e.g., boosting the Ambient Occlusion pass slightly using a Mix node) to see how passes can be used after rendering, without re-rendering the whole scene.
4. In Output Properties, set your file format to a PNG image sequence for a test animation render of a few frames, and separately test rendering directly to a video format (e.g., FFmpeg Video) for the same frames.
5. Compare file sizes and note any risk you can identify with rendering long animations directly to video versus an image sequence (e.g., what happens if the render crashes partway through).

**Requirements**

- At least two render passes enabled and viewed in the Compositor
- One simple compositing adjustment attempted using a pass
- Both image sequence and direct video output tested and compared

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. Based on your Checkpoint 1 test, which engine would you choose for a fast preview vs. a final render, and why?
2. What sample count did you settle on, and what was your reasoning?
3. What did having separate render passes let you do that you couldn't do with just the combined image?
4. Why might rendering to an image sequence be safer than rendering directly to video for a long animation?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI2020_D3_RenderSettings.blend`

**Eevee vs. Cycles Comparison Renders**

Filename: `LastName_ANI2020_D3_Eevee.png`, `LastName_ANI2020_D3_Cycles.png`

**Sample Count Comparison Renders**

Filename: `LastName_ANI2020_D3_LowSample.png`, `LastName_ANI2020_D3_HighSample.png`

**Reflection Document**

Filename: `LastName_ANI2020_D3_Reflection.pdf`

---

## 📊 Assessment Criteria

**Engine Comparison (25%)**

- Both Eevee and Cycles rendered from the same camera angle
- Render times documented and compared
- At least two specific visual differences identified
- Reasonable, well-justified conclusion about when to use each engine

**Sample Settings & Render Time (25%)**

- At least two different sample counts tested and compared
- Denoising tested and its effect clearly documented
- Final sample count choice is reasonable and justified
- Understanding shown of the quality vs. time trade-off

**Render Passes & Output (30%)**

- At least two render passes enabled and correctly viewed in the Compositor
- A genuine compositing adjustment attempted using a pass
- Both image sequence and video output tested
- Clear understanding shown of the risk trade-off between output formats

**Reflection (20%)**

- Thoughtful, specific reflection on the process
- Clear, accurate reasoning for engine choice in different situations
- Honest account of the sample count decision
- Clear explanation of the image sequence vs. video output trade-off

---

## 💡 Key Lesson

Render settings are a budget, not a checkbox — every project has a fixed amount of time, and the choices made here (engine, samples, output format) determine whether that time goes toward quality, iteration speed, or safety against crashes. This budgeting mindset becomes critical once render deadlines get tighter in Grade 12 competition prep.
