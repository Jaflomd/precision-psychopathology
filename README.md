# Precision Psychopathology

One-pager bedside Mental State Examination (bMSE) scorer with dimensional psychopathology profiles.

**Live app:** https://jaflomd.github.io/precision-psychopathology/

## Features

- **28 clinical dimensions** scored in a single page (bipolar, gate, profile, conviction, multitest, two-axis)
- **Capa 2 outcomes** — 3ST/Klonsky (suicide risk), BVC/Brøset (aggression), Diogenes pattern (self-neglect), Appelbaum-Grisso (decision-making capacity)
- **HiTOP/Forbes per-feeder grid** — no aggregation, configuration-based clinical signals
- **RDoC and bMSE radars** — SVG visualizations of 21+27 constructs
- **Brain Inference** — real-time inference of implicated networks (CEN, DMN, SAL, DA-Str, Reward, OFC-Amy, HPC, LC-NE)
- **Clinical narrative report** — auto-generated prose for copy-paste into EMR
- **Mobile-ready** — touch targets ≥44px, bottom action bar, responsive viewport down to 320px
- **Keyboard shortcuts** — S (sweep normals), T (confirm tentatives), 1-5 / 0 / Tab / Arrows
- **Local persistence** — state stored in `localStorage`, no server, no auth, no PHI leaves the device

## Architecture

- `index.html` — single-file app (HTML + CSS + JS render layer)
- `bmse-data.js` — shared catalog: dimension definitions, HITOP/RDoC/BMSE maps, calc helpers, Capa 2 outcomes, Brain Inference, MSE narrative generator
- No build step, no dependencies, no external API calls

## Authorship

Co-developed by:
- Dr. Jeff Huarcaya-Victoria — [@psiquiatrahuarcaya](https://www.instagram.com/psiquiatrahuarcaya)
- Dr. Javier Flores-Cohaila — [@jaflo.md](https://www.instagram.com/jaflo.md)

## Disclaimer

Clinical decision support tool, not a diagnostic instrument. Capa 2 outcomes provide configuration-based clinical signals, not probabilistic predictions. Large 2017 (PPV 0.4% for suicide tools) and Fazel 2012 (PPV ~41% for violence tools) — use the trace, not the score.
