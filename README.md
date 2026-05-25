# VR Therapeutic Modules for Bedridden Patients

**Bachelor Thesis · Czech Technical University in Prague · 2025**

> Unity · C# · Meta Quest 2 & 3 · XR Interaction Toolkit · Android Platform

---

## Overview

A set of interactive VR therapeutic modules for bedridden seniors — designed for cognitive and physical stimulation, accessibility, and independent use. Built as my bachelor thesis by extending and refactoring an existing Unity VR rehabilitation application (originally a Master's thesis project).

**Platform:** Meta Quest 2 / 3 (Android)  
**Status:** Functional prototype — tested with real patients at a Czech senior care facility

---

## What I built

- **Two original VR mini-games** with purpose-built mechanics for elderly users — engagement, low motor demand, and clear feedback loops
- **Audio tutorial system** — voice-guided instructions for every module, enabling independent use without staff assistance
- **Refactored and extended legacy codebase** — analyzed the prior Master's thesis Unity project, identified architecture issues, and restructured before extending
- **Accessibility-first interaction design** — input choices, UI scale, and feedback tuned through hands-on observation with real users

---

## Technical stack

| Area | Details |
|------|---------|
| Engine | Unity (URP) |
| Language | C# |
| XR | XR Interaction Toolkit 2.5, XR Hands 1.3, OpenXR |
| Platform | Meta Quest 2/3 via `com.unity.xr.oculus` |
| Build | Android mobile pipeline (Meta Quest is Android) |
| Research | `cz.leosrehacek.vr_dashboard_logger` — CTU telemetry package for usage logging |
| Shaders | Shader Graph (hand shader, interaction feedback materials) |

---

## Engineering highlights

- **Legacy code integration** — inherited a complex multi-scene Unity project; analyzed undocumented systems, refactored for clarity and extensibility, then built on top
- **Android/Meta Quest build pipeline** — configured Unity for Quest target, managed XR plugin stack, resolved platform-specific interaction issues
- **User-Centered Design loop** — requirements gathered through direct observation of seniors and caregivers; iterated on interactions until accessible and reliable under real conditions
- **XR Interaction Toolkit** — hand tracking, spatial UI, and grab/trigger interactions implemented within the XRI framework

---

## User testing

Tested hands-on with senior patients and care staff at a real facility in the Czech Republic. Accessibility and UX were refined through multiple observation rounds — not from a spec, but from watching real users struggle and succeed.

---

## How to run

1. Open in Unity 2022 LTS or later
2. Configure XR: Project Settings → XR Plug-in Management → enable Oculus / OpenXR
3. Build to Meta Quest via Android build target, or connect a Quest and use Link for Play mode
