# 3D Animation 12 – Playable Environment: From Scene to Level

## Unit 2: Advanced Unreal Engine — Challenge H4 (Unit Capstone)

**Time:** 1.5–2 Weeks (5–6 Class Periods)
**Due Date:** *[insert due date]*

*Builds directly on Challenge H3's interactions.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Add a playable character to a level (first-person or third-person)
- Chain multiple Blueprint interactions together into a real level flow, where later interactions depend on earlier ones
- Apply advanced lighting (Light Mixer, reflection captures) to a space designed to be walked through, not just viewed from a fixed camera
- Optionally bookend the experience with a short Sequencer intro/outro cinematic

This is the unit capstone — your Challenge H3 level and interactions become the foundation for an actual short, playable experience: a small first-person or third-person exploration level, in the style of a simple adventure game or FPS objective room.

---

## 💭 Production Question

### What turns a room full of triggers into something that feels like a level with a beginning, middle, and end?

---

## Checkpoint 1 — Playable Character & Level Flow Planning (Days 1–2)

**✏️ Get a Player Moving Through Your Space**

1. Add a playable character to your Challenge H3 level — use Unreal's First Person or Third Person template (available via Add Content, or included in a new template project you can migrate assets into) and place its Player Start in your level.
2. Play the level and confirm you can walk around your existing Challenge H1–H3 assets and interactions as a moving player, not just an editor camera.
3. Sketch a simple level flow on paper or in a document: where does the player start, what's the first thing they encounter, and what's the "objective" that ends the level (reach a marked location, open a final door, collect a specific object)?
4. Decide on a genre framing for your piece — a short FPS-style objective room, or a small adventure/exploration level — since this will guide your choice of interactions and mood in the checkpoints ahead.

**Requirements**

- A playable character correctly placed and controllable in the level
- A written level flow: start point, at least one obstacle/interaction along the way, and a clear objective/end point
- A chosen genre framing (FPS-style or adventure/exploration)

---

## Checkpoint 2 — Chaining Interactions Together (Days 2–4)

**✏️ Build a Real Level Flow, Not Isolated Triggers**

1. Revisit your Challenge H3 interactions and decide which ones belong in your final level flow.
2. Add at least one new interaction this level actually needs (a pickup item, a switch, a locked door) if your H3 work doesn't already cover it.
3. Set up a Blueprint variable (e.g., a Boolean like `HasKey`, or an Integer counter like `SwitchesActivated`) that tracks player progress — this is the key difference from H3's standalone triggers, since interactions can now depend on each other.
4. Connect at least one interaction so it only works once a condition is met (e.g., a door's "Open" logic checks `HasKey == true` before it will actually open; if false, play a "locked" sound or message instead).
5. Set up a final trigger or condition that represents "level complete" — a message, a light change, or a simple end-screen text — that only fires once the player has met all required conditions.
6. Playtest the full flow yourself from the very start, exactly as an actual player would, to confirm the dependency logic works correctly.

**Requirements**

- At least 3 interactions present and chained into one coherent level flow
- At least one interaction that depends on a variable/condition set by an earlier interaction
- A clear "level complete" state that only triggers once all conditions are met
- Full flow tested start to finish by the student themselves

---

## Checkpoint 3 — Advanced Lighting for a Playable Space (Days 4–5)

**✏️ Light the Space to Be Walked Through**

1. Open the Light Mixer panel (Window → Light Mixer) and organize/adjust your scene's full lighting setup.
2. Walk the actual player path from start to objective and check lighting from that perspective at each stage — a shot that looked good from one fixed camera angle in earlier assignments may look flat or overly dark when walked through.
3. Add Reflection Captures near any reflective surfaces along the player's path.
4. Use lighting deliberately to help guide the player (e.g., a brighter area drawing attention to the next objective) as well as to set mood.

**Requirements**

- Light Mixer used to organize and adjust the full scene's lighting
- Lighting checked and adjusted specifically from the player's walking perspective, not just a static camera view
- At least one example of lighting used to guide player attention toward an objective

---

## Checkpoint 4 — Post-Process & Optional Cinematic Bookend (Day 5)

**✏️ Final Look and Optional Cinematic**

1. Add a Post Process Volume and adjust Exposure and Color Grading for your level's final mood.
2. **Optional:** using your Challenge H2 Sequencer skills, build a short intro cinematic (a few seconds of camera movement establishing the space before player control begins) and/or a short outro cinematic that plays once the "level complete" state triggers.
3. Compare your level with and without post-process adjustments to confirm they add value.

**Requirements**

- Post Process Volume applied with deliberate exposure/color grading choices
- Optional: a Sequencer intro and/or outro cinematic attempted for bonus credit

---

## Checkpoint 5 — Playtest & Peer Critique (Day 5–6)

**✏️ Have Someone Else Actually Play It**

1. Have a peer play through your level from the very start, without guidance or hints from you.
2. Watch where they get confused, stuck, or miss an interaction entirely — don't intervene unless they're completely blocked.
3. Ask afterward: was the objective clear? Did the chained interactions (locked door, switches, etc.) make sense once they figured them out?
4. Note at least two specific pieces of feedback and make adjustments before final submission.

---

## Checkpoint 6 — Reflection (Day 6)

**✏️ Answer:**

1. What was the biggest difference between designing isolated interactions (Challenge H3) and designing a level where interactions depend on each other?
2. What did watching a peer actually play your level reveal that you couldn't see just by testing it yourself?
3. How did lighting for a walked path differ from lighting for a single fixed camera shot?
4. If you added one more room, interaction, or objective to this level, what would it be?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Unreal Project Folder (zipped)**

Filename: `LastName_ANI3030_H4_PlayableLevel.zip`

**Level Flow Sketch/Document**

Filename: `LastName_ANI3030_H4_LevelFlow.pdf`

**Playthrough Video (full start-to-finish playthrough, recorded)**

Filename: `LastName_ANI3030_H4_Playthrough.mp4`

**Critique Notes**

Filename: `LastName_ANI3030_H4_CritiqueNotes.pdf`

**Reflection Document**

Filename: `LastName_ANI3030_H4_Reflection.pdf`

---

## 📊 Assessment Criteria

**Playable Character & Level Flow (15%)**

- Player character correctly placed and controllable
- Clear, documented level flow with a start point and defined objective
- Genre framing (FPS-style or adventure/exploration) is clear in the final level

**Chained Interactions (35%)**

- At least 3 interactions present and working
- At least one interaction correctly depends on a variable/condition set earlier
- Clear "level complete" state that only fires once conditions are met
- Full flow works reliably start to finish

**Advanced Lighting (25%)**

- Light Mixer used effectively across the whole scene
- Lighting checked and adjusted from the player's walking perspective
- At least one example of lighting used to guide player attention

**Post-Process & Presentation (10%)**

- Deliberate, well-justified post-process adjustments
- Optional Sequencer bookend attempted for bonus credit where applicable

**Playtest Response (5%)**

- Peer playtest genuinely observed and documented
- At least two specific pieces of feedback addressed

**Reflection (10%)**

- Thoughtful, specific reflection on the whole unit
- Clear comparison between isolated and chained interaction design
- Honest account of what the peer playtest revealed

---

## 💡 Key Lesson

This is the difference between a demo and a level: a demo shows off a feature, a level makes the player earn their way through it. Chaining your Challenge H3 interactions into a real flow — with lighting that guides rather than just decorates — is the exact skill set the 3D Digital Game Art Skills Alberta category rewards, and it's a taste of real game-level design thinking.
