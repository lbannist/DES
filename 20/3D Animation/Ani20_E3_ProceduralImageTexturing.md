# 3D Animation 11 – Procedural vs. Image-Based Texturing

## Unit 3: Material Creation & Texturing — Challenge E3

**Time:** 1 Week (3 Class Periods)
**Due Date:** *[insert due date]*

*Builds on Challenges E1–E2 and the UV work from Challenge C2.*

---

## 🎯 Learning Objectives

By the end of this assignment students will:

- Build a procedural texture using Noise and/or Voronoi textures
- Apply an image-based texture using their own UV unwrap
- Use Texture Paint mode to paint details directly onto a model
- Compare the strengths and limitations of procedural vs. image-based approaches

---

## 💭 Production Question

### When is it better to generate a texture with math, and when is it better to paint or photograph one?

---

## Checkpoint 1 — Procedural Texture Build (Day 1)

**✏️ Build with Noise and Voronoi**

1. Add a Noise Texture node in the Shader Editor and connect it into a Color Ramp node to control contrast/banding, then into your Principled BSDF's Roughness or Base Color input.
2. Adjust the Noise Texture's Scale and Detail values and observe how the pattern changes.
3. Try a Voronoi Texture node instead (or combined with Noise) for a more cell-like or scattered pattern, useful for things like stone, dirt speckling, or organic-looking variation.
4. Render test images at a few different Scale values to see how the procedural texture holds up at different levels of zoom — this is one of procedural texturing's key strengths (infinite, non-repeating detail at any scale).

**Requirements**

- At least one procedural texture (Noise and/or Voronoi) driving a material input
- Scale/Detail adjusted and tested at more than one value
- Result applied with visual intent (e.g., realistic roughness variation, not just as a demo)

---

## Checkpoint 2 — Image-Based Texture Application (Days 1–2)

**✏️ Apply an Image Texture Using Your UVs**

1. Select an object with a clean UV unwrap (your Challenge C2 character, or another approved model).
2. Find or create a base color image texture appropriate to your model.
3. Add an Image Texture node, load your image, and connect it to Base Color on the Principled BSDF — the image should map correctly onto the surface using your existing UVs.
4. Check the texture for any obvious stretching or misalignment tied back to your UV layout — if there's a problem, revisit your Challenge C2 UVs rather than just accepting a bad result.

**Requirements**

- Image texture correctly applied using the model's own UV unwrap
- Texture shows no major stretching or misalignment
- Clear connection made between UV quality (from Challenge C2) and texture quality here

---

## Checkpoint 3 — Texture Paint Detail Pass (Days 2–3)

**✏️ Paint Additional Detail**

1. Switch to Texture Paint mode on your object.
2. In the Image Editor (or the paint slot), create or select a new image to paint onto (make sure it's linked to the correct UV map).
3. Use the paint brush to add a hand-painted detail directly onto the model — a scuff, a logo, a color variation, a dirt smudge — something an image texture or procedural texture alone wouldn't easily achieve.
4. Save your painted image (Image → Save As, from within the Image Editor) so the paint work isn't lost when you close the file.

**Requirements**

- At least one hand-painted detail added via Texture Paint mode
- Painted image saved and correctly linked back to the material
- Detail is additive and intentional, not just random scribbling

---

## Checkpoint 4 — Comparison & Reflection

**✏️ Answer:**

1. What kind of surface detail did the procedural texture handle well? What would have been hard to do procedurally?
2. What did the image-based texture let you do that the procedural texture couldn't?
3. How did your Challenge C2 UV quality affect how well the image texture applied?
4. What did texture painting let you add that neither procedural nor plain image texturing could easily achieve?
5. If you were only allowed to use one of these three approaches for a full character, which would you choose, and why?

---

## 📤 Final Submission Requirements

Students must submit all of the following:

**Blender Project File**

Filename: `LastName_ANI2020_E3_TexturingMethods.blend`

**Procedural Texture Renders (at least 2 scale variations)**

Filename: `LastName_ANI2020_E3_Procedural_01.png`, `_02.png`

**Image Texture Render**

Filename: `LastName_ANI2020_E3_ImageTexture.png`

**Texture Paint Detail Render**

Filename: `LastName_ANI2020_E3_PaintedDetail.png`

**Reflection Document**

Filename: `LastName_ANI2020_E3_Reflection.pdf`

---

## 📊 Assessment Criteria

**Procedural Texture (25%)**

- Noise and/or Voronoi texture correctly driving a material input
- Scale/Detail tested at more than one value with clear comparison
- Result applied with genuine visual intent
- Understanding shown of procedural texturing's strengths (infinite, non-repeating detail)

**Image-Based Texture (25%)**

- Image texture correctly applied using the model's UV unwrap
- No major visible stretching or misalignment
- Clear connection made to UV quality from Challenge C2
- Texture choice is appropriate to the model's design

**Texture Painting (25%)**

- At least one intentional hand-painted detail added
- Painted image correctly saved and linked
- Detail adds genuine value not achievable by the other two methods
- Paint work is clean and controlled, not messy or accidental

**Reflection (25%)**

- Thoughtful, specific reflection on all three methods
- Clear, accurate comparison of strengths and limitations
- Honest connection drawn between UV quality and texture results
- Well-reasoned final choice of preferred method with justification

---

## 💡 Key Lesson

Real production texturing almost never uses just one method — procedural, image-based, and hand-painted approaches are usually layered together. Understanding what each does best is what lets you combine them intentionally, rather than defaulting to whichever one you learned first.
