# 3D Animation 12 – Advanced Rigging: Control Rigs & Corrective Shape Keys

## Unit 1: Advanced Character Animation — Challenge G1

**Time:** 1.5 Weeks (4 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Gr11's Rigify rigging (Challenge C3). *

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Build or refine custom control shapes for easier animator interaction
- Organize rig controls logically using rig layers
- Practice seamless mid-animation IK/FK switching
- Use corrective shape keys to fix problem deformation at extreme poses

---

## 💭 Production Question

### What separates a rig an animator merely tolerates from one they actually trust?

---

## Checkpoint 1 — Custom Control Shapes (Day 1)

**📖 Control Shape Study**

1. Open your Gr11 Rigify rig and look at its default control shapes (circles, squares, custom widgets).
2. Research or recall why animators prefer distinct, recognizable control shapes for different bone types (e.g., a different shape for IK hand controls vs. FK arm controls).
3. Create a simple custom mesh shape (a small arrow, a diamond, a ring) in a separate collection to use as a new control widget.
4. Assign your custom shape to a bone's Custom Shape setting (Bone Properties → Viewport Display → Custom Shape) and observe the change in the viewport.

**Questions to answer:**

1. Why does a distinct control shape matter beyond just aesthetics?
2. Which bone did you choose to reshape, and why did you pick that particular shape?

---

## Checkpoint 2 — Organizing Rig Layers (Day 1–2)

**✏️ Clean Up Your Control Layout**

1. Open the Armature Properties → Viewport Display → Bone/Armature Layers (or Rigify's Layer panel, depending on your Blender version).
2. Group your controls logically — face controls on one layer, body controls on another, IK/FK switches on their own layer if helpful.
3. Hide layers you don't need visible all the time (e.g., deform bones) so the animator's view stays uncluttered.
4. Test switching between layers and confirm you can still access every control you need for animating.

**Requirements**

- Rig controls organized into at least two logical layers/groups
- Deform bones hidden from the default animating view
- All necessary controls remain accessible

---

## Checkpoint 3 — IK/FK Switching Mid-Animation (Day 2–3)

**✏️ Practice a Seamless Switch**

1. Pose an arm using FK for the first half of a short animation (e.g., a big free gesture).
2. At a chosen frame, snap the IK controls to match the FK bone's current position/rotation (many rigs, including Rigify, include a snapping operator for this — check your rig's IK/FK panel).
3. Switch the IK/FK influence slider at that frame and continue the animation in IK (e.g., the hand now needs to stay planted on a surface).
4. Play back the full animation and check that there's no visible pop or jump at the switch point.

**Requirements**

- At least one clean IK-to-FK or FK-to-IK switch performed mid-animation
- No visible pop/jump at the switch point
- A clear, sensible reason given for why the switch was needed at that point in the animation

---

## Checkpoint 4 — Corrective Shape Keys (Day 3–4)

**✏️ Fix an Extreme Pose**

1. Pose your character into an extreme position where deformation looks poor even after weight painting (a sharply bent elbow, a twisted torso, a wide facial expression).
2. With the mesh selected, add a new Shape Key (Object Data Properties → Shape Keys → +) based on the current (broken-looking) shape.
3. In Edit Mode on that shape key, sculpt/adjust the problem area back to a believable shape while the pose is held.
4. Set up a Driver on the shape key's Value, linked to the relevant bone's rotation, so the correction activates automatically as the character moves into that pose (check with your teacher on the specific driver setup your rig supports).
5. Test the correction by posing the character into and out of the extreme pose and confirming the fix activates and deactivates appropriately.

**Requirements**

- At least one corrective shape key created for a genuine deformation problem
- Shape key linked to the relevant bone via a driver (or otherwise activated automatically)
- Correction verified to activate/deactivate correctly across the pose range

---

## Checkpoint 5 — Reflection

**✏️ Answer:**

1. How did organizing your rig into layers change how it felt to animate with?
2. What made your IK/FK switch attempt successful (or where did it go wrong on your first try)?
3. What specific deformation problem did your corrective shape key solve?
4. How does this advanced rigging work change your confidence going into Challenge G4's final performance shot?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI3030_G1_AdvancedRig.blend`

**IK/FK Switch Test Render**

Filename: `LastName_ANI3030_G1_IKFKSwitch.mp4`

**Corrective Shape Key Before/After Renders**

Filename: `LastName_ANI3030_G1_Corrective_Before.png`, `_After.png`

**Reflection Document**

Filename: `LastName_ANI3030_G1_Reflection.pdf`

---

## 📊 Assessment Criteria

**Control Shape & Layer Organization (20%)**

- At least one custom control shape created and applied
- Rig controls organized into logical, clearly separated layers
- Deform bones hidden from the animating view
- Rig remains fully usable after reorganization

**IK/FK Switching (25%)**

- At least one clean mid-animation switch performed
- No visible pop or jump at the switch point
- Switch timing makes sense within the animation's context
- Clear explanation given for why the switch was necessary

**Corrective Shape Keys (35%)**

- At least one genuine deformation problem identified and corrected
- Correction is driven automatically by the relevant bone, not manually toggled
- Fix activates and deactivates appropriately across the full pose range
- Before/after comparison clearly shows the improvement

**Reflection (20%)**

- Thoughtful, specific reflection on the process
- Honest account of what worked or didn't on the first IK/FK switch attempt
- Clear description of the specific deformation problem solved
- Concrete connection drawn to the upcoming Challenge G4 capstone

---

## 💡 Key Lesson

A rig that's organized, switchable, and self-correcting at extremes is the difference between fighting your tools and actually performing with them. These are exactly the kind of details judges notice in a finished competition piece, even when they can't articulate why a shot "feels" more polished.
