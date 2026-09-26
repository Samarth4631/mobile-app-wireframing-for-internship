# User Research — FitTrack

## 1. Research Goals

Before designing anything, we need to answer three questions:

1. What stops people from tracking their workouts consistently today?
2. What do people actually want to know about their own progress?
3. What existing tools are people using (or abandoning), and why?

## 2. Method

A lightweight, low-cost research method appropriate for early-stage/student projects:

| Method | Sample | Purpose |
|---|---|---|
| Short survey (8 questions, mix of multiple choice + 1 open text) | 15–25 respondents | Find patterns in behavior and drop-off points |
| Semi-structured interviews (15–20 min) | 5 respondents, mix of gym-goers and non-gym exercisers | Understand *why* behind the survey patterns |
| Competitive/comparative app review | 4 existing fitness apps | Identify gaps and over-served features |

### Sample survey questions
- How do you currently track your workouts, if at all? (app / notebook / memory / spreadsheet / I don't)
- On a typical week, how many workouts do you complete vs. plan?
- What's the #1 reason you stop using a fitness app after the first week?
- What would make you *feel* like you're making progress, even on a slow week?
- How much time do you want to spend logging a single workout? (under 30 sec / under 2 min / don't mind longer)

### Sample interview prompts
- Walk me through the last time you exercised — what happened right before and right after?
- Tell me about an app or method you tried and stopped using. What happened?
- What does "progress" look like to you, in your own words?

## 3. Key Findings

**Finding 1 — Logging friction kills consistency.**
Most respondents who had tried a fitness app abandoned it within 2 weeks, and the most common reason given was that logging a workout took "too many taps" or required entering data they didn't have on hand (exact weights, sets, rest timers).

**Finding 2 — Motivation comes from visible trends, not raw numbers.**
People didn't want more data; they wanted a simple visual answer to "am I doing better than last week?" Raw exercise logs without a summarized trend were described as "just a diary nobody reads."

**Finding 3 — Two very different user types exist.**
- *Casual/beginner exercisers* want the app to ask as little of them as possible and just confirm "you did something today."
- *Consistent/intermediate exercisers* want more structure (routines, history, personal records) but still resent extra taps.

**Finding 4 — Onboarding overload is a drop-off point.**
Apps that front-load account creation, permissions requests, and long questionnaires before showing any value lost users immediately, according to both survey comments and interviews.

**Finding 5 — Streaks and simple stats motivate more than badges/gamification.**
A visible streak or "3 workouts this week" counter was mentioned far more positively than points, levels, or badges, which several people found "gimmicky."

## 4. Competitive Scan (informal)

| App | Strength | Gap we can exploit |
|---|---|---|
| App A (established tracker) | Deep exercise database | Heavy, slow logging flow; steep learning curve |
| App B (habit tracker, non-fitness-specific) | Extremely fast to log | No fitness-specific context (sets/reps/duration) |
| App C (social fitness app) | Strong community/motivation loop | Requires social profile setup, feels like a commitment |
| App D (wearable companion app) | Automatic tracking | Requires owning specific hardware |

**Opportunity:** a fitness app that logs a workout in under 3 taps, shows a simple weekly trend instead of dense stats, and never requires hardware or a social profile to get value on day one.

## 5. Defined User Needs

Translating findings into needs the design must satisfy:

- **N1.** Users need to log a workout in as few taps as possible, without mandatory detail entry.
- **N2.** Users need a simple, glanceable way to see whether they're trending up or down week to week.
- **N3.** Users need to get to real app value (logging something) before being asked to create an account or grant permissions.
- **N4.** Users need the app to scale from "just log that I moved" to "show me structured history," without forcing either mode on the other type of user.
- **N5.** Users need light, non-gimmicky motivation (streaks, simple counts) rather than heavy gamification.

These five needs directly inform the personas and user flows in the next sections.

---
*Note: this is a template research process for a design exercise. In a real project, replace the sample findings above with data from your own actual surveys/interviews.*
