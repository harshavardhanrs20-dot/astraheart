# AstraHeart

**Know where your health is heading—even with no link to Earth.**

Live demo: https://harshavardhanrs20-dot.github.io/astraheart/

AstraHeart is an offline-first, single-page astronaut health-monitoring prototype by team **ASTRAQEL**. It combines check-in signals, personal baselines, spaceflight-hazard context, and illustrative risk estimates.

## Features

- Single-file HTML/CSS/JavaScript app with no server, build step, or install.
- Interactive line-art body map with keyboard-accessible hotspots and status-linked details.
- Check-in for heart rate, systolic/diastolic blood pressure, fasting glucose, temperature, sleep, mood, exercise, cabin CO₂, radiation dose, and symptoms.
- Editable, source-labeled clinical/reference bands in the `THRESHOLDS` object near the top of the script. Clinical ranges are general references—not NASA flight limits.
- Explainable risk overview, indicator source popovers, threshold projections, combined patterns, hazard chains, what-if simulator, recommended actions, and offline handoff report.
- 30-day simulated trends, Mars Transit Day 140 walkthrough, Judge mode, and a reset control.
- Best-effort browser `localStorage` persistence.

## How to run

1. Keep `body.png` in the same folder as `index.html`.
2. Open `index.html` in a current desktop or mobile browser.
3. Use **Demo scenario** or **Judge mode** to explore the seeded scenario. No network connection is required to run the app; resource links need internet access.

## Two-minute demo script

1. **0:00–0:20 — Orient.** Introduce AstraHeart and its offline-first purpose. Point out mission day, environment, and comms delay.
2. **0:20–0:40 — Explore the body map.** Select the heart, bones, or brain hotspot. Show the status, linked spaceflight hazard, Earth connection, and action guidance.
3. **0:40–1:00 — Check in.** Open Check-in and review the measurement tips, personal baseline, and cumulative radiation field.
4. **1:00–1:20 — Analyze.** Submit a check-in. Review readiness, cardiac risk, source popovers, contributing signals, and the confidence note.
5. **1:20–1:40 — Explain and act.** Open a hazard chain, adjust sleep or CO₂ in What-if, and show the recommended actions and handoff report.
6. **1:40–2:00 — Show mission behavior.** Start Judge mode or Demo scenario. Follow the Mars Transit Day 140 signal progression, then point to trends and Resources.

## Resources and credits

- [NASA Human Research Program](https://www.nasa.gov/hrp/) — research supporting crew health and the five hazards of human spaceflight.
- Canadian Space Agency, **“Monitoring radiation for astronaut health”** (2026-02-26). The Resources panel credits the article; its direct article URL should be added when confirmed.
- [IEEE Xplore search for CardioLeakGuard-XAI](https://ieeexplore.ieee.org/search/searchresult.jsp?queryText=CardioLeakGuard-XAI). Replace this search link with the verified paper DOI or IEEE record when available.
- `body.png` — local reference line art. **Source/license: add here.**
- Built with AI coding assistance.

## Limitations and future work

- This is a decision-support prototype, not a medical device or diagnosis. Follow onboard medical procedures and flight-surgeon guidance.
- Numeric ranges are general clinical references or explicitly labeled illustrative ranges; they are not NASA flight-specific limits.
- The cardiac-risk hook and explainability bars are placeholders/adaptations, not a validated spaceflight model. The current model metadata and weights are replaceable in `MODEL_CONFIG`.
- Scenario data, wearable sync, and some trends are simulated. The app does not connect to real sensors or transmit reports.
- Future work: integrate real sensor feeds, add voice input, plug in a validated ONNX/JSON model, verify and link the IEEE paper, document the body-art license, and validate thresholds/model behavior with NASA Human Research Program data and flight medical experts.
