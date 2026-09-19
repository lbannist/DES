# CAD 11 – Parametric Design

## Unit E: Parametric Design — Challenge E2

**Time:** 1 Week (3–4 Class Periods)
**Due Date:** *[insert due date]*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Design a parametric model whose dimensions are derived from an external constraint, not chosen arbitrarily
- Write parameter relationships (formulas) rather than typing in values that simply happen to work
- Confirm a model regenerates correctly when the external constraint changes
- Understand the difference between parameterizing a shape and parameterizing a real design requirement

---

## 💭 Production Question

### What changes when your parameters have to answer to something outside the model?

---

## Checkpoint 1 — Deriving Dimensions from a Spec (Days 1–2)

**✏️ Set Up Parameters Driven by an External Component**

1. Review the supplied component spec sheet (dimensions of the electronics component your enclosure must house).
2. Set up user parameters for the enclosure's wall thickness, internal clearance, and lid tolerance, written as formulas derived from the component's dimensions — for example, wall thickness = component width + clearance × 2 — rather than typed-in numbers.
3. Model the enclosure body and lid using these derived parameters.

**Requirements**

- User parameters written as formulas referencing the component's dimensions, not standalone values
- Enclosure body and lid modeled using these derived parameters
- Internal clearance sufficient to actually fit the component (checked, not assumed)

---

## Checkpoint 2 — Testing with a New Spec (Day 3)

**✏️ Swap the Component and Confirm It Regenerates**

1. Swap in a different-sized component spec sheet (supplied).
2. Update only the parameters tied to the component's dimensions — do not touch any sketch geometry directly.
3. Regenerate the enclosure and confirm it resizes correctly to fit the new component, with wall thickness and clearance still correct.

**Requirements**

- Enclosure successfully regenerates for a second, different component spec
- No manual sketch edits made during the swap
- Wall thickness and clearance remain correctly derived for the new component

---

## Checkpoint 3 — Reflection

**✏️ Answer:**

1. What formula did you use to derive your wall thickness, and why that relationship specifically?
2. What broke (if anything) the first time you swapped in the new component spec, and how did you fix it?
3. How is this different from Challenge E1, where the parameters only had to satisfy the model itself?
4. Where else in real design might dimensions need to be derived from something outside your control?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Fusion 360 Project File**

Filename: `LastName_E2_Enclosure.f3d`

**Component Spec Sheets Used**

Filename: `LastName_E2_ComponentSpecs.pdf`

**Regeneration Screenshots (Both Components)**

Filename: `LastName_E2_Regeneration.png`

**Reflection Document**

Filename: `LastName_E2_Reflection.pdf`

---

## 📊 Assessment Criteria

**Parameter Derivation (35%)**

- Dimensions correctly written as formulas tied to the external component spec
- Sound reasoning behind the chosen relationships

**Regeneration & Testing (30%)**

- Enclosure regenerates correctly for a second component spec with no manual fixes

**Fit & Function (15%)**

- Internal clearance genuinely sufficient to house the component

**Reflection (20%)**

- Clear articulation of the derived relationships
- Honest account of what broke and how it was resolved

---

## 💡 Key Lesson

Parameters that only satisfy your own model are a start — parameters that correctly answer to something outside the model are what make a design actually usable in the real world.
