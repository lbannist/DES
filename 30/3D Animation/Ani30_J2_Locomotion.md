# 3D Animation 12 – Motion Blending & Locomotion

## Unit 4: Real-Time Sequencing & Technical Animation — Challenge J2

**Time:** 1 Week (3–4 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenge J1 and reconnects to your Unit 2 Blueprint interactivity work.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Import multiple locomotion animations (idle, walk, run) sharing one skeleton
- Build a Blend Space that smoothly combines those animations based on speed
- Build an Animation Blueprint using a visual State Machine
- Connect that Animation Blueprint to player input controls, without writing code

---

## 💭 Production Question

### What's the difference between three separate animation loops and one character that actually feels alive under player control?

---

## Checkpoint 1 — Preparing & Importing Animation Clips (Day 1)

**✏️ Get Your Animations Into Unreal**

1. In Blender, prepare at least three locomotion animations on your Challenge J1 character's rig: an idle, a walk cycle, and a run cycle (reuse and refine your Grade 10/11 cycles if helpful).
2. Export each as a separate FBX, or as one FBX containing multiple actions if your workflow supports it — check with your teacher which approach your class uses.
3. Import the animation(s) into Unreal, making sure each is correctly assigned to your Challenge J1 character's Skeleton asset (Unreal will warn you if a skeleton mismatch occurs).
4. Preview each animation individually in the Unreal Animation Editor to confirm it plays back correctly on the imported skeleton.

**Requirements**

- At least three distinct locomotion animations (idle, walk, run) imported
- All animations correctly assigned to the same Skeleton asset
- Each animation previewed and confirmed working individually

---

## Checkpoint 2 — Building a Blend Space (Days 1–2)

**✏️ Combine Animations by Speed**

1. Create a new Blend Space (1D) asset in the Content Browser, using your character's Skeleton.
2. Set up the horizontal axis to represent Speed (e.g., 0 to 375, a common Unreal default range, or values appropriate to your character).
3. Place your Idle animation at Speed 0, your Walk animation at a mid-range speed value, and your Run animation at the top of the range.
4. Use the Blend Space's preview window to drag the speed value across the range and check that the blending between animations looks smooth, not like a jarring pop between poses.
5. If the blend looks wrong at any point (e.g., feet sliding, an awkward mid-blend pose), adjust the speed values where each animation sits until it feels natural.

**Requirements**

- A functional 1D Blend Space combining idle, walk, and run
- Smooth blending confirmed across the speed range in the preview window
- Any foot-sliding or awkward blending identified and adjusted

---

## Checkpoint 3 — Animation Blueprint & State Machine (Days 2–3)

**✏️ Build the Logic Layer**

1. Create a new Animation Blueprint (AnimBP) targeting your character's Skeleton.
2. In the AnimGraph, add a State Machine and build states for at least Idle/Locomotion (your Blend Space can live inside a single "Locomotion" state, or you can build separate states — check which approach your teacher prefers).
3. Add a float variable (e.g., `Speed`) to the AnimBP and connect it to drive your Blend Space's Speed input.
4. Set up transition rules between states if you're using separate states (e.g., transition to a "Jump" state if a Jump condition is true) — even a simple two-state setup demonstrates the concept.

**Requirements**

- A functional Animation Blueprint with a State Machine
- A Speed variable correctly driving the Blend Space
- At least one clear state transition set up and logically correct

---

## Checkpoint 4 — Connecting to Player Input (Days 3–4)

**✏️ Make It Responsive**

1. Assign your new Animation Blueprint to your character's Skeletal Mesh component (in the character's Blueprint, under the Mesh component's Animation settings).
2. Connect your character's actual movement speed (from the Character Movement Component, or from your Unit 2 Blueprint input controls) to the `Speed` variable in your AnimBP — this is the step that makes the blend respond to real player input instead of just a preview slider.
3. Play the level and move your character using keyboard/controller input, watching for a smooth transition from idle to walk to run as speed increases and decreases.
4. If the transition feels laggy or too abrupt, revisit your Blend Space's speed placement or add basic interpolation to smooth the Speed variable itself.

**Requirements**

- AnimBP correctly assigned to the character
- Character's actual movement speed correctly driving the Blend Space in real time
- Smooth, responsive transitions confirmed by actually moving the character during play

---

## Checkpoint 5 — Reflection

**✏️ Answer:**

1. What did adjusting the Blend Space's speed values teach you about how blending actually works?
2. What was the hardest part of building the State Machine logic?
3. How did seeing your character respond to real player input change how you think about the animation cycles you built back in Grade 10 and 11?
4. What's one more state or blend (a strafe, a crouch, a turn-in-place) you'd want to add if you had more time?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Exported Animation FBX Files**

Filename: `LastName_ANI3030_J2_Animations.fbx` (or one file per animation if exported separately)

**Unreal Project Folder (zipped)**

Filename: `LastName_ANI3030_J2_UnrealProject.zip`

**Gameplay Capture (character moving through idle/walk/run under player control)**

Filename: `LastName_ANI3030_J2_LocomotionDemo.mp4`

**Reflection Document**

Filename: `LastName_ANI3030_J2_Reflection.pdf`

---

## 📊 Assessment Criteria

**Animation Import & Skeleton Setup (20%)**

- At least three distinct locomotion animations correctly imported
- All animations correctly matched to the character's Skeleton
- Each animation confirmed working individually before combining

**Blend Space Construction (25%)**

- Functional 1D Blend Space with correctly placed animations
- Smooth blending across the full speed range
- Foot-sliding or awkward blend points identified and corrected

**Animation Blueprint & State Machine (25%)**

- Functional AnimBP with a working State Machine
- Speed variable correctly driving the Blend Space
- At least one logically correct state transition

**Player-Responsive Locomotion (20%)**

- AnimBP correctly assigned and functioning on the character
- Real movement speed correctly drives the Blend Space during actual play
- Transitions feel smooth and responsive, not laggy or jarring

**Reflection (10%)**

- Thoughtful, specific reflection on the process
- Clear explanation of what blend space tuning revealed
- Honest account of the State Machine's hardest logic to build
- Specific idea for an additional state/blend to add later

---

## 💡 Key Lesson

This is the moment isolated animation loops stop being isolated — a walk cycle and a run cycle you built for their own sake are now driven by an actual player's input, in real time. This no-code, visual logic (Blend Spaces, State Machines) is exactly how professional game animators make characters feel responsive without needing to be programmers.
