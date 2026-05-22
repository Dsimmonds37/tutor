# tutor

A personal Claude Code plugin for interactive, all-purpose learning.

## What it does

The `/tutor` skill turns Claude into a patient, Socratic teaching companion. It adapts to any topic, calibrates to your current level, finds real-world examples via web search, gives hands-on challenges, and tracks your progress in a persistent learning journal.

## Learning philosophies embedded

| Philosophy | How it shows up |
|---|---|
| **Socratic method** | Claude asks questions before explaining — guides you to discover answers |
| **Zone of Proximal Development** | Probes your level first, then pitches explanations just beyond it |
| **Constructivism** | Every session includes something to build, write, or try |
| **Feynman technique** | Periodically asks you to explain the concept back |
| **Spaced repetition** | Review mode surfaces least-recently-studied topics |
| **Bloom's taxonomy** | Questions and challenges progress from recall → synthesis |
| **Growth mindset** | Mistakes are reframed as learning signal, never failure |

## Usage

```
/tutor <topic>         Start a new learning session
/tutor review          Review past lessons (spaced repetition)
/tutor quiz <topic>    Run a 5-question quiz on a topic
```

## Files

- `learning-journal.md` — your persistent learning log, auto-updated by the skill
- `plugins/tutor/skills/tutor/SKILL.md` — the skill definition

## Installation

```bash
# Add this repo as a local marketplace
claude plugin marketplace add ~/tutor --name my-skills

# Install the tutor plugin
claude plugin install tutor@my-skills
```
