# Forge — Fitness Planner & Tracker

Forge is an offline-first, dual-mode fitness planner and progressive overload tracker built entirely in a single, self-contained HTML file. It bridges structured 30-day calisthenics progressions with flexible weekly gym splits, complete with transparent autoregulation, RIR-based recovery guidance, rest timers, and offline local media storage.

Zero build steps. Zero runtime dependencies. Zero third-party analytics.

---

## Key Features

### 1. Dual-Mode Training Architecture
* **Calisthenics Mode:** Automatically generates structured 30-day progression blocks (Foundation, Build, Peak, and Taper phases). Supports strength, endurance, or completely custom setups with grease-the-groove (GtG) and deload days.
* **Gym Mode:** Build custom weekly splits or import standard templates (Push/Pull/Legs, Upper/Lower, Full Body, Starting-Strength style). Supports exercise ordering, superset/circuit pairing, and custom rep ranges.

### 2. Autoregulation & Smart Recovery
* **RIR-Driven Guidance:** Calculates fatigue trends using Reps in Reserve (RIR) and suggests progressive overload (+2.5% to +5% weight or reps) or deload recommendations.
* **Soreness & Injury Flags:** Flag specific exercises to automatically reduce planned volume by ~30% and load by ~10% while suggesting movement substitutions.
* **Deload Protocol:** Automatically prompts a deload block after high-volume fatigue cycles or every 4th cycle week.

### 3. Comprehensive Logging & Analytics
* **Unified Streaks & Calendar:** Combined calisthenics and gym streak tracking with a 26-week GitHub-style activity heatmap.
* **Body Metrics & Progress Photos:** Log bodyweight and custom circumference metrics. Stores progress photos locally in browser IndexedDB (avoiding `localStorage` quota limitations) with a split-screen before/after comparison slider.
* **PR Tracking & 1RM Estimations:** Automatic tracking of heaviest lifts, rep personal records, and calculated one-rep maxes (Epley formula).

### 4. Utilities & Offline Tooling
* **Drift-Proof Rest Timer:** Audio beep (Web Audio API) and vibration feedback tuned to exercise intensity and RIR.
* **Gym Calculators:** Plate-loading visualizer (per side) and a percentage-based warm-up ramp generator (40%/60%/80%).
* **Calendar Export:** Download current gym templates as standard `.ics` recurring calendar events.
* **PWA & Shortcuts:** Configured with a Web App Manifest supporting app shortcuts for quick logging.
* **Rule-Based & Enhanced AI Coach:** Native rule-based assistant answering plan queries offline, with an optional BYOK (Bring Your Own Key) hook for OpenAI/Anthropic APIs.

---

## Getting Started

Because Forge is delivered as a single self-contained document, setup requires no installation:

1. Clone or download the repository:
   ```bash
   git clone [https://github.com/your-username/forge-fitness-tracker.git](https://github.com/your-username/forge-fitness-tracker.git)
