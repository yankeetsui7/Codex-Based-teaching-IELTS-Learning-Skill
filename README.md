# Codex Based teaching IELTS Learning Skill

An evidence-based Codex skill for planning, teaching, adapting, and reviewing long-term IELTS learning.

## Why this skill was created

Long-term IELTS study often becomes a collection of disconnected exercises. A learner may finish many questions without knowing whether a skill has transferred, while lesson plans become overloaded with corrective rules, repeated rewriting, and temporary tasks.

This skill was created to give Codex a stable teaching framework while keeping the learner's changing targets, calendar, weaknesses, and daily evidence separate. Its purpose is not to force every learner through one syllabus. It helps Codex make consistent decisions about:

- what to teach next;
- how much to teach in one session;
- when to stop repeating a task;
- how to respond to fatigue or a schedule change;
- what counts as evidence that a skill is becoming stable;
- how Agent-based self-study and lessons with a human teacher inform each other.

## What the skill defines

### A four-level planning system

The skill connects:

1. **Final target** — exam date or window and score requirements;
2. **Monthly Aim** — the capability milestone for the natural month;
3. **Weekly Ambition** — a small set of observable results for the natural week;
4. **Daily Target** — the task that fits the learner's current time, energy, dependencies, and progress.

Lower-level tasks must support the higher-level goal. Extra exercises are not added merely because they may be useful.

### A concise learning loop

Each substantive task follows a default sequence:

```text
define the objective and success evidence
→ teach the necessary method or callable language
→ run a short controlled application when needed
→ test transfer with unfamiliar material and less prompting
→ assess the primary and secondary objectives
→ close, defer, or repair precisely
```

The loop is normally validated once or twice. Repetition is not treated as progress by itself.

### Three completion branches

- If the primary and secondary objectives are achieved, the task closes.
- If the primary objective is achieved but a secondary issue remains, that issue is classified as blocking, natural-recurrence, low-impact observation, or closed.
- If the objectives are not achieved, Codex diagnoses the answer, asks where the learner is stuck, teaches the precise problem, and performs another useful validation rather than restarting the entire lesson.

### Evidence and record rules

The skill distinguishes controlled practice, independent transfer, and exam-style performance. It preserves original answers, time, and prompting level when they affect later decisions.

A dated study report is required after a substantive session. Weekly Reviews are required at natural-week boundaries. Full lesson plans, specialist reviews, and attention-test records are created only when they have future value.

### Calendar and fatigue adaptation

When calendar access exists, Codex reads real availability before planning. The learner's current message takes precedence over a stale or missing calendar event.

Attention checks are used only when they help decide whether to continue, reduce load, switch, rest, or stop. The skill does not turn attention testing into another fixed exercise quota.

### Two learning modes

- **Codex self-study:** Codex organizes teaching, output, assessment, adaptation, and records.
- **Human-teacher collaboration:** the learner debriefs the offline lesson to Codex; Codex adjusts self-study and prepares useful information to report back to the teacher.

The skill preserves disagreements between learner, Codex, and human teacher until later evidence resolves them.

### Subject-specific routing

- **Writing:** moves from task understanding and callable language to independent transfer. Low-impact Task 1 issues should not indefinitely delay Task 2.
- **Reading and Listening:** can use targeted error removal instead of complete subject teaching when the learner already has a reliable method and strong baseline.
- **Speaking:** prioritizes continuous speech and fewer disruptive pauses before memorized complexity, followed by vocabulary that can actually be called under time pressure.

## What the skill needs

The skill works best with:

- a private learner profile created from `references/profile-template.md`;
- an exam target or approximate exam window;
- the latest reliable component scores or equivalent evidence;
- current monthly and weekly goals;
- the latest study report and any unfinished task;
- the learner's available time, fatigue, and task preference for the current session;
- original answers, actual time, and prompting level when performance is being assessed;
- optional calendar access for realistic scheduling;
- optional debrief information from a human IELTS teacher.

Missing information should be requested only when it would materially change the session. Codex should not repeat questions already answered in the learner's private profile.

## Privacy model

This public repository contains only reusable instructions and blank templates. A learner's scores, calendar events, unavailable dates, study reports, original answers, and teacher debriefs should stay in a private workspace.

Calendar access authorizes reading only when planning requires it. It does not authorize creating, moving, or deleting events.

## Repository structure

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── workflow.md
    └── profile-template.md
```

- `SKILL.md` is the skill entry point.
- `references/workflow.md` contains the stable teaching and planning rules.
- `references/profile-template.md` is copied into a private learner workspace and completed there.
- `agents/openai.yaml` provides Codex UI metadata.

## Installation

Copy the repository into the Codex skills directory so that `SKILL.md` remains at the skill root. Then invoke `$ielts-learning-coach`, or allow Codex to select it automatically for relevant IELTS planning, study, feedback, and debrief requests.

Before first use, create the private learner profile. Do not complete the profile inside a public clone that will be committed and pushed.

## Intended boundary

This skill is a learning workflow, not an official IELTS scoring service and not a replacement for reliable test materials or professional judgment. A controlled exercise result should not be presented as a precise score increase. The user's current instruction always takes precedence over the skill.
