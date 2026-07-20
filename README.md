# 🚁 PID Control — From Absolute Zero to a Self-Hovering Drone

An interactive, visual, beginner-friendly course that teaches **PID control** by building a
**1D drone altitude hover simulator** step by step. Designed for someone with **decent programming
but weak math/physics** — every idea is taught with **intuition → visualization → animation → code
→ (only then) math**, never equations first.

You will *not* memorize formulas. You will understand **why** every behaviour happens.

---

## ✅ What's in this build

All **10 notebooks are complete and fully runnable**. Every notebook was executed end-to-end in a
headless kernel and verified to run with **zero errors** — including all animations and interactive
sliders. Notebooks ship **without saved outputs** (so they're small and clean); everything
regenerates when you run them.

| # | Notebook | Status | Teaches |
|---|----------|--------|---------|
| 01 | `01_Dynamic_Systems.ipynb` | ✅ **Complete** | position, velocity, acceleration, time steps, Euler integration, animation |
| 02 | `02_Forces_and_Gravity.ipynb` | ✅ **Complete** | force, mass, Newton's 2nd law, gravity, free fall, thrust, manual hover |
| 03 | `03_Open_vs_Closed_Loop.ipynb` | ✅ **Complete** | open vs closed loop, sensor, target, error, feedback, bang-bang control |
| 04 | `04_P_Controller.ipynb` | ✅ **Complete** | proportional gain, overshoot, rise/settling time, steady-state error |
| 05 | `05_I_Controller.ipynb` | ✅ **Complete** | steady-state error, integral action, windup, anti-windup |
| 06 | `06_D_Controller.ipynb` | ✅ **Complete** | derivative, prediction/damping, noise amplification, filtering |
| 07 | `07_Complete_PID.ipynb` | ✅ **Complete** | combining P+I+D, controller class, real-time dashboard |
| 08 | `08_PID_Tuning.ipynb` | ✅ **Complete** | manual tuning, per-gain effects, parameter sweeps, Ziegler–Nichols |
| 09 | `09_Practical_Control.ipynb` | ✅ **Complete** | noise, actuator limits, wind, delay, robustness |
| 10 | `10_Final_Drone_Project.ipynb` | ✅ **Complete** | polished interactive simulator + challenge problems |

---

## ▶️ How to run

### Option A — Google Colab (recommended, zero setup)
1. Go to [colab.research.google.com](https://colab.research.google.com).
2. `File → Upload notebook` and pick, e.g., `01_Dynamic_Systems.ipynb`.
3. Run cells top to bottom (**Shift+Enter**). Run the **Setup cell** first.
4. If an animation ever looks blank, just re-run that one cell.

### Option B — Local Jupyter
```bash
pip install -r requirements.txt
jupyter notebook      # then open the notebooks in order
```

---

## 🧭 How to study
- Do the notebooks **in order** — each builds on the last (with a quick recap at the top).
- Actually attempt the 🧪 **Exercises** before opening the `▸ Reveal` hints/solutions.
- Play with every 🎛️ **slider** — the intuition comes from experimenting, not from reading.

## 🎓 The whole course in one paragraph
Measure the error. **P** pushes proportional to it (fast, but leaves a gap and can oscillate).
**I** accumulates it over time (erases the gap, but can wind up). **D** reacts to its rate of change
(damps and anticipates, but amplifies noise). Add the three, defend against the real world with
anti-windup and derivative filtering, and *tune* the balance for the disturbances you face.

## 📦 Dependencies
Only **numpy**, **matplotlib**, and **ipywidgets** — nothing else. Everything is implemented by
hand so the mechanics are never hidden.

## 📁 Structure
```
PID_Course/
├── 01_Dynamic_Systems.ipynb        ✅ complete
├── 02_Forces_and_Gravity.ipynb     ✅ complete
├── 03_Open_vs_Closed_Loop.ipynb    ✅ complete
├── 04_P_Controller.ipynb           ✅ complete
├── 05_I_Controller.ipynb           ✅ complete
├── 06_D_Controller.ipynb           ✅ complete
├── 07_Complete_PID.ipynb           ✅ complete
├── 08_PID_Tuning.ipynb             ✅ complete
├── 09_Practical_Control.ipynb      ✅ complete
├── 10_Final_Drone_Project.ipynb    ✅ complete
├── README.md
├── requirements.txt
├── assets/            (notebooks self-generate all plots; no external images needed)
└── solutions/         (worked solutions for 01–03; solutions for 04–10 are embedded in each notebook)
```

Happy hovering. 🚁
