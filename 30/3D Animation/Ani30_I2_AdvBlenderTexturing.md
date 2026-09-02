# 3D Animation 12 – Advanced Blender Texturing & Look Development

## Unit 3: Hard-Surface Modeling, Texturing & Look Development — Challenge I2

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Gr11's Material Creation & Texturing unit.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Use Fresnel and Layer Weight nodes for edge-based shading effects
- Use Color Ramps for stylized shading control
- Layer multiple surface looks on one object using Mix Shader
- Add Subsurface Scattering or a Clear Coat layer for refined, believable materials

---

## 💭 Production Question

### What's the difference between a material that's technically correct and one that actually looks expensive?

---

## Checkpoint 1 — Fresnel & Layer Weight Effects (Day 1)

**📖 Edge-Based Shading Study**

1. Add a Fresnel node to a material's Shader Editor and connect it into a Mix Shader's Fac input, mixing between two different shaders (e.g., a base color and a bright rim-like shader).
2. Render and observe how the effect changes based on viewing angle — edges facing away from camera should show more of the second shader.
3. Try swapping the Fresnel node for a Layer Weight node and compare the difference in the resulting falloff.
4. Adjust the Fresnel's IOR (index of refraction) value and note how it changes the sharpness of the edge effect.

**Questions to answer:**

1. What's the practical visual difference between Fresnel and Layer Weight?
2. What real-world material property does this edge-based effect help simulate?

---

## Checkpoint 2 — Color Ramps for Stylized Shading (Days 1–2)

**✏️ Control Shading with Color Ramps**

1. Add a Color Ramp node between a Fresnel/Layer Weight output (or a Shader to RGB node from your lighting) and a color input, to create stylized banding rather than smooth gradients.
2. Adjust the Color Ramp's stops and interpolation mode (Linear, Constant, Ease) and observe how each creates a different stylized look.
3. Apply this to at least one material where a stylized (rather than fully photorealistic) look is the goal.

**Requirements**

- Color Ramp used to control at least one shading effect
- At least two different interpolation modes tested and compared
- Result applied with clear stylistic intent

---

## Checkpoint 3 — Advanced PBR: Subsurface Scattering or Clear Coat (Days 2–3)

**✏️ Add a Refined Material Layer**

1. Choose a material that would benefit from Subsurface Scattering (skin, wax, marble) or Clear Coat (varnished wood, car paint, glossy plastic).
2. On the Principled BSDF, enable and adjust the relevant setting — Subsurface Weight/Radius/Color, or Coat Weight/Roughness.
3. Render before/after comparisons to confirm the setting is adding a genuine, noticeable improvement rather than an unnoticeable tweak.
4. Adjust values until the effect looks convincing at your chosen render distance/scale.

**Requirements**

- Subsurface Scattering or Clear Coat applied to at least one material
- Before/after comparison clearly shows the improvement
- Values tuned specifically for the object's scale and intended look

---

## Checkpoint 4 — Reflection

**✏️ Answer:**

1. Where did the Fresnel/Layer Weight edge effect add the most believability to your material?
2. How did the Color Ramp change a smooth gradient into something more stylized?
3. What convinced you that your Subsurface Scattering or Clear Coat setting was actually working, versus just being technically present but invisible?
4. How do these refined shading techniques compare to what you'll be able to achieve with Substance Painter (if you're on the Game Art stream) or continued Blender work (if you're on the Animation stream)?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI3030_I2_AdvancedTexturing.blend`

**Fresnel/Layer Weight Comparison Render**

Filename: `LastName_ANI3030_I2_EdgeEffect.png`

**Subsurface/Clear Coat Before/After Renders**

Filename: `LastName_ANI3030_I2_Refined_Before.png`, `_After.png`

**Reflection Document**

Filename: `LastName_ANI3030_I2_Reflection.pdf`

---

## 📊 Assessment Criteria

**Fresnel/Layer Weight Application (25%)**

- Edge-based effect correctly built and connected
- Both Fresnel and Layer Weight tested and compared
- Effect applied with a clear real-world material in mind
- IOR or falloff value adjusted with intent

**Color Ramp Use (20%)**

- Color Ramp correctly used to control a shading effect
- At least two interpolation modes tested and compared
- Result shows clear stylistic intent

**Advanced PBR Layer (35%)**

- Subsurface Scattering or Clear Coat correctly applied
- Clear, convincing before/after improvement demonstrated
- Values appropriately tuned for the object's scale and material type
- Effect reads correctly at the intended render distance

**Reflection (20%)**

- Thoughtful, specific reflection on the process
- Clear explanation of where the edge effect added believability
- Honest assessment of the advanced PBR layer's visible impact
- Fair comparison drawn to the stream-specific texturing path ahead

---

## 💡 Key Lesson

The gap between "technically correct" and "looks expensive" is almost always these smaller refinements — edge falloffs, subtle banding control, subsurface or coat layers. Every student builds this same eye for refinement here, whether their next step is Substance Painter or continued Blender work.
