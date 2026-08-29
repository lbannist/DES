# 3D Animation 11 – Rigid Body & Soft Body Simulation

## Unit 4: Physics Simulation & Intro to Unreal Engine — Challenge F1

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*


---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Set up Rigid Body simulations for objects that fall, collide, or knock into each other
- Set up a basic Soft Body simulation for squishy/deformable objects
- Bake a simulation so it plays back reliably
- Build simple naming and saving habits now that will make exporting select objects to Unreal easier later this unit

---

## 💭 Production Question

### What's the difference between animating something falling, and letting it actually fall?

---

## Checkpoint 1 — Rigid Body Basics (Day 1)

**✏️ Set Up a Falling/Colliding Scene**

1. Add a ground plane and set it as a Rigid Body of type "Passive" (Physics Properties → Rigid Body → Type: Passive) — this means it won't move but other objects will collide with it.
2. Add 3–5 objects above the ground (cubes, spheres, or simple shapes) and set each as a Rigid Body of type "Active."
3. Play the animation (spacebar) and watch the objects fall and collide with the ground and each other.
4. Adjust each Rigid Body's Mass, Friction, and Bounciness values and re-play to see how the simulation changes.
5. Once you're happy with the result, bake the simulation (Physics Properties → Rigid Body Cache → Bake) so it plays back the same way every time.
6. Rename your objects clearly in the Outliner (e.g., `RigidBody_Cube_01`, `RigidBody_Ground`) — a couple of these objects may end up exported to Unreal later in this unit, and clear names now save confusion then.

**Requirements**

- At least one Passive rigid body (ground/surface) and 3+ Active rigid bodies
- Mass, Friction, and/or Bounciness adjusted intentionally, not left at default for every object
- Simulation baked successfully
- Objects clearly named in the Outliner

---

## Checkpoint 2 — Soft Body Basics (Days 1–2)

**✏️ Set Up a Squishy Object**

1. Add a simple mesh with enough subdivided geometry to deform smoothly (a subdivided cube or sphere works well) and set it as a Soft Body (Physics Properties → Soft Body).
2. Add a ground plane below it (can reuse your Rigid Body ground from Checkpoint 1, but note Soft Body needs its own Collision setting on the ground object, not a Rigid Body setting).
3. Adjust the Soft Body's Goal and Edges settings (Stiffness, Damping) and play the simulation to see how the object squishes and settles when it lands.
4. Try at least two different Stiffness values and compare how "squishy" versus "firm" the object feels in each.
5. Bake the simulation once you're satisfied with the result.
6. Save your file using a version-numbered name (e.g., `LastName_F1_PhysicsSim_v01.blend`) rather than overwriting the same unnamed save repeatedly — small habit, but one worth having in place before this unit starts moving files into Unreal.

**Requirements**

- Soft Body object correctly deforms and settles on a collision surface
- At least two different Stiffness values tested and compared
- Simulation baked successfully
- File saved with a clear, version-numbered filename

---

## Checkpoint 3 — Reflection

**✏️ Answer:**

1. What happened when you changed Mass and Bounciness on your rigid body objects?
2. What's the difference in how Rigid Body and Soft Body objects are set up (Passive/Active vs. Goal/Stiffness)?
3. Why is baking a simulation important before final rendering?
4. Where could you see rigid body or soft body simulation being useful in a future animation or environment project?
5. Which object from today, if any, do you think would be worth exporting to Unreal later this unit — and is it named clearly enough for that to be easy?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI2020_F1_PhysicsSim.blend`

**Rigid Body Simulation Render**

Filename: `LastName_ANI2020_F1_RigidBody.mp4`

**Soft Body Simulation Render**

Filename: `LastName_ANI2020_F1_SoftBody.mp4`

**Reflection Document**

Filename: `LastName_ANI2020_F1_Reflection.pdf`

---

## 📊 Assessment Criteria

**Rigid Body Setup (30%)**

- Correct Passive/Active rigid body setup
- Mass, Friction, and/or Bounciness adjusted with clear intent
- Objects interact believably with the ground and each other
- Simulation successfully baked

**Soft Body Setup (30%)**

- Soft Body object deforms and settles believably
- Stiffness/Damping tested at more than one value
- Collision with the ground surface works correctly
- Simulation successfully baked

**Technical Execution (20%)**

- Both simulations play back reliably after baking
- No obvious glitches (objects flying off-scene, clipping through the ground)
- Appropriate mesh density used for the soft body to deform smoothly

**Reflection (20%)**

- Thoughtful, specific reflection on the process
- Clear, accurate comparison between rigid body and soft body setup
- Honest account of what changing specific values did
- Concrete idea for a future use of physics simulation

---

## 💡 Key Lesson

Physics simulation lets you stop hand-animating things that should behave according to real-world rules — this saves enormous time on effects work, and understanding it now means you'll recognize exactly when a simulation is the right tool instead of manual keyframing.
