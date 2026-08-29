# 3D Animation 12 – Basic Blueprints for Interactivity

## Unit 2: Advanced Unreal Engine — Challenge H3

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenges H1–H2.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Understand basic Blueprint visual scripting concepts (events, functions, variables)
- Build a simple interactive element (a trigger, a light toggle, a door)
- Build these interactions inside one continuing level — not disconnected test scenes — so they're ready to be chained into a real playable space in Challenge H4

---

## 💭 Production Question

### What's the smallest amount of interactivity that makes a scene feel like a real place instead of a static picture?

---

## Checkpoint 1 — Blueprint Basics (Day 1)

**📖 Visual Scripting Orientation**

1. Create a new Blueprint Actor (Content Browser → right-click → Blueprint Class → Actor).
2. Open the Blueprint Editor and explore the Event Graph, noting common starting nodes like Event BeginPlay and Event Tick.
3. Add a simple Print String node connected to Event BeginPlay, compile, and place the Blueprint in your level to confirm the message appears when you play.
4. Explore the difference between an Event (something that happens) and a Function (something you call) at a basic conceptual level.
5. Before building anything further, pick one continuing level (your Challenge H1 scene, or a new one) to do all of this unit's Blueprint work in — Challenge H4 will turn this same level into something a player can actually walk through and interact with, so it's worth choosing a space with a bit of size and layout to it now.

**Questions to answer:**

1. What's the difference between Event BeginPlay and Event Tick?
2. What did the Print String test confirm was working correctly?
3. What level are you building in, and does it have enough space/layout for a player to eventually move through it?

---

## Checkpoint 2 — Trigger Volume Interaction (Days 1–2)

**✏️ Build a Trigger-Based Interaction**

1. Add a Trigger Box or Trigger Sphere to your level and place it somewhere a camera or player character would pass through.
2. In a Blueprint, add an Event that fires "On Actor Begin Overlap" for that trigger volume.
3. Connect that event to a simple action — toggling a light's visibility, playing a sound, or triggering a small object movement (e.g., a door rotating open).
4. Test the interaction by simulating or playing in the editor and walking/moving through the trigger.

**Requirements**

- A trigger volume correctly set up with an overlap event
- Overlap event connected to a clear, working action
- Interaction successfully tested and functioning

---

## Checkpoint 3 — Light or Door Toggle (Days 2–3)

**✏️ Build a Second, Different Interaction**

1. Choose a second interaction type different from Checkpoint 2 (if you did a light toggle, try a door/object rotation this time, or vice versa).
2. Use a Timeline node if animating a smooth transition (e.g., a door opening gradually rather than snapping instantly) — add a Timeline, set keyframes for a rotation or location value, and connect it to your trigger event.
3. Test and refine the timing/easing of the interaction until it feels natural.

**Requirements**

- A second, distinct interaction type built
- Timeline (or equivalent smooth transition method) used if the interaction involves movement
- Interaction feels natural, not instant/jarring, unless that's the intended effect

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. What was the hardest part of understanding Blueprint's event-based logic at first?
2. How did using a Timeline change the feel of your second interaction compared to an instant on/off toggle?
3. In Challenge H4, these interactions may need to depend on each other (e.g., a door that only opens after a switch is triggered) — which of your two interactions do you think would be easiest to chain to another, and how might that work?
4. What's one more interaction type you'd like to try if you had more time?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Unreal Project Folder (zipped)**

Filename: `LastName_ANI3030_H3_BlueprintProject.zip`

**Interaction Demo Video (both interactions working)**

Filename: `LastName_ANI3030_H3_InteractionDemo.mp4`

**Reflection Document**

Filename: `LastName_ANI3030_H3_Reflection.pdf`

---

## 📊 Assessment Criteria

**Blueprint Fundamentals (20%)**

- Clear understanding shown of Events, Functions, and basic Blueprint structure
- Print String or equivalent test successfully used to verify logic
- Blueprint compiles and runs without errors

**Trigger-Based Interaction (35%)**

- Trigger volume correctly set up and functional
- Overlap event connected to a clear, working action
- Interaction tested and confirmed to work reliably

**Second Interaction & Timeline Use (30%)**

- A distinct second interaction type built
- Timeline (or equivalent) used for any smooth/animated transition
- Timing/easing feels natural and appropriate to the interaction

**Reflection (15%)**

- Thoughtful, specific reflection on the process
- Honest account of the hardest conceptual hurdle
- Clear explanation of the Timeline's effect on feel
- Concrete idea for the Challenge H4 showcase scene

---

## 💡 Key Lesson

You don't need to be a programmer to make a scene feel alive — a couple of well-placed triggers and simple visual scripting logic go a long way toward making a showcase environment feel like a real, inhabited place rather than a static render.
