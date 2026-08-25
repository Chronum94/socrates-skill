# Socrates Skill

**A tutor, not an answer machine.** Guides you to your own conclusions through
questioning — across code, science, humanities, and anything else you're trying
to understand.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)
[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-Open%20Standard-blue?style=for-the-badge)](https://skills.sh)

## Quick Install

```bash
npx skills add Chronum94/socrates-skill
```

<details>
<summary>Other installation methods</summary>

**Claude Code**

```bash
claude install-skill Chronum94/socrates-skill
```

**Manual (Git clone)**

```bash
git clone https://github.com/Chronum94/socrates-skill.git ~/.claude/skills/socrates
```

</details>

## The idea

Most tutoring skills implement "never give the answer," which fails immediately
in contact with reality: you cannot reason your way to the fact that Python has
a GIL, or that Hastings was 1066. Withholding a *fact* isn't Socratic — it's
guess-what-I'm-thinking, and it's why people dislike the method.

This skill draws the line differently:

> **Give premises freely. Never give conclusions.**

Facts, definitions, notation, API signatures, dates — handed over without
ceremony the moment they're relevant. What follows *from* them is yours to work
out.

## What makes it different

**It knows when to stop.** Hard overrides drop the method entirely for
safety-critical situations, distress, medical/legal/financial specifics, live
incidents, and any clear request to just be told. Consent is not optional and
isn't negotiated.

**It has an escape hatch.** A seven-rung assistance ladder from open question
down to full explanation-plus-re-derivation, descended on specific signals
(guessing, degrading answers, frustration) rather than a strike count. No
infinite loops, no twenty-question death march.

**It knows its own limits.** An epistemic gradient governs how it questions: on
settled material it leads confidently; on contested material it flags the
dispute; at the frontier — exact figures, citations, niche APIs — it says it may
be fabricating and shifts to teaching *verification* instead. The goal is that
you leave able to check claims, including its own.

**It matches your level.** Jargon and complexity are held to what's actually been
established — either taught earlier in the session, or confirmed as ground you can
stand on. No performing sophistication at someone who hasn't got there yet.

**It reaches across fields.** Structural analogy is treated as a primary tool —
feedback loops, conservation, bottlenecks, selection effects and the rest recur
everywhere, and the tutor's job is to make you notice when the thing in front of
you is the thing you already understand from somewhere else.

**It's grounded in the actual literature**, including the parts that argue
against it. Unguided discovery learning is empirically weak for novices; the
skill knows this and adapts rather than pretending otherwise.

## Coverage

Four domain playbooks, because the method genuinely differs by field:

| Family | Includes |
|---|---|
| **STEM reasoning** | Math, physics, chemistry, biology, statistics, CS theory — prediction-first, limiting cases, documented misconception catalog |
| **Code & systems** | Debugging, architecture, code reading, performance — predict-then-run, hypothesis bisection, urgency overrides |
| **Humanities & interpretive** | Philosophy, literature, history, ethics, law — evidence discipline, steelmanning, and a tutor that can lose the argument |
| **Acquisition & applied** | Language learning, memorization-dense fields, medicine, strategy, personal decisions — where naive Socratic fails hardest |

## Trigger

Explicitly opt-in. It never hijacks a normal question.

| Trigger | Example |
|---|---|
| `socratic` / `Socrates` | "Socratic mode — walk me through this auth flow" |
| `tutor me` / `teach me` | "Tutor me through this proof" |
| `don't just tell me` | "Don't just tell me why this segfaults" |
| `quiz me` / `guide me` | "Quiz me on this chapter" |
| `소크라테스` | "소크라테스님, 이 문제는 어떻게 풀어야 할까요?" |

## How a session runs

1. **Calibrate** — one compact turn establishing goal, starting point, time available
2. **Read** — the tutor works through the material fully before asking anything, and
   pivots to questioning toward *verification* where the ground truth isn't settled
3. **Question** — minimal framing, step size re-judged every answer, and question
   density scaled to what you can keep up with: a single question when the step is
   hard, several in parallel or cascade when you're moving fast
4. **Adapt** — ascend on traction, descend the ladder on stall signals, supply premises on sight
5. **Verify** — a *novel* case you haven't seen, because "yes, I understand" is not evidence
6. **Close** — the principle in your words, what's still open, one thread to pull alone

## Structure

```
SKILL.md                    Operating core — doctrine, overrides, ladder, loop
references/
  questions.md              Question taxonomy, cross-domain transfer, bad-question catalog
  casebook.md               ~30 edge cases with scripts
  domains.md                Per-field playbooks
  assessment.md             Transfer tests, teach-back, diagnosing wrong answers
  epistemics.md             Settled → contested → frontier; verification protocol
  pedagogy.md               Cited theory, and when this method is the wrong tool
```

Reference files load on demand, so a normal session doesn't carry all of it.

## Language

Mirrors whatever language you write in.

## Credits

Expanded from the original [socrates-skill](https://github.com/RoundTable02/socrates-skill)
by RoundTable02.

## License

MIT
