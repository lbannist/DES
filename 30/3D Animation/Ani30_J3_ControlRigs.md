# 3D Animation 12 – In-Engine Tweaking & The Final Render

## Unit 4: Real-Time Sequencing & Technical Animation — Challenge J3

**Time:** 1 Week (3–4 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenges J1–J2.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Use Unreal's Control Rig to make direct pose adjustments to an imported animation, inside the engine
- Build a trigger-based system that plays a specific cinematic animation sequence
- Configure and run the Movie Render Queue for a final, portfolio-ready video export

---

## 💭 Production Question

### If you can't go back and fix something in Blender, how do you fix it without leaving the engine at all?

---

## Checkpoint 1 — Control Rig Setup (Day 1)

**✏️ Adjust a Pose Directly in Unreal**

1. Open a Level Sequence containing one of your character's animations (from Challenge J1 or J2) and add a Control Rig track for your character.
2. In the Sequencer timeline, find a specific frame where a pose could be improved — a hand that clips through the body, an arm that could read more clearly, a foot that isn't quite planted.
3. Use the Control Rig's controls (the same kind of rig controls you built in Challenge G1) to adjust that specific pose directly on the timeline, without needing to reopen Blender.
4. Add a key at that frame so your adjustment holds, and check the animation plays correctly before and after your fix.

**Requirements**

- A Control Rig track successfully added to a Sequencer animation
- At least one genuine pose problem identified and corrected directly in Unreal
- Animation plays correctly through the adjusted frame with no popping

---

## Checkpoint 2 — Trigger-Based Cinematic (Days 1–3)

**✏️ Build an Approach-Triggered Cinematic**

1. Place an object or marker in your level that represents something worth a cinematic moment (a door, an artifact, a landmark).
2. Add a Trigger Box near it and, using your Unit 2 Blueprint skills, set up an "On Actor Begin Overlap" event tied to the player character approaching.
3. Connect that event to play a specific Level Sequence — this could be your Challenge J1 camera work, a new short camera move, or a moment where your character performs a specific animation (a reaction, a gesture).
4. Consider whether player control should pause during the cinematic (a common technique in games) — if your class covers this, try disabling player input for the sequence's duration and re-enabling it afterward.
5. Test the full interaction: approach the trigger as a player, confirm the cinematic plays correctly, and confirm normal play resumes afterward.

**Requirements**

- A trigger correctly set up to play a specific Level Sequence on player approach
- The triggered cinematic plays cleanly from start to finish
- Player control behavior (paused or not) is a deliberate choice, not an accident

---

## Checkpoint 3 — Movie Render Queue Export (Days 3–4)

**✏️ Render Your Final Portfolio Video**

1. Open the Movie Render Queue (Window → Cinematics → Movie Render Queue) and add your best Level Sequence (Challenge J1's camera work, or your new J3 cinematic) to the render job.
2. Configure output settings: resolution (1920×1080 minimum), output format, and any anti-aliasing/quality settings appropriate for a final portfolio-quality render.
3. Render the final video and review it fully once complete, checking for any missing textures, popping, or technical errors that weren't visible in the viewport preview.
4. If anything looks wrong in the final render that didn't in the editor, diagnose and re-render rather than submitting a flawed final file.

**Requirements**

- Final video rendered through Movie Render Queue, not a viewport capture
- Output resolution and quality settings appropriate for a portfolio-ready piece
- Final render reviewed fully and free of technical errors

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. What pose problem did you fix with Control Rig, and why was it worth fixing directly in Unreal instead of going back to Blender?
2. What was the trickiest part of getting the trigger-based cinematic to play and then hand control back to the player cleanly?
3. What did reviewing your final Movie Render Queue output reveal that you hadn't noticed in the viewport?
4. Looking back at Challenges J1–J3, what's the single most valuable technical skill you built in this unit?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Unreal Project Folder (zipped)**

Filename: `LastName_ANI3030_J3_UnrealProject.zip`

**Control Rig Before/After Comparison**

Filename: `LastName_ANI3030_J3_ControlRig_Before.png`, `_After.png`

**Trigger-Cinematic Demo Video**

Filename: `LastName_ANI3030_J3_TriggerCinematic.mp4`

**Final Movie Render Queue Export**

Filename: `LastName_ANI3030_J3_FinalRender.mp4`

**Reflection Document**

Filename: `LastName_ANI3030_J3_Reflection.pdf`

---

## 📊 Assessment Criteria

**Control Rig Adjustment (20%)**

- Control Rig track correctly added and functional
- A genuine, specific pose problem identified and corrected
- Adjustment holds cleanly with no popping around the fixed frame

**Trigger-Based Cinematic (35%)**

- Trigger correctly plays a specific Level Sequence on player approach
- Cinematic plays cleanly from start to finish
- Player control behavior during the cinematic is a deliberate, working choice
- Interaction tested and confirmed reliable

**Final Render Quality (30%)**

- Rendered through Movie Render Queue at appropriate resolution/quality
- Final output reviewed and free of technical errors
- Render represents portfolio-ready quality, not a rough draft

**Reflection (15%)**

- Thoughtful, specific reflection on the process
- Clear reasoning for the Control Rig fix chosen
- Honest account of the trickiest trigger/cinematic logic
- Genuine identification of the unit's most valuable skill

---

## 💡 Key Lesson

This is a complete interactive/cinematic pipeline cycle, start to finish: an asset built and rigged in Blender, brought into a real-time engine, made responsive to player input, polished without ever leaving the engine, and rendered to a final, presentation-ready file. That full loop — not any single tool inside it — is the actual skill this unit was built to teach.
