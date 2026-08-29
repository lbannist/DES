# 3D Animation 11 – Cinematic Trailer

## Unit 4: Physics Simulation & Intro to Unreal Engine — Challenge F5 (Unit Capstone)

**Time:** 2 Weeks (6–7 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenge F4's lit Unreal scene.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Analyze how professional trailers use pacing, music, sound design, and title reveals to build atmosphere
- Set up basic camera movement in Unreal's Sequencer and render it out
- Apply title/text elements to a finished piece
- Add sound effects and music, syncing them to visual beats
- Turn a finished Unreal scene into a short, polished cinematic trailer

This is the true capstone of the entire unit — physics simulation, Unreal import/lighting, and now cinematic presentation all come together here.

---

## 💭 Production Question

### What makes a 20-second trailer make you want to see the whole thing?

---

## Checkpoint 1 — Trailer Reference Study (Day 1)

**📖 Analyze Real Trailers**

Your teacher will provide two reference trailers to study: the *Metroid Prime* GameCube trailer (2003) and the *MechWarrior 2* trailer (1995). Both are older examples chosen specifically because they show these techniques clearly, without excessive modern editing speed getting in the way.

1. Watch both trailers once all the way through without taking notes — just get a first impression.
2. Watch again, this time pausing to note: where does music start, build, and peak? Where do sound effects (not music) do the work instead?
3. Note exactly when and how the title/logo appears — is it sudden, does it build up, is there a tagline?
4. Count the approximate number of distinct shots/cuts in each trailer and note the average shot length — is it fast-cut or slow and atmospheric?
5. Identify one moment in each trailer that feels like the "hook" — the moment designed to make you want more.

**Questions to answer:**

1. How did music pacing relate to what was happening on screen in each trailer?
2. How and when did the title appear in each trailer?
3. What was each trailer's "hook" moment, and what made it work?
4. Which trailer's overall pacing (fast-cut vs. slow/atmospheric) is closer to what you want for your own piece, and why?

---

## Checkpoint 2 — Concept & Shot List Planning (Days 1–2)

**✏️ Plan Your Trailer**

1. Decide what your trailer is "for" — a fictional movie, TV show, or video game, using your Challenge F4 scene as its world.
2. Using your Checkpoint 1 analysis, sketch a rough structure: establishing shot(s) → building tension/atmosphere → a hook moment → title reveal → optional tagline or release-date-style final card.
3. Write a shot list (aim for 4–8 shots) noting roughly what each shot shows and how long it should last.
4. Decide where your title should land in this structure, based on what you observed in your references.

**Requirements**

- A clear concept (movie/show/game) established for the trailer
- A written shot list of 4–8 shots with rough durations
- A planned location for the title reveal within that structure

---

## Checkpoint 3 — Camera Sequence in Unreal (Days 2–4)

**✏️ Build and Render Your Camera Work**

1. In your Challenge F4 scene, create a new Level Sequence (right-click in Content Browser → Animation → Level Sequence).
2. Add a Cine Camera Actor and add it to the Sequencer as a track.
3. For each shot on your shot list, either move/keyframe this camera to a new position and add a cut, or add additional Cine Cameras for different angles and cut between them using a Camera Cuts track.
4. Match your shot durations roughly to your Checkpoint 2 plan, adjusting as needed once you see it in motion.
5. Render your sequence using the Movie Render Queue (Window → Cinematics → Movie Render Queue) at a resolution and format suitable for further editing (a high-quality video file).

**Requirements**

- All planned shots built and cutting together in the Sequencer
- Shot durations roughly match the Checkpoint 2 plan
- Sequence rendered out via Movie Render Queue as a usable video file

---

## Checkpoint 4 — Title Card & Text (Days 4–5)

**✏️ Add Your Title**

1. Import your rendered Unreal footage into a video editor (DaVinci Resolve, or Blender's Video Sequence Editor, per your class's setup).
2. Create a title card — your fictional movie/show/game's name, styled with a font and simple animation (fade in, scale up, or a simple reveal) appropriate to its genre.
3. Place the title at the point in your trailer you planned in Checkpoint 2, based on your reference analysis.
4. If time allows, add a simple tagline or "coming soon"-style final card at the end.
5. **Optional bonus:** instead of (or in addition to) a post-production title card, try building the title as a 3D Text Render Actor directly inside your Unreal scene, lit and integrated into the environment itself, the way some trailers reveal a logo as part of the world.

**Requirements**

- A styled title card created and placed at an intentional point in the trailer
- Title styling (font, animation) appropriate to the fictional project's genre/mood
- Optional: an in-engine 3D title attempted for bonus credit

---

## Checkpoint 5 — Sound Design: SFX & Music (Days 5–6)

**✏️ Add Sound and Music**

1. Source or create background music appropriate to your trailer's mood (royalty-free or teacher-approved sources only) and add it to your timeline.
2. Add at least two distinct sound effects (a whoosh on a camera move, an impact, an ambient environmental sound) at moments that support specific visual beats — this is different from just having music playing underneath everything.
3. Adjust audio levels so music, SFX, and any voice/dialogue (if used) don't compete with or drown each other out.
4. Watch your trailer back and check: does at least one visual beat (a cut, a reveal, the title appearing) line up with a music or sound beat?

**Requirements**

- Background music added and appropriately leveled
- At least two distinct sound effects placed at meaningful visual moments
- At least one clear instance of a visual beat synced to an audio beat

---

## Checkpoint 6 — Final Edit, Peer Critique & Export (Days 6–7)

**✏️ Finish and Test Your Trailer**

1. Do a full watch-through of your assembled trailer and tighten any pacing issues — cut anything that drags, adjust any transition that feels abrupt in the wrong way.
2. Share your trailer with a peer group. Ask specifically: does this make you want to see more? Where did you lose interest, if anywhere?
3. Note at least two specific pieces of feedback and make final adjustments based on them.
4. Export your final trailer at a resolution and length appropriate for presentation (check with your teacher for any specific requirements).

**Requirements**

- Full trailer watched through and pacing tightened
- Peer feedback documented and acted on
- Final export meets presentation requirements

---

## Checkpoint 7 — Reflection

**✏️ Answer:**

1. What specifically did you borrow from the Metroid Prime or MechWarrior 2 trailers, and how did you adapt it for your own piece?
2. Which was harder to get right: the camera work in Unreal, or the pacing/sound design in the edit?
3. What did your peer feedback reveal about where your trailer lost or held attention?
4. Looking back across this entire unit — physics simulation, Unreal import, lighting, and now this trailer — which skill do you feel most confident heading into Grade 12 with?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Unreal Project Folder (zipped)**

Filename: `LastName_ANI2020_F5_UnrealSequence.zip`

**Raw Rendered Unreal Footage**

Filename: `LastName_ANI2020_F5_RawFootage.mp4`

**Editing Project File**

Filename: `LastName_ANI2020_F5_EditProject.drp` (DaVinci Resolve) or `.blend` (VSE)

**Final Exported Trailer**

Filename: `LastName_ANI2020_F5_Trailer.mp4`

Export Requirements:

- 20–45 seconds
- Minimum 1920 × 1080 resolution
- Audio (music and SFX) included and properly synced

**Shot List & Reference Notes**

Filename: `LastName_ANI2020_F5_ShotList.pdf`

**Critique Notes**

Filename: `LastName_ANI2020_F5_CritiqueNotes.pdf`

**Reflection Document**

Filename: `LastName_ANI2020_F5_Reflection.pdf`

---

## 📊 Assessment Criteria

**Reference Analysis & Planning (15%)**

- Genuine, specific analysis of both reference trailers
- Clear shot list with a deliberate structure informed by that analysis
- Title placement planned intentionally, not as an afterthought

**Camera Work in Unreal (20%)**

- Shots successfully built and cutting together in Sequencer
- Shot durations reflect the planned structure
- Camera work shows growth from earlier, simpler Unreal camera use

**Title & Text (15%)**

- Title card styled appropriately to the fictional project's genre/mood
- Title placed at an intentional structural point
- Any in-engine 3D title attempt (bonus) integrated cleanly

**Sound Design (25%)**

- Music appropriately chosen and leveled
- At least two distinct, well-placed sound effects
- At least one clear sync between a visual beat and an audio beat
- Overall audio mix doesn't compete with itself

**Final Polish & Critique Response (10%)**

- Pacing tightened based on a full watch-through
- Peer feedback genuinely considered and applied
- Final export meets all technical requirements

**Reflection (15%)**

- Thoughtful, specific reflection on the whole process
- Clear, specific connection drawn to the reference trailers studied
- Honest comparison of which part of the process was hardest
- Genuine self-assessment of readiness heading into Grade 12

---

## 💡 Key Lesson

A trailer isn't just a shorter version of the finished thing — it's a completely different craft built on pacing, restraint, and the specific alchemy of picture and sound working together. This is your first real practice with that craft, and it's a direct preview of the reel-editing and cinematic work waiting in Grade 12.
