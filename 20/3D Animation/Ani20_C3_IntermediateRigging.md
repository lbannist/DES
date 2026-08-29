# 3D Animation 11 – Intermediate Rigging with Rigify

## Unit 1: Character Refinement, Storyboarding & Animation Principles — Challenge C3

**Time:** 1.5 Weeks (4 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenges C1–C2 and Gr10's rigging basics.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Enable and use Blender's Rigify add-on to generate a control rig
- Fit a Rigify metarig to a custom character's proportions
- Understand the difference between deform bones and control bones
- Test and use Rigify's built-in IK/FK switching

---

## 💭 Production Question

### What would a rig need to have in order for an animator to trust it completely?

---

## Checkpoint 1 — Enabling Rigify & Metarig Setup (Day 1)

**📖 Rigify Setup**

1. Go to Edit → Preferences → Add-ons, search for "Rigify," and enable it if it isn't already on.
2. Add a Rigify Human (Meta-Rig) via Shift + A → Armature → Human (Meta-Rig).
3. Compare the metarig's proportions to your Challenge C1 character in Edit Mode — note where the metarig's bones don't match your character's proportions.

**Questions to answer:**

1. What is a metarig, and how is it different from the final generated rig?
2. What Rigify bone groups do you notice already built into the metarig (arms, legs, spine, face)?

---

## Checkpoint 2 — Fitting the Metarig (Days 1–2)

**✏️ Adjust the Metarig to Your Character**

1. Enter Edit Mode on the metarig and select individual bones one at a time.
2. Move, scale, and rotate each bone so it sits correctly inside your character's mesh — start with the spine, then work outward to arms and legs.
3. Adjust bone roll (Ctrl+R while a bone is selected, or use the N-panel's bone roll value) if a limb bends in the wrong direction once posed later.
4. Check your character from the front and side view repeatedly while fitting bones — a bone that looks fine from the front can be badly placed from the side.
5. Pay close attention to fitting the hand and finger bones (if your character has visible fingers) and the foot bones, since these are the most commonly misaligned.

**Requirements**

- Metarig bones repositioned to accurately match the character's proportions
- Checked and adjusted from multiple viewing angles, not just one

---

## Checkpoint 3 — Generating & Testing the Rig (Days 2–3)

**✏️ Generate Your Control Rig**

1. With the metarig selected, go to the Armature Properties tab (or the Rigify panel) and click "Generate Rig."
2. Select the newly generated rig and enter Pose Mode.
3. Identify the difference between the deform bones (which actually move the mesh) and the control bones (which you as the animator select and move) — try clicking a few different control shapes and see what they do.
4. Parent your character mesh to the generated rig with Automatic Weights (select mesh, then rig, Ctrl+P → Automatic Weights) if it isn't already connected.
5. Test-pose a few limbs and confirm the mesh deforms correctly — if deformation is poor in a spot, you may need to revisit weight painting as in Gr10 Challenge A3.

**Requirements**

- Rig successfully generated from the fitted metarig
- Mesh correctly parented and responding to the new rig's controls
- Basic test poses show acceptable deformation

---

## Checkpoint 4 — IK/FK Switch Practice (Day 3)

**✏️ Test IK and FK**

1. Select an arm or leg control bone (usually a hand or foot control for IK) and check its custom properties in the N-panel for an "IK/FK" slider.
2. Pose the limb using IK (the hand/foot control drags the whole limb, good for keeping a foot planted on the ground).
3. Switch the slider to FK and notice how you now have to rotate each individual bone in the chain (upper arm, forearm, hand) separately.
4. Try a pose where IK makes more sense (a hand resting on a table) and a pose where FK makes more sense (a big free-swinging arm gesture), and note the difference in how each feels to pose.

**Requirements**

- Both IK and FK tested on at least one limb
- A clear example given (in reflection) of when each would be the better choice

---

## Checkpoint 5 — Reflection (Day 4)

**✏️ Answer:**

1. What was the hardest part of fitting the metarig to your character's proportions?
2. What's the practical difference between a deform bone and a control bone?
3. Give one example of a pose where IK is better, and one where FK is better.
4. How did generating a rig with Rigify compare to hand-building an armature in Grade 10?
5. What would you do differently next time you fit a metarig to a new character?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI2020_C3_RigifyRig.blend`

**Test Pose Screenshots (IK example, FK example)**

Filename: `LastName_ANI2020_C3_IKPose.png`, `LastName_ANI2020_C3_FKPose.png`

**Reflection Document**

Filename: `LastName_ANI2020_C3_Reflection.pdf`

---

## 📊 Assessment Criteria

**Metarig Fitting (25%)**

- Metarig bones accurately match the character's proportions
- Fitting checked and corrected from multiple viewing angles
- Bone roll/orientation corrected where needed
- Hands and feet fitted with particular care

**Rig Generation & Deformation (30%)**

- Rig successfully generated without errors
- Mesh correctly parented to the generated rig
- Test poses show clean deformation with no major stretching/collapsing
- Any deformation issues found were addressed, not ignored

**IK/FK Understanding (25%)**

- Both IK and FK tested and clearly demonstrated
- Correct, specific example given of when to use each
- Screenshots clearly show the difference between the two modes
- Reflection shows accurate understanding of the underlying concept

**Reflection (20%)**

- Thoughtful, specific reflection on the process
- Clear, accurate explanation of deform vs. control bones
- Honest comparison to the Grade 10 hand-built rigging process
- Concrete idea for improving the metarig-fitting process next time

---

## 💡 Key Lesson

Rigify doesn't remove the need to understand rigging — it removes the repetitive bone-building work so you can focus on fitting, testing, and trusting a rig. This same fitting-and-testing process scales up directly into the more advanced control rigs used in Grade 12.
