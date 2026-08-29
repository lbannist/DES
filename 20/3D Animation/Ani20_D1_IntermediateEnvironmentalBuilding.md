# 3D Animation 11 – Intermediate Environment Building

## Unit 2: Environment, Lighting & Rendering — Challenge D1

**Time:** 1.5 Weeks (4 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Gr10's low-poly landscape unit.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Use the Array and Boolean modifiers to build more complex environment geometry
- Practice basic kit-bashing — combining reused pieces into a more detailed scene
- Maintain consistent scale across a more ambitious environment than Grade 10

---

## 💭 Production Question

### How much more convincing can a space feel with just a bit more geometric complexity?

---

## Checkpoint 1 — Reference & Planning (Day 1)

**📖 Environment Study**

1. Find 2–3 reference images of environments more detailed than your Grade 10 low-poly landscape — look for architecture, ruins, or structured natural environments.
2. Identify repeating structural elements in your references (columns, fence posts, window patterns) — these are good candidates for the Array modifier.
3. Identify any complex shapes that look like they're built from combining simpler shapes (an archway, a cut-out window) — these are good candidates for Boolean operations.
4. Sketch a rough plan for your own environment, noting where you expect to use Array and where you expect to use Boolean.

**Questions to answer:**

1. What repeating elements did you find in your references, and where would Array modifiers help build them?
2. What complex shapes did you find that look like combined simpler shapes?

---

## Checkpoint 2 — Array Modifier Structures (Days 1–2)

**✏️ Build a Repeating Structure**

1. Model a single repeating unit (a fence post, a column, a window frame section).
2. Add an Array modifier (Modifier Properties → Add Modifier → Array) and adjust the Count and the Relative/Constant Offset values until the repeated units line up correctly with consistent spacing.
3. If your structure needs to curve or follow a path (e.g., a fence following a curved road), add a Curve modifier alongside the Array modifier and set it to follow a curve object.
4. Apply the Array modifier once you're happy with the result (Object → Apply → Array) if your workflow calls for it, or leave it non-destructive if you want to keep adjusting it later.

**Requirements**

- At least one structure built using the Array modifier
- Spacing/offset adjusted intentionally, not left at default
- Structure integrates believably into the planned environment layout

---

## Checkpoint 3 — Boolean Modifier Details (Days 2–3)

**✏️ Combine or Cut Shapes**

1. Model your base shape (a wall, a block) and a second "cutter" shape (a window opening, a doorway, a hole).
2. Add a Boolean modifier to the base shape, set it to Difference, and target the cutter shape to carve the opening.
3. Try a Boolean set to Union on a separate pair of shapes to combine two forms into one seamless object (e.g., merging a pipe into a wall).
4. Check the resulting geometry closely in Edit Mode for any messy leftover geometry (Boolean operations can sometimes create small artifacts) and clean up with Merge by Distance if needed (Mesh → Clean Up → Merge by Distance).

**Requirements**

- At least one Boolean Difference operation (cutting an opening)
- At least one Boolean Union operation (combining shapes), if time allows
- Resulting geometry checked and cleaned of Boolean artifacts

---

## Checkpoint 4 — Kit-Bashing & Scene Assembly (Day 4)

**✏️ Assemble the Full Environment**

1. Bring your Array-based structures and Boolean-based details together with any simpler modeled pieces into one scene.
2. Duplicate and reposition pieces as needed to fill out the environment, following your Checkpoint 1 layout sketch.
3. Check scale consistency throughout — compare doorway/window sizes to a rough human-scale reference object if helpful.
4. Take a full-scene screenshot from a clear, readable angle.

**Requirements**

- Array and Boolean elements combined into one cohesive scene
- Consistent scale maintained throughout
- Scene shows clear improvement in complexity over the Grade 10 low-poly landscape

---

## Checkpoint 5 — Reflection

**✏️ Answer:**

1. Where did the Array modifier save you the most time compared to modeling by hand?
2. What was the trickiest part of getting a Boolean operation to produce clean geometry?
3. How did you check and maintain scale consistency across this more complex scene?
4. Compare this environment to your Grade 10 low-poly landscape — what's genuinely more convincing about it, and why?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI2020_D1_Environment.blend`

**Full Scene Screenshot**

Filename: `LastName_ANI2020_D1_SceneOverview.png`

**Reflection Document**

Filename: `LastName_ANI2020_D1_Reflection.pdf`

---

## 📊 Assessment Criteria

**Array Modifier Use (25%)**

- At least one structure built with the Array modifier
- Spacing/offset values adjusted with clear intent
- Structure integrates cleanly into the overall scene
- Curve-following or other advanced Array use attempted where relevant

**Boolean Modifier Use (25%)**

- At least one clean Boolean Difference operation
- Resulting geometry checked and cleaned of artifacts
- Boolean details add genuine visual complexity, not just noise
- Union or additional Boolean use attempted where time allowed

**Scene Cohesion & Scale (30%)**

- All elements combined into one believable, cohesive environment
- Scale consistent throughout, verified against a reference object
- Layout roughly follows the Checkpoint 1 planning sketch
- Overall complexity is a clear step up from the Grade 10 landscape

**Reflection (20%)**

- Thoughtful, specific reflection on the process
- Clear explanation of where Array saved time
- Honest account of Boolean troubleshooting
- Specific comparison drawn to the Grade 10 project

---

## 💡 Key Lesson

Array and Boolean modifiers let you build believable complexity without modeling every single detail by hand — the same non-destructive thinking professional environment artists rely on constantly, and a habit that will directly speed up hard-surface work in Grade 12.
