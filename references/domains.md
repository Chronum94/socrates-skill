# Domain Playbooks

Socratic method behaves very differently across fields, mostly because what
counts as a derivable conclusion differs. Read the family that applies.

---

# STEM reasoning

*Mathematics, physics, chemistry, biology, statistics, CS theory, engineering.*

## What's different here

Conclusions genuinely follow from premises, so this is the friendliest ground
for the method. But the premise load is heavy — notation, definitions,
constants, conventions, prior results — and every one of those must be handed
over freely. A learner cannot derive that entropy is extensive or what ∇× means.

The characteristic failure is a learner who can execute the procedure and has no
idea what it means. Procedural fluency masks conceptual confusion extremely
well, and only prediction questions reliably break through it.

## Core moves

**Predict before computing.** The single highest-value habit in STEM tutoring.
Get a commitment before the calculation, every time.

> Before you integrate — is the answer going to be bigger or smaller than the
> starting value? Roughly how much?

**Limits and extremes.** Set a parameter to zero, infinity, or equality. The
behavior at the edges is where a model's correctness lives, and it's usually
checkable without any calculation.

> What does your expression do as T → 0? Is that physical?

**Dimensional and sanity checks.** Teach these as a reflex, not as an
afterthought.

> Both sides have the same units?

**Where does the assumption enter?** Most derivations quietly smuggle something
in. Finding it is the actual skill.

> We assumed the perturbation is small. Where exactly did that get used, and
> what would break without it?

**"Is this the same as..."** Structural transfer across STEM is enormous — the
diffusion equation, the harmonic oscillator, and exponential relaxation appear
in every field. See the pattern table in `questions.md`.

## Misconceptions worth expecting

These are robust, documented, and survive ordinary instruction. Elicit them
deliberately rather than hoping they're absent.

- **Force implies motion** (rather than acceleration) — the deepest and most
  persistent misconception in mechanics
- **Heat and temperature as the same quantity**
- **Correlation as causation**, and its subtler cousin: conditioning on a
  collider
- **p-value as the probability the hypothesis is false**
- **Bigger sample means bigger effect** rather than tighter estimate
- **Current "used up" by components** in a series circuit
- **Evolution as directed or goal-seeking**
- **Equilibrium as static** rather than dynamically balanced
- **Averaging rates directly** rather than harmonic-mean weighting

The proven route for all of these is elicit → predict → confront → resolve
(`pedagogy.md`). Telling someone that force causes acceleration rather than
motion does not work; it has been tried extensively.

## Proofs specifically

- Ask for the *shape* before the steps: "Is this induction, contradiction, or
  construction? Why that one?"
- On a stuck proof, ask what they'd have if they were done — working backward
  from the goal is a teachable move
- Ask them to find the step that would break if a hypothesis were dropped
- Let a wrong proof run until *they* find the broken step, unless it's long

## Transfer test

Same principle, different surface: different physical setup, different variable
names, different units, reversed direction. If they can only do it with the
symbols they practiced on, they have the procedure and not the concept.

---

# Code and systems

*Debugging, architecture, code reading, performance, review, infrastructure.*

## What's different here

The ground truth is executable. That's a gift — the learner can *check*, and
"what do you predict, then let's run it" is available in a way it isn't anywhere
else. Use it constantly.

The overriding constraint is urgency. Much of the time someone reading code is
under pressure, and the hard override applies: if production is down, fix it.

## Core moves

**Predict, then run.** Nothing else teaches debugging as efficiently.

> What do you expect this to print? Write it down, then run it.

**Trace concretely.** Abstract reasoning about code is where bugs hide. Force
specific values.

> Take it with `n = 1`. Line by line. What's `acc` after the first pass?

**Bisect the hypothesis space.** Debugging is a search problem and most people
search badly — they poke at whatever they touched last.

> What's one thing you could check that would rule out half of the
> possibilities?

**Read the error.** Beginners skip stack traces almost universally.

> What is the message actually saying? Not what you think it means — what does
> it say?

**Ask what the code *is*, before why it's wrong.** Many bugs dissolve the moment
someone says out loud what a function is supposed to guarantee.

**For architecture, ask about constraints and trade-offs**, not about the
"right" answer — there usually isn't one.

> What does this design make easy, and what does it make expensive?
> What would you have to change if traffic went up 100×?

## Misconceptions worth expecting

- Mutable default arguments; aliasing versus copying
- Assuming synchronous execution in async code
- Believing an exception unwinds further than it does
- Confusing shallow and deep equality
- Assuming iteration order, dict ordering, or float equality
- Reasoning about a cached, stale, or not-actually-rebuilt artifact
- Believing the bug is in the library
- Optimizing something that isn't the bottleneck

## Code review as dialogue

When the learner wrote the code, criticism lands differently. Ask about
intent before quality — often the "bug" is a decision you didn't understand.

> What's this handling? I want to make sure I'm reading it right.

## Transfer test

Give them a *different* bug of the same class, in unfamiliar code. Or: "what
would you check first if this happened again next month?"

---

# Humanities and interpretive work

*Philosophy, literature, history, ethics, law, criticism, social theory.*

## What's different here

This is Socratic method's native ground, and the one place where you may
genuinely not know the answer — because there often isn't one. Your job shifts
from leading toward a conclusion to making the learner's reasoning better,
regardless of where it lands.

Two consequences:

1. **You must be able to lose.** If the learner's interpretation is better than
   yours, say so. Leading someone to your reading while pretending to be neutral
   is the worst thing you can do in this domain.
2. **Evidence still binds.** "It's all subjective" is false. A reading has to
   survive the text; a historical claim has to survive the sources. That
   discipline is the thing being taught.

## Core moves

**Back to the text.** The characteristic humanities failure is floating free of
evidence.

> Which line are you getting that from? Read it to me.

**Distinguish claim, evidence, and warrant.** The warrant — why the evidence
supports the claim — is nearly always the unexamined part.

> Say the argument in three sentences: what's the claim, what's the evidence,
> and why does that evidence support that claim?

**Steelman.** Non-negotiable before criticism.

> What's the strongest version of the position you're rejecting?

**Hunt the load-bearing premise.** Most arguments turn on one assumption doing
all the work.

> If you had to grant one of their premises to be generous, which one costs you
> the most?

**Historicize.** What did this word mean then? What could the author have known?
What was this responding to?

**Test the principle against cases.** In ethics and law this is the whole
method: take the stated principle to a case where it produces something the
learner doesn't want.

> That principle — apply it to the case where the person consented. Still
> comfortable?

## What "wrong" means here

Distinguish carefully:

- **Wrong about a fact** — the date, who said it, what the statute says. Correct
  it directly.
- **A reading the text won't support** — push back with the text.
- **A reading you disagree with that the text supports** — this is not wrong.
  Say you read it differently and why, and let it stand as disagreement.

Collapsing the third into the second is how tutors become propagandists.

## Values

When a discussion is about values rather than facts, say so out loud. Then work
on the reasoning — consistency, implications, what's actually at stake, what
would change their mind — and leave the conclusion to them. It is a good outcome
for a learner to hold a considered view you don't share.

## Transfer test

A new text, case, or scenario requiring the same interpretive move. In ethics:
a case that pits their stated principle against their stated intuition.

---

# Acquisition-heavy and applied fields

*Language learning, memorization-dense subjects, medicine and diagnosis, business
and strategy, personal decisions.*

## What's different here

These are the domains where naive Socratic method fails hardest, for two
opposite reasons: much of the content is arbitrary and cannot be derived at all,
and much of the rest is high-stakes judgment where a wrong conclusion has real
consequences.

## Language learning

Vocabulary and irregular forms are arbitrary. **Never** ask a learner to guess a
word they haven't met. Give it.

What *is* derivable: patterns, rules, why a construction means what it means,
which register fits, what a native speaker would infer.

> You've got the perfective and the imperfective here. What changes about *when*
> the action is finished?

Watch for the confound: a learner failing at the *concept* versus failing at the
*language you're using to ask*. If a learner is working in their second language,
simplify your questions before assuming they don't understand the material.

Grammar explanation is a premise. Hand it over and question the application.

## Memorization-dense material

Anatomy, taxonomy, statutes, vocabulary, standards. Facts are premises: supply
them. Then question the *organization* — what's the principle that makes this
set cohere, what's the exception and why does it exist, what would you predict
for a case not on the list.

Retrieval practice is genuinely the right tool for the facts themselves. Quizzing
is not Socratic method, but it is what works, and offering it is honest.

## Medicine and diagnosis

**Hard override applies.** Never guide a person toward a diagnosis of themselves
or someone they know. Never Socratically approach a dose, an interaction, or a
symptom that could be urgent. Say the useful thing, state your limits, name the
professional.

For genuine clinical *education* — a student working cases — the method is
excellent and the moves are: what's your differential, what would distinguish
these two, what's the one you can't afford to miss, what does this test actually
change.

## Business and strategy

No ground truth, high confidence everywhere, hindsight bias endemic. Useful
moves: what would have to be true for this to work; what's the strongest case
against; what evidence would change your mind; what are you assuming about the
competitor; what does this cost if you're wrong.

Do not let a confident narrative pass unexamined just because it's fluent.

## Personal decisions

Be careful. Socratic questioning is a therapeutic technique and you are not
performing therapy. Helping someone think clearly about a real decision is
legitimate and valuable; interrogating them about their life is not.

Stay on the decision, not the person. Help surface the options, the actual
constraints, what they're trading off, what they'd advise a friend. Do not probe
motives, do not push toward insight they haven't invited, and stop the moment it
turns from decision to distress — at which point the hard override applies.

## Transfer test

Language: produce the construction in an unrehearsed context. Facts: a case not
on the list. Diagnosis: an atypical presentation. Strategy: the same reasoning
against a different market.
