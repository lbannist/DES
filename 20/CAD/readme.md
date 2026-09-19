# CAD 11 — Modules C–F

Grade 11 CAD deep-dive: manufacturing-ready modeling, assemblies, parametric design, and validation. This follows the mandatory, provincial pre-req Grade 11 module (not included in this repo) and runs **11–13 weeks** total.

Each module strips away tutorial support as it goes. By the end of Module F, students can take an unfamiliar physical part and measure it, model it, validate it, and fabricate it — twice, in two different processes — without a tutorial in sight.

## Modules

| Module | Focus | Challenges | Weeks |
| --- | --- | --- | --- |
| [C — Manufacturing-Ready Modeling](#module-c--manufacturing-ready-modeling) | Solid modeling → CAM → real fabrication | 4 | ~3 |
| [D — Assemblies, Fasteners & Handoff Documentation](#module-d--assemblies-fasteners--handoff-documentation) | Threaded parts, multi-part assemblies, documentation that works for someone outside CAD | 3 | ~2–3 |
| [E — Parametric Design](#module-e--parametric-design) | Named parameters, external constraints, design tables | 4 | ~3 |
| [F — Validation & Reverse-Engineering Capstone](#module-f--validation--reverse-engineering-capstone) | Stress analysis, real-world fit, final fabrication in a substitute material | 3 | ~3–4 |

---

## Module C — Manufacturing-Ready Modeling

**~3 weeks | 4 challenges**

| # | File | Challenge |
| --- | --- | --- |
| C1 | [CAD11_UnitC_C1_SparkPlugCAM.md](./CAD11_UnitC_C1_SparkPlugCAM.md) | Spark plug tutorial series: model + generate/simulate CAM toolpath |
| C2 | [CAD11_UnitC_C2_IndependentPartCAM.md](./CAD11_UnitC_C2_IndependentPartCAM.md) | Model a new part from a dimensioned drawing and produce its CAM toolpath, independently |
| C3 | [CAD11_UnitC_C3_ToyPlaneModel.md](./CAD11_UnitC_C3_ToyPlaneModel.md) | Model a simplified toy airplane from reference photos alone, split into fabricable parts |
| C4 | [CAD11_UnitC_C4_ToyPlaneFabrication.md](./CAD11_UnitC_C4_ToyPlaneFabrication.md) | CAM, CNC-cut (or 3D print), and assemble the toy plane; revise the model based on real fit |

## Module D — Assemblies, Fasteners & Handoff Documentation

**~2–3 weeks | 3 challenges**

| # | File | Challenge |
| --- | --- | --- |
| D1 | [CAD11_UnitD_D1_ScrewCapAssembly.md](./CAD11_UnitD_D1_ScrewCapAssembly.md) | Model a two-part threaded screw-cap assembly; match pitch and clearance |
| D2 | [CAD11_UnitD_D2_AdirondackChairHandoff.md](./CAD11_UnitD_D2_AdirondackChairHandoff.md) | Adirondack chair tutorial series + BOM + exploded view, packaged into Lego-style build plans for a non-CAD builder |
| D3 | [CAD11_UnitD_D3_ReverseEngineeredProduct.md](./CAD11_UnitD_D3_ReverseEngineeredProduct.md) | Reverse-engineer a real multi-part product by measurement alone; model, assemble, document |

## Module E — Parametric Design

**~3 weeks | 4 challenges**

| # | File | Challenge |
| --- | --- | --- |
| E1 | [CAD11_UnitE_E1_ParametricTire.md](./CAD11_UnitE_E1_ParametricTire.md) | Parametric tire design series; produce variants by changing driving parameters only |
| E2 | [CAD11_UnitE_E2_ParametricEnclosure.md](./CAD11_UnitE_E2_ParametricEnclosure.md) | Electronics enclosure with dimensions derived from an external component spec |
| E3 | [CAD11_UnitE_E3_DesignTableFamily.md](./CAD11_UnitE_E3_DesignTableFamily.md) | Design table / configuration generating a family of part variants from one spreadsheet |
| E4 | [CAD11_UnitE_E4_ParametricCapstone.md](./CAD11_UnitE_E4_ParametricCapstone.md) | **Capstone:** live, unsupported build combining external-spec derivation, range-robust patterns, and a design table |

## Module F — Validation & Reverse-Engineering Capstone

**~3–4 weeks | 3 challenges**

| # | File | Challenge |
| --- | --- | --- |
| F1 | [CAD11_UnitF_F1_StressAnalysisFundamentals.md](./CAD11_UnitF_F1_StressAnalysisFundamentals.md) | Stress analysis fundamentals on the Xbox controller shell; apply to a reverse-engineered mechanical part |
| F2 | [CAD11_UnitF_F2_FitValidationIteration.md](./CAD11_UnitF_F2_FitValidationIteration.md) | 3D print, fit-check against the real assembly (bolts, mating parts), iterate design, re-validate stress |
| F3 | [CAD11_UnitF_F3_WoodCapstone.md](./CAD11_UnitF_F3_WoodCapstone.md) | **Capstone:** CAM + CNC-route the final design in wood; compare stress results across materials |

---

## File naming convention

`CAD11_Unit[C–F]_[Challenge#]_[ShortDescription].md`

Each challenge file includes: learning objectives, a production question, 2–3 checkpoints with requirements, a reflection section, final submission requirements with exact filenames, weighted assessment criteria, and a key lesson.
