# 📱 Mobile App Wireframing — FitTrack

**A UX case study in early-stage design planning: user research → personas → user flows → low-fidelity wireframes.**

> Task type: UX/Product Design exercise
> Tools referenced: Figma / Adobe XD (wireframes in this repo are provided as lightweight SVG mockups so they render directly on GitHub with no external app required — see [Notes on tooling](#notes-on-tooling))

---

## 🎯 The Brief

Design low-fidelity wireframes for a mobile application by working through the full early-stage design process:

1. Conduct basic user research to define user needs
2. Create user personas and user flows
3. Design low-fidelity wireframes
4. Document the design thinking process

**Chosen product: FitTrack** — a mobile app that helps busy, everyday people log workouts, see their progress, and stay consistent without needing to be "gym people." A fitness app was chosen because it has clearly competing user needs (speed vs. detail, motivation vs. simplicity), which makes for a richer UX exercise than a single-purpose utility app.

## 📂 Repository Structure

```
mobile-app-wireframing/
├── README.md                          ← you are here
├── 01-research/
│   └── user-research.md               ← research goals, method, findings, competitive scan
├── 02-personas/
│   └── personas.md                    ← 2 primary user personas
├── 03-user-flows/
│   └── user-flows.md                  ← 3 core user flows (Mermaid diagrams)
├── 04-wireframes/
│   ├── wireframes.md                  ← annotated wireframes with rationale
│   └── images/                        ← 6 low-fidelity screen wireframes (SVG)
└── 05-design-thinking/
    └── design-thinking-process.md     ← Empathize → Define → Ideate → Prototype → Test writeup
```

## 🧭 How to Read This Repo

Read it in folder order — each stage builds on the last:

| Stage | File | What it answers |
|---|---|---|
| 1. Research | [`01-research/user-research.md`](01-research/user-research.md) | Who are we designing for, and what do they actually need? |
| 2. Personas | [`02-personas/personas.md`](02-personas/personas.md) | Who is the "typical" user, concretely? |
| 3. User Flows | [`03-user-flows/user-flows.md`](03-user-flows/user-flows.md) | What steps does a user take to complete their goal? |
| 4. Wireframes | [`04-wireframes/wireframes.md`](04-wireframes/wireframes.md) | What does each screen in that flow look like, structurally? |
| 5. Design Thinking | [`05-design-thinking/design-thinking-process.md`](05-design-thinking/design-thinking-process.md) | How did we get from problem to prototype, and why? |

## 🖼️ Wireframe Preview

| Onboarding | Home Dashboard | Log Workout |
|---|---|---|
| ![Onboarding](04-wireframes/images/01-onboarding.svg) | ![Home](04-wireframes/images/03-home-dashboard.svg) | ![Log Workout](04-wireframes/images/04-log-workout.svg) |

See [`04-wireframes/wireframes.md`](04-wireframes/wireframes.md) for all 6 screens with annotations.

## 🛠️ Notes on Tooling

The brief suggests Figma or Adobe XD, which are the industry-standard tools for this kind of work and are the right choice if you're doing this as a live project. This repo instead ships the wireframes as plain SVG files so that:
- They render natively in the GitHub file browser and README — no account, plugin, or export step needed for a reviewer to see them.
- They stay easy to diff and version in Git (they're just text/XML), which mirrors how a design system's tokens might be tracked.

**To continue this project in Figma/XD:** treat `04-wireframes/wireframes.md` as your screen spec — it lists every element, its rough position, and the interaction each screen supports — and rebuild each frame at 375×812 (iPhone-size artboard) using only grayscale rectangles, lines, and circles (no color, no real copy, no icons) to keep it genuinely low-fidelity.

## ✅ Expected Outcome

By the end of this repo you should be able to see, end to end:
- How a design need is derived from research rather than assumed
- How a persona keeps a team aligned on "who" the design decisions serve
- How a user flow exposes the *minimum* number of screens/steps needed
- How a low-fidelity wireframe forces structural decisions before visual ones

## 📄 License

Provided as an educational template — free to reuse and adapt for coursework, portfolios, or your own case studies.
