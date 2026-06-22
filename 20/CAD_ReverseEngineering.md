# Fusion 360 Reverse Engineering Challenge
## Object Reproduction & Technical Drawing

---

## Overview

You have spent several weeks learning Fusion 360 by following guided tutorials. You know how to sketch, extrude, revolve, fillet, and create assemblies. Now it is time to work like a real engineer.

In this challenge you will be given a **physical object** — an **outdoor hose bib (exterior water tap)** — and asked to measure it, model it in Fusion 360, and produce a complete set of **engineering drawings** that a machinist or manufacturer could use to build it. No step-by-step instructions are provided. You must make decisions, solve problems, and justify your choices.

**Duration:** 5–10 classes (approximately 300–500 minutes of work)

---

## Learning Goals

By the end of this challenge you will be able to:

- Measure a real-world object accurately using calipers and a ruler
- Break a complex object into simple geometric features (extrusions, revolves, sweeps, threads)
- Reconstruct those features in Fusion 360 without a tutorial
- Apply constraints and dimensions correctly so the model is fully defined
- Create a multi-view engineering drawing with standard orthographic projections
- Add dimensions, tolerances, surface finish notes, and a title block
- Communicate your design intent through annotations a machinist could follow

---

## Tools & Materials You Will Need

- The physical assembly (i.e. outside hose bib)
- Digital calipers (class set — sign one out)
- Steel rule
- Pencil, graph paper, or printed measurement worksheet
- Fusion 360
- Printed or on-screen copy of this challenge sheet

---

## Phase 1 — Measure & Sketch

**Goal:** Produce a complete hand-drawn sketch with all dimensions before touching Fusion 360.

---

### Step A — Examine Before You Measure

Before picking up the calipers, spend five minutes just looking at and handling the object. This is not wasted time — professional engineers call it a *design review* and it prevents costly mistakes later.

Ask yourself these questions and write your answers in your notebook:

**How does it rest?**
Set the object down on the desk. Does it sit flat? Does it roll? Does it need to be propped up? The **surface it naturally rests on is a strong candidate for your datum face** — the reference surface all your measurements will come from. Identify and label it before you measure anything. If the object rolls or does not have a clear resting face, look for the most prominent flat surface — a machined shoulder, a flat base, or one face of a hex or square feature.

**What are the distinct features?**
Go around the object systematically — do not jump randomly. Start at one end and work to the other. For each feature you encounter, write it down and note:
- Is it flat or curved?
- Is it round (cylindrical / conical) or prismatic (hex / square / rectangular)?
- Does it have a pattern — is it repeated, mirrored, or evenly spaced?
- Is it a separate piece attached to the main body, or all one piece?
- Are there any threads? (Set these aside for Phase 1.5 — finish all other features first.)

Aim to identify every distinct feature before measuring any of them. A typical object in this challenge will have between 5 and 12 distinct features.

**Are there any patterns or symmetry?**
Symmetry saves modelling time. If a part has two identical arms, two matching holes, or a repeating pattern of ribs or slots, you only need to model one instance in Fusion 360 and mirror or pattern the rest. Identify any symmetry now and note it on your feature list — you will come back to it in Phase 2.

---

### Step B — Establish a Datum

A **datum** is a known reference point, edge, or face that all other measurements are taken from. Using a consistent datum means your dimensions chain together logically and errors do not compound the way they do when you measure randomly from different places.

**How to choose your datum:**
- The datum face should be flat, stable, and easy to place against a flat surface (your desk or a square).
- Look for a machined shoulder, a flat base, or the largest flat face on the object — these are typically the most accurate surfaces on a manufactured part.
- Mark your chosen datum clearly on your sketch with a small triangle symbol **▽** and the label **DATUM A**.

**How to use your datum:**
Once you have Datum A, measure every length *from that face*, not from the previous feature. This is called **datum dimensioning** and it is standard practice in manufacturing.

Example — instead of measuring:
- Outlet end = 25 mm long
- Thread-to-body transition = 8 mm (measured from where the outlet ends)
- Body = 40 mm (measured from where the transition ends)

Measure everything from Datum A:
- Outlet end ends at 25 mm from Datum A
- Transition ends at 33 mm from Datum A
- Body ends at 73 mm from Datum A

If you make a small error in one measurement, it does not cascade into every measurement after it.

> **Why does this matter?** If you measure feature-to-feature and one dimension is 1 mm off, everything downstream shifts by 1 mm. If you measure from a datum, each feature is only as wrong as that one measurement — the error stays isolated.

---

### Step C — Create Your Hand Sketches

Draw the at least 3 of the following views on graph paper, large enough to write dimensions on clearly. Neatness counts — these sketches are your data sheet for the whole project.

- **Front view** (looking at what you consider the natural "face" of the object)
- **Side view** (looking from the left or right)
- **Top view** (looking straight down)
- **End view(s)** of any cylindrical ends, holes, or features that are not visible in the three standard views
- **Cross-section sketch** — estimate what the inside looks like based on what you can observe at openings, holes, or ends

Label your datum face on every view where it appears, using the **▽ DATUM A** symbol and a brief note describing what that face is (e.g. *rear shoulder*, *flat base*, *bottom hex flat*).

---

### Step D — Measure Systematically

Now pick up the calipers. Work view by view, feature by feature, always measuring from Datum A where possible. Record every measurement directly on your sketch — do not write numbers on a separate sheet and transfer them later.

**Minimum measurements to record for every object:**

| What to measure | Tool | Notes |
|---|---|---|
| Overall length (Datum A to far end) | Calipers or rule | Your most important baseline |
| Location of every shoulder, step, or transition (from Datum A) | Calipers | This is datum dimensioning — measure from A, not feature-to-feature |
| Outer diameter of every cylindrical feature | Calipers | Measure in two perpendicular directions and average |
| Across-flats width of every hex or square feature | Calipers | Count the number of flats (6 = hex, 8 = octagon, 4 = square) |
| Height/length of every hex or square feature | Calipers | |
| Width and thickness of flat arms, tabs, or flanges | Calipers | |
| Diameter and depth of any holes | Calipers | Note if the hole is blind (closed end) or through |
| Fillet and chamfer sizes (estimate) | Calipers or eyeball | Measure with calipers where possible; estimate where not |

**Measuring round features (cylinders):**
Measure the diameter in two perpendicular directions and record both. If they differ by more than 0.5 mm, average them and note that the part is slightly out-of-round (common on cast and moulded parts). Do not guess — never assume a feature is perfectly circular.

**Measuring hex features:**
The across-flats dimension (the wrench size) is more useful than the across-corners dimension. Measure across flats with your calipers. Confirm the number of flats by counting before you sketch the polygon.

**Threads — record only the location and rough diameter for now.**
You will identify and classify threads properly in Step E. For now, just note on your sketch: *"threaded feature here, approx. Ø__ mm, length __ mm."*

BEFORE MOVING ON - Build your assembly with what you know right now.  It might take some forward and backwards up and down the Fusion timeline to minimize the amount of stpes required.  Also there won't be threads until you start Phase E.

TEACHER REVIEW - Have your teacher check over the assembly made and double check some critical measurements.   Accuracy is IMPORTANT!!

---

### Step E — Thread Identification

Threads are tackled last because they require a different approach from everything else. You cannot simply measure a thread diameter and call it done — threads follow published standards, and identifying the correct standard is what lets Fusion 360 (and a machinist) reproduce them accurately.

Work through the following process for **each threaded feature** on your object, one at a time.

---

#### Step E1 — Confirm It Is Actually a Thread

Look closely. Not every spiral or groove is a standard thread. Ask:
- Do you see a continuous helical ridge wrapping around a cylinder or into a hole?
- Does it look consistent — same pitch, same depth, the whole way along?
- Is the diameter noticeably smaller (for external threads) or larger (for internal threads) than the feature it is on?

If yes, it is a thread. Mark it on your sketch with a note: *"threaded — to be classified."*

---

#### Step E2 — Is It External or Internal?

**External thread** — the thread is on the outside of a cylinder (a bolt, a stud, a pipe end, a nozzle).
**Internal thread** — the thread is on the inside of a hole (a nut, a threaded insert, a threaded port).

Note which type each threaded feature is. This determines how you will create it in Fusion 360 later.

---

#### Step E3 — Is It Straight or Tapered?

Look at the threaded section from the side:
- **Straight (parallel):** The cylinder stays the same diameter all the way along the thread. The thread crests form a straight line parallel to the centreline.
- **Tapered:** The cylinder gets slightly narrower toward the tip. If you hold a ruler alongside the threaded section, you can see the taper.

Pipe threads used in plumbing and gas fittings are often tapered (e.g. NPT). Machine fasteners, hose fittings, and most bolts are straight. **Taper matters** because Fusion 360 applies the taper geometry automatically once you select the right standard — but only if you identify it correctly.

---

#### Step E4 — Measure the Thread Diameter

Using your calipers, measure:
- **External thread:** measure the **major diameter** — the largest diameter, across the tips of the crests.
- **Internal thread:** measure the **minor diameter** — the diameter of the hole itself (the root of the thread).

Write this measurement on your sketch. Remember to measure in two perpendicular directions and average. The actual thread standard diameter will be the nearest **nominal size** in the standard tables — your measured value will be close but not exact.

---

#### Step E5 — Estimate the Thread Pitch

Thread pitch is the distance between adjacent thread crests (in mm) or the number of threads per inch (TPI) depending on the standard.

**Method 1 — Count over a known length:**
Using your calipers, mark off exactly 25 mm along the threaded section. Count the number of complete thread crests within that 25 mm span.

- If you counted in mm: pitch (mm) = 25 ÷ number of crests
- If you are working in inches: TPI = (number of crests ÷ 25) × 25.4

**Method 2 — Thread pitch gauge (if available):**
Your classroom may have a thread pitch gauge — a fan of thin metal blades, each with a different tooth spacing. Lay each blade against the thread until one fits perfectly (teeth mesh cleanly with the crests). Read the pitch from the blade label.

Write your estimated pitch on your sketch next to the thread diameter.

---

#### Step E6 — Identify the Thread Standard

Now use your diameter measurement and pitch estimate together to look up the thread standard in Appendix A or the reference cards provided. The goal is to match your measurements to a **named standard** — the standard is what gets entered into Fusion 360, not the raw numbers.

**Common thread standards you may encounter:**

| Standard | Where you'll see it | Key characteristic |
|---|---|---|
| **UNC** (Unified National Coarse) | Bolts, screws, general fasteners | Imperial, coarse pitch, most common fastener thread |
| **UNF** (Unified National Fine) | Precision fasteners, thin-walled parts | Imperial, fine pitch, more threads per inch than UNC |
| **Metric (M)** | Modern fasteners, European parts | Metric diameter and pitch (e.g. M10 × 1.5) |
| **NPT** (National Pipe Taper) | Plumbing, gas, fluid fittings | Tapered, seals on thread engagement |
| **NPS** (National Pipe Straight) | Plumbing couplings | Straight, same form as NPT but no taper |
| **BSP** (British Standard Pipe) | Older plumbing, imported fittings | Common in UK, Australia, and older Canadian plumbing |
| **GHT / NH** (Garden Hose Thread) | Hose fittings, outdoor taps | Straight, larger pitch, 3/4 in – 11.5 NH is the most common |

**To confirm the standard:**
1. Find the row in the standard table where the nominal diameter matches your measurement (within 1–2 mm).
2. Check that the pitch or TPI also matches your estimate.
3. If both match, you have identified the standard. If only one matches, check adjacent sizes — you may have measured across the wrong diameter (major vs. minor).

Write the full thread callout on your sketch:
- Metric example: `M12 × 1.75`
- Imperial example: `1/2 – 13 UNC`
- Pipe example: `3/4 NPT`
- Hose example: `3/4 – 11.5 NH`

---

#### Step E7 — Note the Thread Length

Measure the length of the threaded section from where the threads begin to where they end (or to the shoulder). This tells Fusion 360 how long to apply the thread feature.

Record: *"Thread starts at __ mm from Datum A, ends at __ mm from Datum A. Thread length = __ mm."*

---

#### Step E8 — When No Standard Matches: Custom Threads Using the Coil Tool

Sometimes your object will have a thread that does not match any standard in the library — an older part, a proprietary fitting, or a non-standard pitch. When that happens, Fusion 360's built-in Thread feature cannot reproduce it accurately, and you will need to model the thread geometry manually using the **Coil tool**.

**What you need to know before using the Coil tool:**

To build a custom thread you must have measured and recorded all of the following. Go back to the physical object and confirm each value before modelling:

| Value | What it means | How to measure it |
|---|---|---|
| **Major diameter** | The largest diameter — across the crest tips on an external thread | Calipers across the outer peaks |
| **Minor diameter** | The smallest diameter — across the root valleys | Calipers inside a nut, or calculate: major Ø − (2 × thread depth) |
| **Pitch** | Distance in mm from one crest to the next | Count crests over 25 mm, divide 25 by the count |
| **Threads per inch (TPI)** | Alternative to pitch for imperial threads | Count crests over 25.4 mm (1 inch) |
| **Thread depth** | Radial height of one thread tooth | (Major Ø − Minor Ø) ÷ 2 |
| **Thread angle** | Angle of the flanks (sides) of the tooth profile | 60° for most UN/Metric; 55° for BSP; check reference card if unsure |

**How to create the custom thread in Fusion 360:**

1. Model the base cylinder at the **minor diameter** (the core shaft, without threads).
2. Go to `Create > Coil`.
3. On a plane passing through the centreline, sketch a small triangle representing your thread tooth. Dimension the height to match the thread depth and the angle to match the thread angle.
4. Set the coil **pitch** to your measured pitch value.
5. Set the coil **height** to match the thread length.
6. Set `Operation: Cut` so the coil removes material from the shaft (for an external thread).
7. For an **internal thread** (a threaded hole), model the hole at the **major diameter** first, then use the coil to cut inward toward the minor diameter.

**Why matching male and female threads is critical:**

A custom coil thread only works if the mating part is modelled with exactly the same specifications. If the male thread (external) and the female thread (internal) do not share identical pitch, major diameter, minor diameter, and thread angle — they will not thread together in real life or in a Fusion 360 interference check.

Think of it this way: the gap between the male crest and the female root must be consistent all the way around, with just enough clearance for the parts to engage smoothly. Even a 0.1 mm difference in pitch will cause the threads to bind after just a few turns. When modelling both sides of a custom thread:

- Use the **same sketch profile** for both male and female tooth — copy it rather than redrawing it from memory.
- Add a small **clearance** (typically 0.1–0.2 mm on the diameter) to the female thread to allow assembly. Standard thread tables include this automatically; for custom coils you must add it manually.
- Confirm that pitch, depth, and angle are identical on both parts before moving on.

**Verify with Section Analysis:**

Once both the male and female threaded components are modelled, do not assume they are correct — **verify them visually** using Fusion 360's Section Analysis tool before finalizing anything.

1. In the Design workspace, go to `Inspect > Section Analysis`.
2. Select a plane that cuts through the centreline of the threaded pair — the XZ or YZ origin plane usually works.
3. Fusion 360 shows a live cross-section through both parts simultaneously.
4. Zoom in on the thread engagement zone and check:
   - Do the male crests sit cleanly inside the female roots without overlapping?
   - Is there a consistent, even gap (clearance) visible around the full thread profile?
   - Are the pitches aligned — do the crests and roots line up at every thread, not crest-to-crest?
5. **If threads overlap (interference):** the major or minor diameter is too large — increase the female clearance.
6. **If the gap looks sloppy and uneven:** tighten the clearance or recheck your pitch measurement.
7. **If crests are hitting crests:** your pitch values do not match — go back and correct one of the coil definitions before proceeding.

> **Why section analysis matters:** A 3D shaded view can look convincing even when two parts would physically collide or fail to engage. Section analysis removes the outer surfaces and shows the geometry underneath — it is the closest thing to sawing the real part in half to check your work. Always run it before calling a threaded pair complete.

---

#### Quick Check — Before Moving On

For each threaded feature, you should now have recorded:

- [ ] External or internal?
- [ ] Straight or tapered?
- [ ] Measured major or minor diameter (in mm)
- [ ] Estimated pitch (mm) or TPI
- [ ] Identified thread standard and nominal size (or confirmed no standard matches — custom coil required)
- [ ] Thread length and location from Datum A
- [ ] Full thread callout written on sketch (or custom spec table if no standard applies)

If any item is missing, go back to the object and measure it before you close your sketchbook.

---

---

### First-Timer Tips — Phase 1

These are the most common mistakes students make the first time they measure a real object. Read them now so you do not have to learn them the hard way.

**Tip 1 — Sketch first, measure second.**
Never start measuring without a sketch to write on. If you collect numbers without a drawing to anchor them, you will forget what you measured within ten minutes.

**Tip 2 — Write the unit on every number.**
Write `42 mm`, not just `42`. When you come back to your sketch tomorrow, you will not remember whether a number was in mm or cm.

**Tip 3 — The object is not perfect — and that is okay.**
Real manufactured parts have casting draft, shrinkage, machining marks, and wear. Your model should represent the *design intent* — the ideal geometry — not every imperfection. If a face looks like it should be flat but measures 0.3 mm off flat, model it as flat.

**Tip 4 — Round to the nearest 0.5 mm for cast or moulded features, 0.1 mm for machined features.**
Threads, mating surfaces, and precision fits are machined — keep those to 0.1 mm. The general body of a casting or moulded part does not need sub-millimetre precision.

**Tip 5 — If a feature looks symmetric, check if it actually is.**
Two arms, two holes, two flanges — measure both. If they differ by less than 1 mm, treat them as equal and note it on your sketch. If they differ more, record the actual measurements for each.

**Tip 6 — Calipers measure what they touch, not what you think they touch.**
Make sure the caliper jaws are seated squarely against the feature. A tilted caliper gives a larger reading than the true diameter. Practice on a known object (like a coin) until you get a consistent reading.

**Tip 7 — Do not try to identify threads from a single measurement.**
Thread identification requires diameter *and* pitch together. A bolt that is 12 mm in diameter could be M12 × 1.25, M12 × 1.5, or M12 × 1.75 — three different threads with the same diameter. Always estimate the pitch before looking up the standard.

**Tip 8 — You will probably need to re-measure something in Phase 2.**
That is normal and expected. Keep your sketches accessible during the modelling phases. Professional engineers call this *going back to the part* and it is a sign of good practice, not failure.

**Tip 9 — Photograph your object from multiple angles.**
Before returning the object at the end of class, take 4–6 photos from different angles. Include close-up shots of any threaded features and transitions. Reference photos are invaluable when you are modelling in class 3 and cannot remember what a transition looked like.

> **Remember:** A machinist working from bad measurements will make a bad part. The time you invest in Phase 1 pays off in every phase that follows.

---

### Deliverable — Phase 1

Hand in (or photograph and upload) your annotated hand sketches with:
- Datum A clearly marked on every view
- All measurements recorded in mm, directly on the sketch
- Feature list completed in your notebook
- Patterns and symmetry noted
- Thread callouts recorded for every threaded feature (using Phase 1.5 checklist)

Your teacher must approve your Phase 1 sketches before you open Fusion 360.

---

## Phase 2 — Body & Main Features (Classes 2–3)

**Goal:** Build the core body of the hose bib in Fusion 360.

### Suggested Workflow

Work in this order. You may need to adjust based on how your object differs from a typical hose bib.

**Step A — Create a new component**
Name it `Hose_Bib_Body`. Everything goes inside this component.

**Step B — Outlet end (hose thread side)**
Start with the outlet — it is roughly cylindrical and gives you a strong anchor point.
- Sketch a circle on the origin plane. Dimension it to match the outer diameter you measured.
- Extrude it to the correct length.
- Add the GHT thread using `Create > Thread`. Check **Modeled** so the thread geometry appears. Use the 3/4 in – 11.5 NH standard.

**Step C — Valve body**
The body is typically a hex or octagonal prism with rounded ends.
- Sketch a regular polygon (Inscribed or Circumscribed — use the across-flats measurement to choose).
- Extrude or use a combination of extrude and fillet to shape the body.
- The transition from the hex body to the cylindrical ends is a good place to use chamfers or fillets — observe your part closely.

**Step D — Inlet end (pipe thread side)**
- Model the male NPT end similar to the outlet.
- Use `Create > Thread > Tapered` to represent NPT. Check **Modeled**.
- NPT is tapered at 1:16 — Fusion 360 handles this automatically when you select the NPT standard.

**Step E — Packing nut**
- Model as a separate hex feature sitting between the body and the stem area.
- Dimension from your measurements.

### Deliverable — Phase 2

Save and submit your Fusion 360 file at the end of Class 3. The body, outlet, inlet, and packing nut should be visible and roughly proportioned. It does not need to be perfect — you will refine in Phase 3.

> **Stuck?** If you cannot figure out how to model a specific feature, sketch it on paper first and show your teacher. You are allowed to simplify — for example, you may represent threads as a cylinder with a note on the drawing rather than full helical geometry if performance is an issue.

---

## Phase 3 — Handle & Refinement (Classes 4–5)

**Goal:** Complete the model and refine proportions.

### Tasks

**Handle**
Hose bib handles vary. Yours may be:
- A T-bar (two rectangular arms extending from a centre hub)
- An oval grip with a centre slot
- A cross (four spokes)

Model it accurately from your measurements. Consider:
- Starting with a sketch of the handle's profile
- Using Extrude with a symmetric offset from the centre plane
- Adding fillets to match the real object's rounded edges

**Refinement**
Go back through each feature and compare your model to the physical object:
- Are proportions correct?
- Do transitions between features look right?
- Are threads the correct length?
- Does the handle sit at the right height relative to the body?

**Appearances (optional)**
Apply a Brass appearance to the body and a different colour to the handle if your object has a painted handle. This is cosmetic only — it does not affect the drawing.

### Deliverable — Phase 3

Updated Fusion 360 file with the complete model. Take a screenshot of a shaded 3D view and paste it into your progress log.

---

## Phase 4 — Engineering Drawing Setup (Class 6)

**Goal:** Create a drawing file from your model using Fusion 360's Drawing workspace.

### Tasks

1. **Open the Drawing workspace.** Go to `Design > Drawing > From Design`.

2. **Set drawing standard and units.**
   - Standard: ASME Y14.5 (North American)
   - Units: mm
   - Sheet size: A3 (420 × 297 mm) or your teacher's preference

3. **Insert a base view.**
   - Choose the Front view as your base.
   - Scale: 1:1 if it fits, or 1:2 if the object is large.

4. **Add projected views.**
   From the base view, project:
   - Right Side view
   - Top view
   - An Isometric view (place it in the lower right)

5. **Add a Section view.**
   Cut through the centreline of the body to show the internal passage. Label it `SECTION A-A`.

6. **Add a Detail view** (optional but recommended).
   Zoom in on one of the threaded ends. This makes thread callouts legible.

### Deliverable — Phase 4

A drawing file with at minimum 4 views: Front, Right Side, Top, and Isometric. Section view is required. Save and submit the drawing file.

---

## Phase 5 — Dimensions & Annotations (Classes 7–8)

**Goal:** Fully dimension your drawing so a machinist can build the part without seeing the model.

### Dimensioning Rules

Follow these ASME rules — your teacher will check for them:

- Every feature must have at least one dimension.
- Do **not** duplicate dimensions — dimension each feature once.
- Extension lines must not cross dimension lines if avoidable.
- Dimension text must be horizontal (unidirectional style).
- Leave at least 10 mm between the part outline and the first dimension line.
- Leave at least 7 mm between stacked dimension lines.

### Required Dimensions

Place these on the appropriate views:

| Dimension | Where to place it |
|---|---|
| Overall length | Front view, below the part |
| Body hex width across flats | Front or Top view |
| Outlet thread diameter and length | Front view or Detail view |
| Inlet thread diameter and length | Front view |
| Packing nut height and hex width | Front or Side view |
| Handle length and width | Top or Front view |
| All significant diameters | Section A-A |

### Thread Callouts

Threads are called out with a leader note, not a diameter dimension alone. Format:

```
3/4 – 11.5 NH (GHT) — for the outlet
3/4 NPT — for the inlet
```

In Fusion 360 Drawing: use `Annotate > Leader` and type the thread callout manually.

### Title Block

Fill in the title block completely:

| Field | What to enter |
|---|---|
| Part Name | Outdoor Hose Bib |
| Part Number | HB-001 |
| Material | Brass (or as observed) |
| Scale | 1:1 or 1:2 |
| Drawn By | Your name |
| Date | Today's date |
| School / Class | Your class code |
| Sheet | 1 of 1 |

### Deliverable — Phase 5

Fully dimensioned drawing with thread callouts and completed title block. Print a PDF or export as a PDF for submission.

---

## Phase 6 — Review, Corrections & Submission (Classes 9–10)

**Goal:** Peer review, final corrections, and formal submission.

### Peer Review (Class 9)

Exchange your printed or on-screen drawing with a partner. Each reviewer uses the checklist below. Mark each item **Pass** or **Needs Work** with a brief comment.

**Drawing Review Checklist**

- [ ] Front, Side, Top, and Isometric views are present and correctly oriented
- [ ] Section view cuts through the centreline and is labelled A-A
- [ ] All views are the same scale (or scale is noted per view)
- [ ] No features are missing a dimension
- [ ] No dimensions are duplicated across views
- [ ] Thread callouts use correct standard format
- [ ] Title block is fully completed
- [ ] Lines follow correct line types (visible, hidden, centreline, phantom)
- [ ] Overall drawing is clear and legible at the stated scale
- [ ] The drawing could realistically be used by a machinist to build the part

After review, write two specific improvements you will make based on your partner's feedback.

### Final Corrections (Class 10)

Make all corrections identified in the peer review. Then submit:

1. **Fusion 360 model file** (.f3d)
2. **Drawing PDF** (exported from Fusion 360 Drawing)
3. **Reflection paragraph** (see below)

---

## Reflection (Submitted with Final Package)

Write 150–250 words responding to these prompts:

- What was the hardest part of this challenge, and how did you solve it?
- Which Fusion 360 tools did you use that you had not used in previous tutorials?
- If you were going to machine this part from brass rod stock, which features would be most difficult to produce and why?
- How is a detailed engineering drawing different from a 3D render or screenshot of your model? Why does the drawing still matter?

---

## Marking Rubric

| Category | 4 — Excellent | 3 — Proficient | 2 — Developing | 1 — Beginning |
|---|---|---|---|---|
| **Measurement accuracy** | All dimensions within ±0.5 mm of actual object; measurements well documented | Most dimensions accurate; minor errors in 1–2 features | Several dimensions off; limited documentation | Measurements missing or significantly inaccurate |
| **Model quality** | All features modelled; correct proportions; threads modelled; fillets/chamfers present | Most features present; minor proportion issues | Key features missing or poorly shaped | Model does not resemble the object |
| **View selection & projection** | All required views present; correctly projected; section view correct | Minor projection errors; all views present | One view missing or significantly incorrect | Multiple views missing or incorrect |
| **Dimensioning** | Fully dimensioned; no duplicates; correct placement; thread callouts correct | Mostly dimensioned; 1–3 errors or omissions | Partial dimensioning; several errors | Few or no dimensions |
| **Title block & annotations** | Title block complete; notes and callouts professional | Minor omissions in title block | Several fields missing | Title block mostly empty |
| **Reflection** | Insightful; references specific tools and challenges; connects to real manufacturing | Addresses all prompts; adequate depth | Addresses some prompts; surface level | Minimal or off-topic |

**Total: /24**

---

## Quick Reference — Useful Fusion 360 Tools for This Challenge

| Task | Where to find it |
|---|---|
| Polygon sketch | Sketch > Polygon (Circumscribed or Inscribed) |
| Thread feature | Solid > Create > Thread |
| Fillet / Chamfer | Solid > Modify > Fillet / Chamfer |
| Shell (hollow body) | Solid > Modify > Shell |
| Mirror feature | Solid > Create > Mirror |
| New drawing | Design > Drawing > From Design |
| Section view | Drawing toolbar > Section View |
| Detail view | Drawing toolbar > Detail View |
| Leader / Note | Drawing > Annotate > Leader |
| Center marks | Drawing > Annotate > Center Mark |

---

## Appendix A — Thread Reference

| Thread Type | Use | Nominal Size | Pitch / TPI |
|---|---|---|---|
| NPT | Pipe inlet (tapered, seals on threads) | 3/4 in | 14 TPI |
| GHT / NH | Garden hose outlet (straight, seals on washer) | 3/4 in | 11.5 TPI |

In Fusion 360, select thread standard **ANSI Unified Screw Threads** for GHT or **ANSI Pipe Threads** for NPT. Enable **Modeled** to see thread geometry in the 3D view.

---

## Appendix B — Engineering Drawing Line Types

| Line type | Appearance | Use |
|---|---|---|
| Visible line | Thick solid | Edges you can see |
| Hidden line | Thin dashed | Edges behind a surface |
| Centreline | Thin, long-short-long dash | Axes of symmetry, hole centres |
| Cutting plane | Thick, long-short-short-long | Shows where a section cut is made |
| Section line (hatch) | Thin lines at 45°, evenly spaced | Fills cut surfaces in a section view |
| Dimension / Extension | Thin solid | Dimension strings |
| Leader | Thin solid with arrowhead | Notes and callouts |

Fusion 360 Drawing applies most line types automatically. You may need to manually add centrelines using `Annotate > Center Mark` or `Center Line`.

---

*Challenge designed for Grade 10 Technology / Engineering — CAD Unit*
*Prerequisite projects: Lego Block, Birdhouse, Snap-Fit Case, Black Pipe Lab*
