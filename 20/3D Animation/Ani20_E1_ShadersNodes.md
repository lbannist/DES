# 3D Animation 11 – Shader Editor & Node Fundamentals

## Unit 3: Material Creation & Texturing — Challenge E1

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*


---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Navigate the Shader Editor and understand node-based material thinking
- Use the Principled BSDF as an all-purpose shader
- Mix multiple shaders together using a Mix Shader node
- Organize complex node setups into reusable Node Groups

---

## 💭 Production Question

### If a material is just a set of connected instructions, what's the smallest set of nodes that gets a convincing result?

---

## Checkpoint 1 — Shader Editor Navigation (Day 1)

**📖 Node-Based Thinking**

1. Select any object and open the Shader Editor workspace tab.
2. Identify the default Principled BSDF node and the Material Output node it connects to.
3. Practice adding a new node (Shift + A in the Shader Editor) and connecting/disconnecting it from the Principled BSDF's inputs.
4. Change the Base Color input directly, then try plugging a simple Color node (e.g., an RGB node) into it instead, and compare the two approaches.
5. Zoom out in the Shader Editor and note how even a simple material can get visually complex fast — good node organization matters.

**Questions to answer:**

1. What does the Principled BSDF node represent, in plain language?
2. What's the difference between typing a color directly into an input versus plugging in a Color node?

---

## Checkpoint 2 — Mixing Shaders (Days 1–2)

**✏️ Combine Two Shaders**

1. Add a second shader node (e.g., a second Principled BSDF, or a Glossy/Transparent shader) alongside your first.
2. Add a Mix Shader node and connect both shaders into its two shader inputs.
3. Control the mix using the Mix Shader's Fac (factor) input — try a flat value first, then try plugging in a Fresnel node or a Layer Weight node to make the mix vary based on viewing angle.
4. Render a test image and observe how the Fresnel/Layer Weight-driven mix creates a more realistic edge effect (e.g., a subtle rim highlight) compared to a flat mix value.

**Requirements**

- At least two shaders combined using a Mix Shader node
- Mix factor driven by something other than a single flat value (Fresnel, Layer Weight, or a texture)
- Test render clearly shows the effect of the mix

---

## Checkpoint 3 — Node Groups (Days 2–3)

**✏️ Organize a Reusable Node Group**

1. Build a small, reusable node setup (e.g., a simple dirt/grime effect using a Noise texture feeding into a Color Ramp, then into a Mix Shader).
2. Select all the nodes involved and press Ctrl + G to group them into a Node Group.
3. Rename the Node Group clearly (double-click its name) so it's identifiable later.
4. Add Node Group inputs (in the group's own editing view, using the N-panel's Group input/output sockets) for at least one adjustable parameter, such as the Noise scale or the dirt amount.
5. Apply this Node Group to a second material on a different object, adjusting its exposed parameters to fit the new context.

**Requirements**

- A Node Group created from at least three connected nodes
- At least one exposed, adjustable input on the Node Group
- Node Group successfully reused on a second material

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. What does the Principled BSDF let you control, and what surprised you about its options?
2. How did driving your Mix Shader's factor with Fresnel/Layer Weight change the result compared to a flat value?
3. Why would you bother creating a Node Group instead of just rebuilding the same nodes each time?
4. What's one material effect you'd like to try building with nodes in a future project?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI2020_E1_ShaderNodes.blend`

**Node Setup Screenshot**

Filename: `LastName_ANI2020_E1_NodeSetup.png`

**Test Render**

Filename: `LastName_ANI2020_E1_TestRender.png`

**Reflection Document**

Filename: `LastName_ANI2020_E1_Reflection.pdf`

---

## 📊 Assessment Criteria

**Shader Editor Navigation (20%)**

- Comfortable adding, connecting, and disconnecting nodes
- Clear understanding shown of what the Principled BSDF represents
- Correct use of both direct value inputs and node-driven inputs
- Node graph is reasonably tidy and readable

**Mixed Shader Setup (30%)**

- At least two shaders combined via Mix Shader
- Mix factor driven by Fresnel, Layer Weight, or a texture rather than a flat value
- Test render clearly demonstrates the intended effect
- Effect is applied with visual intent, not just as a technical exercise

**Node Group Construction (30%)**

- Node Group built from a genuinely reusable combination of nodes
- At least one useful, exposed input parameter
- Node Group successfully reused on a second material
- Group clearly named and organized for future reuse

**Reflection (20%)**

- Thoughtful, specific reflection on the process
- Clear explanation of the Fresnel/Layer Weight-driven mix effect
- Honest reasoning for why Node Groups are useful
- Specific idea for a future node-based material effect

---

## 💡 Key Lesson

Once you think in nodes instead of single settings, materials become endlessly combinable — the same handful of building blocks (mix, ramp, noise, Fresnel) show up again and again in completely different-looking materials. This is the foundation for every material built for the rest of this unit and into Grade 12.
