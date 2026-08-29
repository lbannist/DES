# 3D Animation 12 – Sequencer Cinematics

## Unit 2: Advanced Unreal Engine — Challenge H2

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenge H1.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Set up a Level Sequence using Unreal's Sequencer
- Keyframe camera cuts and camera movement
- Add audio to a sequence
- Render a final cinematic using the Movie Render Queue

---

## 💭 Production Question

### What turns a static Unreal scene into something that feels directed?

---

## Checkpoint 1 — Sequencer Setup (Day 1)

**📖 Sequencer Basics**

1. In your Challenge H1 project, create a new Level Sequence (right-click in Content Browser → Animation → Level Sequence).
2. Add a Cine Camera Actor to your scene and add it as a track in the Sequencer.
3. Practice setting keyframes on the camera's Transform track by moving the camera at different points on the timeline and pressing the keyframe button.
4. Play back your sequence and observe the resulting camera movement.

**Questions to answer:**

1. What's the difference between a regular camera and a Cine Camera Actor?
2. What did you notice about how Unreal interpolates between your camera keyframes?

---

## Checkpoint 2 — Camera Cuts & Cinematic Camera Settings (Days 1–2)

**✏️ Build a Multi-Shot Sequence**

1. Add a second Cine Camera Actor at a different angle/position in your scene.
2. Add both cameras to a Camera Cuts track in the Sequencer, and set up cuts between them at chosen points on the timeline.
3. Adjust each camera's Depth of Field and Focal Length settings (in the Camera's Details panel) to create a specific cinematic look — try a shallow depth of field on at least one shot to draw focus to a specific subject.
4. Optionally add subtle camera shake using a Camera Shake asset or a simple additive camera animation.

**Requirements**

- At least two cameras cutting between each other in one sequence
- Depth of field and/or focal length adjusted with clear intent on at least one shot
- Cuts are clean and well-timed, not jarring or accidental

---

## Checkpoint 3 — Audio & Final Render (Days 2–3)

**✏️ Add Sound and Render**

1. Add an audio track to your Sequencer (music, ambient sound, or a simple sound effect) and align it with the visual timing of your cuts.
2. Open the Movie Render Queue (Window → Cinematics → Movie Render Queue) and add your Level Sequence to the render queue.
3. Set your output resolution and format, then render your final cinematic.
4. Review the rendered output and confirm audio and video are synced correctly.

**Requirements**

- Audio track added and reasonably synced to the visual cuts
- Final cinematic rendered via Movie Render Queue, not just a viewport capture
- Output resolution and format appropriate for presentation

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. What did you learn about pacing from setting up cuts between two cameras?
2. How did adjusting depth of field or focal length change the feel of a shot?
3. What issues (if any) came up when rendering through the Movie Render Queue, and how did you resolve them?
4. How does this Sequencer work compare to camera work you did back in Blender (Gr10 Challenge B3, Gr11 environment units)?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Unreal Project Folder (zipped)**

Filename: `LastName_ANI3030_H2_SequencerProject.zip`

**Final Rendered Cinematic**

Filename: `LastName_ANI3030_H2_Cinematic.mp4`

**Reflection Document**

Filename: `LastName_ANI3030_H2_Reflection.pdf`

---

## 📊 Assessment Criteria

**Sequencer Setup (20%)**

- Level Sequence correctly created and functional
- Camera keyframes correctly set and interpolating as intended
- Understanding shown of basic Sequencer mechanics

**Camera Cuts & Cinematography (35%)**

- At least two cameras cutting between each other
- Depth of field/focal length used with clear cinematic intent
- Cuts are clean, well-timed, and support the scene's story or mood
- Camera choices show growth from earlier, simpler camera work

**Audio & Final Render (30%)**

- Audio added and reasonably synced to visual timing
- Final cinematic rendered through Movie Render Queue
- Output resolution/format appropriate and technically clean
- No major sync or render errors in the final output

**Reflection (15%)**

- Thoughtful, specific reflection on the process
- Clear explanation of pacing lessons learned
- Honest account of any Movie Render Queue troubleshooting
- Fair comparison drawn to earlier Blender camera work

---

## 💡 Key Lesson

Sequencer is Unreal's answer to editing and cinematography combined — the same shot-planning instincts built in storyboarding carry directly over here, just applied inside a real-time engine with its own render pipeline.
