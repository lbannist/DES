# Architectural Design 12 – Export, Print Prep & 3D Printing the Final Home

## Unit I: Physical & Digital Prototyping — Challenge I1

**Time:** 1.5–2 Weeks (5–6 Class Periods, Including Print Time)
**Due Date:** *[insert due date]*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Simplify architectural geometry appropriately for 3D printing at small scale
- Export a Revit massing model directly to a print-ready mesh format (STL or OBJ), accurately scaled to 1:100
- Slice a print-ready mesh using Elegoo Slicer or Orca Slicer with appropriate settings for a thin-walled model
- Diagnose and correct problems at both the modeling stage and the print stage, and produce a successfully printed 1:100 scale massing model

---

## 💭 Production Question

### Where does a print actually go wrong — in the model, or on the machine — and how do you tell the difference?

---

## Checkpoint 1 — Model Simplification & Scaling (Day 1)

**✏️ Decide What Survives the Print, Then Get the Math Right**

1. Starting from your custom home or capstone model, identify which elements need to survive into the printed massing (exterior walls, roof form, major massing moves) and which can be simplified away (interior partitions, fine trim details, small fixtures). Create a simplified version of the model.
2. Calculate what your building's real-world dimensions should measure at 1:100 scale (e.g., a 2.7 m wall should print at 27 mm), and confirm your Revit model's units and export settings will produce a correctly scaled mesh — check this against at least one known dimension.
3. Adjust minimum wall thicknesses if needed so nothing falls below a printable minimum (approximately 1–1.5 mm at your printer's typical nozzle/resolution).

**Requirements**

- A simplified model version with unnecessary detail removed
- A documented scale calculation for at least one reference dimension
- Wall thicknesses checked and adjusted for printability

---

## Checkpoint 2 — Export & Geometry Check (Day 2)

**✏️ Export It and Prove It's Clean**

1. Export the simplified, scaled model directly from Revit as an STL or OBJ file.
2. Open the exported file in Elegoo Slicer or Orca Slicer and visually check for problems: gaps, inverted faces, floating geometry, or overly thin walls.
3. Fix any problems found in Revit and re-export until the file is clean and ready to print.

**Requirements**

- A successfully exported STL or OBJ file
- Documented geometry check (screenshots or notes)
- Any problems found and corrected before moving on

---

## Checkpoint 3 — Slice, Print & Quality Check (Days 3–5)

**✏️ Set It Up to Succeed, Then Print It**

1. In Elegoo Slicer or Orca Slicer, verify the model's dimensions match your expected 1:100 scale, and orient the model on the print bed for the most stable print (flattest base down, minimal overhangs).
2. Set appropriate print settings for a thin-walled architectural model (layer height, infill, and supports where roof overhangs or cantilevers require them), and run the slicer's preview to check for broken or missing geometry before committing to a print.
3. Slice and print the massing model. Once printed, check wall thickness, roof overhangs, and fine details for print quality. If the print failed or has significant quality issues, diagnose the cause (settings, orientation, or geometry back in Checkpoint 1–2) and reprint.

**Requirements**

- Verified dimensions and stable print orientation
- Documented print settings chosen, with supports applied where needed
- A completed printed massing model, with a documented quality check and, if applicable, a diagnosed and corrected reprint

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. What did you have to simplify or remove from your model, and how did you decide what was safe to lose?
2. Did anything fail — either in the exported geometry or in the actual print? What caused it, and how did you fix it (or would you fix it next time)?
3. What surprised you about the difference between a Revit model and a model that actually prints cleanly?
4. Looking at the physical model next to your digital one, what feels different about seeing your design in your hands?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Simplified & Exported Files**

Filenames: `LastName_I1_Simplified.rvt`, `LastName_I1_Massing.stl` (or `.obj`)

**Sliced Print File**

Filename: `LastName_I1_SlicedFile` (native slicer project file)

**Photos of the Printed Model**

Filename: `LastName_I1_PrintedModel.pdf` (photo set, multiple angles)

**Print Prep & Quality Check Notes**

Filename: `LastName_I1_PrintNotes.pdf`

**Reflection Document**

Filename: `LastName_I1_Reflection.pdf`

---

## 📊 Assessment Criteria

**Model Simplification & Scaling (25%)**

- Appropriate elements retained vs. removed
- Correct scale calculation and printable wall thicknesses

**Export & Geometry Quality (20%)**

- Clean, successfully exported mesh file
- Geometry problems identified and corrected

**Print Settings & Overhang Management (20%)**

- Appropriate settings chosen and justified
- Supports correctly applied where needed

**Print Quality (15%)**

- Wall thickness and overhangs print cleanly
- Evidence of quality checking and, if needed, correction

**Reflection (20%)**

- Specific, thoughtful reflection on the full prep-to-print process

---

## 💡 Key Lesson

A digital model is a promise; a physical print is proof — and most print failures were actually decided back in the model, long before the machine ever turned on.
