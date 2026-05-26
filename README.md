# -Yield-Optimization-of-TSMC-28nm-Virtual-Fab-Using-Sequential-RSM-and-Six-Sigma-in-JMP-
Virtual 9-stage TSMC 28nm fab simulation in JMP using sequential RSM and Six Sigma (DMAIC). Achieved >90% yield, tracked cascading defects, and optimized Cpk from 0.94 to 3.84.

# Yield Optimization for TSMC 28nm via Virtual Fab Simulation in JMP

**Project Objective:** Improve semiconductor manufacturing yield through a virtual 9-stage production line simulation.

**Key Result:** Achieved **>90% final yield** and studied cascading defect propagation across stages with process robustness via RSM.

---

## 🏭 Manufacturing Stages (1→9)

1. Silicon Substrate
2. CVD (Deposition)
3. Photolithography
4. Etching
5. Ion Implantation
6. Annealing
7. Final Clean
8. CMP
9. Packaging

---

## 🛠️ Tools & Methodology (3 Items)

1. **JMP** – DOE, RSM, Process Capability, Profiler, Predictor Screening
2. **Six Sigma (DMAIC)** – Define, Measure, Analyze, Improve, Control
3. **Physics & Engineering Basis** – Arrhenius kinetics, Mack's lithography model, Preston's CMP equation, Ion implantation stoichiometry, Plasma etch dynamics, and cascaded hereditary noise propagation

---

## 📐 Three Steps for DOE & Master Table

**Step 1:** Design separate DOE per stage via `DOE → Custom Design → RSM` (30 runs each)

**Step 2:** Add physics-based equations with `Random Normal(0, σ)` for natural process noise

**Step 3:** Cascade stages via `Tables → Update` and join into `Master.jmp` via `Tables → Join`

---📂 How to Open the Project
Click on Master.jmp file in this repository.

Click the three dots (...) → Select "View".

Click "Download" to save the file to your computer.

Open the downloaded file in JMP Statistical Software.

On the left panel, click the green play button next to any script to run the analysis.

All models (Distribution, Process Capability, Fit Model, Profiler) are saved as executable scripts inside the table.

📌 This README file contains detailed methodology, stage-by-stage analysis, and optimization steps.

## 📊 Final Results

| Metric | Baseline | After Optimization |
|--------|----------|---------------------|
| Overall Yield | ~68% | **>90%** |
| Cpk (Lithography) | 1.06 | **3.84** |
| Cpk (CVD) | 0.94 | **1.34** |
