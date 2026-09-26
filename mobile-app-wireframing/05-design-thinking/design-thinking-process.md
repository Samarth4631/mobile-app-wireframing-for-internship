# Design Thinking Process — FitTrack

Documenting the reasoning behind each stage, following the standard Empathize → Define → Ideate → Prototype → Test model.

---

## 1. Empathize

**Goal:** Understand real behavior around fitness tracking before assuming a solution.

- Ran a short survey (8 questions) and 5 informal interviews (see [`../01-research/user-research.md`](../01-research/user-research.md)).
- Deliberately talked to a mix of consistent exercisers and people who had *tried and quit* fitness apps — the quitters turned out to be more informative than the loyal users.
- Reviewed 4 existing apps to see where competitors already serve users well, so effort wasn't spent re-solving a solved problem.

**Key mindset:** avoid designing for "a fitness person" in the abstract — design for the specific friction points people described.

## 2. Define

**Goal:** Turn raw findings into a sharp, actionable problem statement.

> **Problem statement:** People who want to build a basic exercise habit abandon tracking apps within the first two weeks — not because they lack motivation, but because logging a single workout takes too much time and upfront setup, and the payoff (seeing progress) is buried in dense data or gamified noise they don't trust.

From this, five concrete user needs were defined (N1–N5, see research doc), and two personas (Maya, Daniel) were built to represent the two behavior clusters uncovered in interviews. Defining *two* personas instead of one was itself a design decision — it kept the team honest about who might be under-served by any single flow.

## 3. Ideate

**Goal:** Generate and narrow options before committing to a flow.

Options considered for the core logging interaction:
1. **Full form logging** (sets/reps/weight required every time) — rejected: directly recreates the friction found in research.
2. **Fully automatic tracking via sensors** — rejected for this scope: depends on hardware/permissions, fails N3 (no barrier to first value) and adds engineering scope beyond a wireframe exercise.
3. **Two-tier quick-log + optional detail** (chosen) — a single screen with a fast default path and a collapsed, optional expansion for detail. This was chosen because it's the only option that serves both personas without branching into two separate apps.

The same two-tier thinking was then applied to onboarding (optional account creation) and to progress (trend-first, detail-on-demand), keeping the whole app consistent in philosophy: **show the simple version first, let the user opt into complexity.**

## 4. Prototype

**Goal:** Make the ideas concrete enough to evaluate, at the lowest cost that still tests the idea.

- Built low-fidelity wireframes (grayscale, no real copy, no icons) for the 6 screens covering all 3 core flows — see [`../04-wireframes/wireframes.md`](../04-wireframes/wireframes.md).
- Deliberately stayed low-fidelity: the open question at this stage is "does the *structure* work," not "does it look good." Adding color or polished type too early tends to make reviewers comment on aesthetics instead of flow.
- Each wireframe was checked against the flows in [`../03-user-flows/user-flows.md`](../03-user-flows/user-flows.md) to confirm every step in a flow has a corresponding, unambiguous screen.

## 5. Test (recommended next steps)

Not conducted as part of this exercise (no live prototype/users available), but the intended test plan is documented so the project can be picked up and continued:

- **Method:** 5-user moderated usability test using a clickable prototype built from these wireframes (e.g., in Figma).
- **Tasks to test:**
  1. "You just opened the app for the first time — get to your first logged workout."
  2. "Log a second workout as quickly as you can."
  3. "Check whether you did more or less this week than last week."
- **Success signals:** Task 1 completed without creating an account (validates N3); Task 2 completed in under 3 taps (validates N1); Task 3 answered by glancing at the Progress screen without opening full history (validates N2).
- **What would trigger a redesign:** if users instinctively look for sets/reps fields on the main Quick Log screen (rather than treating it as optional), the "optional detail" pattern may need to be more discoverable, not less.

---

## Summary

Every structural choice in this repo — deferred sign-up, the 2-tap/4-tap dual-speed logging screen, and the trend-first progress view — traces back to a specific research finding. That traceability (finding → need → persona → flow → wireframe) is the actual deliverable of early-stage design work; the wireframes themselves are just where it becomes visible.
