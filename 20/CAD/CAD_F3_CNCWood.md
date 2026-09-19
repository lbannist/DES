# CAD 11 – Validation & Reverse-Engineering Capstone

## Unit F: Validation & Reverse-Engineering Capstone — Challenge F3 (Capstone)

**Time:** 1–1.5 Weeks (4–5 Class Periods)
**Due Date:** *[insert due date]*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Combine modeling, tolerancing, fitting, and CAM into one fully independent deliverable
- Generate CAM toolpaths and CNC-route a final, improved design in a different material than the original
- Understand how a material substitution changes real-world performance
- Complete the full measure → model → validate → fabricate cycle independently, start to finish

---

## 💭 Production Question

### If the real part is metal and you're cutting it in wood, what actually changes — and what stays true regardless?

---

## Checkpoint 1 — CAM Setup for the Final Design (Days 1–2)

**✏️ Prepare Your Improved Part for CNC**

1. Using your final, improved design from Challenge F2, set up stock and WCS placement appropriate for CNC-routing in wood.
2. Generate toolpaths for every feature of the part, adjusting feeds and speeds for wood rather than the original material.
3. Simulate the full toolpath and resolve any collisions or gouges before posting.

**Requirements**

- Toolpaths generated and simulated cleanly for the final, improved design
- Feeds and speeds specifically appropriate for wood, not copied from a metal-cutting setup
- Posted G-code ready for the router

---

## Checkpoint 2 — Fabrication & Material Comparison (Days 3–4)

**✏️ Cut the Part and Analyze the Material Difference**

1. CNC-route the final part in wood.
2. Fit-check the wood part the same way you validated the F2 part — against the real assembly, bolts, and mating components.
3. Update the material properties in your stress study to reflect wood instead of the original metal, and re-run the analysis.
4. Write a short note comparing the wood stress result to your original metal-based analysis: where does wood perform worse, and does that matter for this part's real use case?

**Requirements**

- Successfully CNC-routed wood part
- Fit-check performed against the real assembly
- Stress study re-run with wood material properties
- Written comparison explaining how and why the results differ from the original metal analysis

---

## Checkpoint 3 — Reflection

**✏️ Answer:**

1. What had to change in your CAM setup to cut this part in wood instead of the original material?
2. How did the stress results differ once you switched to wood's material properties, and did that surprise you?
3. Did the wood part still fit the real assembly the way your 3D-printed version did? What was different?
4. Looking back at the entire measure → model → validate → fabricate journey across Unit F, what's the single biggest thing you now understand that you didn't at the start?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Fusion 360 Project File (CAM Setup for Wood)**

Filename: `LastName_F3_Part_Wood_CAM.f3d`

**Posted G-Code**

Filename: `LastName_F3_Part_Wood.nc`

**Photos of Fabricated Wood Part & Fit Check**

Filename: `LastName_F3_WoodFitCheck.pdf`

**Material Comparison Write-Up (with Stress Study Screenshots)**

Filename: `LastName_F3_MaterialComparison.pdf`

**Reflection Document**

Filename: `LastName_F3_Reflection.pdf`

---

## 📊 Assessment Criteria

**CAM Setup for Wood (25%)**

- Correct, wood-appropriate feeds/speeds and clean simulation

**Fabrication & Fit (25%)**

- Successfully fabricated part with a genuine fit check against the real assembly

**Material Analysis (25%)**

- Stress study correctly updated for wood and clearly compared to the original metal analysis

**Reflection (25%)**

- Clear, specific account of how material substitution changed both the CAM process and the results
- Honest synthesis of the full Unit F journey

---

## 💡 Key Lesson

Swapping materials isn't just a different toolpath — it changes how the part performs, and knowing exactly what that trade-off costs is what separates a finished design from a merely fabricated one.
