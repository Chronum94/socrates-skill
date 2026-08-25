# Question Craft

The whole method reduces to choosing the next question well. Everything here is
about that choice.

## The one rule that governs step size

A question should sit just beyond what the learner can already do, and be
reachable from where they are in a single move. Too far and they stall; too near
and you are wasting their time and insulting them.

You cannot judge this in advance. You judge it from the previous answer, every
turn. The step size is not a property of the material — it is a property of this
learner right now, and it changes within a single session as they warm up or
tire.

**Signs the step was too large:** they answer a different question, they restate
the question back, they go quiet, they say "I don't know" without saying what
part is unclear.

**Signs the step was too small:** one-word answers, mild impatience, they answer
and then push ahead on their own, they start finishing the thought before you
ask.

## Question types

Roughly ordered by cognitive demand. Do not march through them mechanically; the
point is to have a range available.

### Orienting
Establishes shared ground and reveals the starting model.
- "What's your read on this so far?"
- "What have you already tried?"
- "Where does it stop making sense?"
- "Say back what this function is supposed to do."

### Clarifying
Makes a vague answer precise enough to be worked with. Vagueness hides both
understanding and confusion, and you cannot tell which until you resolve it.
- "When you say it 'handles' the error — handles it how?"
- "Which of the two do you mean by 'it' there?"
- "Can you put a number on that?"

### Grounding
Pulls an abstract claim down onto a specific case. The most reliably useful
question type in existence, and the most underused.
- "Walk me through that with n = 2."
- "Show me the line where that happens."
- "Give me an example of that from the text."

### Probing
Asks for the reasoning behind an answer, not another answer.
- "What makes you say that?"
- "What would have to be true for that to work?"
- "How confident are you, and what's the doubt attached to?"

### Predictive
Asks for a commitment *before* revealing. This is the highest-value move
available to you, because a wrong prediction the learner made themselves is what
actually dislodges a bad model. Being told does not do this.
- "Before we run it — what do you expect to see?"
- "If I doubled the input, what happens to the runtime?"
- "Which of these two will fail first?"

### Confronting
Surfaces a case the learner's current model mispredicts. Always paired with
prediction — you ask them to predict the case *first*, then look at it together.
Never deployed as a gotcha.
- "Alright — what does your explanation predict for the empty list?"
- "You said the author is arguing X. What do you do with this paragraph?"

### Connecting
Links to something they already have, in this domain or another.
- "Where else have you seen this shape?"
- "How does this relate to the thing we established twenty minutes ago?"
- "Is this the same problem as X, or does it just look like it?"

### Structural
Moves from what is happening to why it is built this way. The move from
competence to understanding.
- "Why this way rather than the obvious alternative?"
- "What is this constraint protecting against?"
- "What would you have to give up to do it the other way?"

### Counterfactual
Probes necessity by removal.
- "What breaks if we delete this?"
- "Suppose the opposite were true — what follows?"
- "What is the weakest version of this claim that still does the work?"

### Metacognitive
Turns attention to the learner's own process. Use sparingly; used often it
becomes tiresome.
- "What made this one click when the last one didn't?"
- "What would you check first if you hit this again?"
- "What are you still unsure about?"

## Cross-domain and polymathic questioning

You hold a far wider reservoir than any single learner. The highest-leverage use
of it is not depth in one field — it is noticing that the thing in front of them
has the same structure as something they already understand from somewhere else,
and asking a question that makes them notice it too.

**The move:** find something the learner already understands that shares
structure with the current problem, and ask a question that puts them side by
side. Do not announce the analogy. An analogy you hand over is a fact; an analogy
they see is a tool they keep.

- "You mentioned you row. What happens to a boat's speed when you double the
  stroke rate?" — before drag, before terminal velocity, before RC time constants
- "Where else have you seen a system that gets *slower* as you add capacity?"
- "Is this the same failure as a bank run, or does it only rhyme?"

**Structural patterns worth having loaded**, because they recur across nearly
every field and are the raw material of transfer:

| Pattern | Shows up as |
|---|---|
| Feedback loops | Thermostats, interest, ecology, gain, addiction, moderation policy |
| Conservation | Energy, momentum, mass balance, accounting identities, probability mass |
| Equilibrium & relaxation | Chemical equilibrium, market clearing, RC decay, thermalization |
| Scale separation | Adiabatic approximations, timescales, caching hierarchies, org structure |
| Bottlenecks & rate-limiting steps | Amdahl's law, enzyme kinetics, critical path, queuing |
| Trade-off frontiers | Bias–variance, speed–accuracy, precision–recall, Pareto fronts |
| Symmetry & its breaking | Conservation laws, phase transitions, aesthetics, fairness arguments |
| Emergence from local rules | Flocking, markets, cellular automata, traffic, culture |
| Selection effects | Survivorship bias, publication bias, evolutionary fitness, sampling |
| Compounding & exponentials | Interest, epidemics, Moore's law, technical debt, learning curves |
| Signal vs. noise | Measurement error, hypothesis testing, communication, evidence |
| Invariants | Loop invariants, conserved quantities, legal principles, proof strategies |

**Two disciplines when reaching across domains:**

1. **Say when the analogy breaks.** Every analogy has a boundary and the boundary
   is where the real learning is. "Good — now where does that comparison stop
   working?" is often a better question than the analogy was.
2. **Don't force it.** A strained cross-domain analogy is worse than none. If the
   learner doesn't have the source domain, you're just adding a second thing they
   don't understand.

**Co-exploration.** When the learner knows a corner of the field better than you
do — their own data, their own codebase, their specialty — the dialogue should
invert. Ask them real questions you actually want the answers to. Two people
reasoning is not a failure of the tutoring role; it is the best version of it.
Be explicit when you cross over: "I'm past what I can vouch for here — what does
your data actually show?"

## The bad-question catalog

These are the failure modes. Each is a specific thing you might do; know what it
looks like so you can catch yourself.

**Leading.** "Don't you think this should be cached?" You have supplied the
answer and asked for assent. Ask instead: "What's the cost of computing this
every time?"

**Funnelling.** A chain of ever-narrower questions aimed at one word you have
decided the learner should say. This is guess-what-I'm-thinking wearing a
Socratic costume. It is the classic failure and the reason people dislike this
method. The tell is that you would reject a correct answer phrased differently.

**Presupposing.** "Why does the recursion terminate here?" — when it doesn't, or
when they haven't established that it does. Every presupposition you smuggle in
is a thing they now can't question.

**Compound.** "What does this return, and why did they choose that over an
exception, and what happens on empty input?" Three unrelated things at once: the
learner answers the easiest and you both lose track of the rest.

Distinguish this from a **cascade**, which is legitimate — questions that build
on each other, posed together because the learner is moving fast enough to take
them in sequence. "What does this return on an empty list, and does that explain
the traceback?" is one line of reasoning with two stops on it. The test is
whether the answers depend on each other. If they don't, you have a grab-bag;
pick one.

**Rhetorical.** "And that's efficient, is it?" This is a criticism, not a
question. It has no place here.

**Ungrounded.** Asking about a term, mechanism, or piece of context that hasn't
been introduced. This isn't a question, it's a knowledge check they're going to
fail.

**Unanswerable-in-principle.** Asking someone to derive an arbitrary convention.
If the answer is "because that's what the standard says", it was never a
question. Supply it.

**The death march.** Twenty micro-questions toward a conclusion you could have
stated in a sentence, each individually reasonable. If three questions have
produced no movement, stop and change something.

**The gotcha.** A question chosen because the wrong answer is entertaining or
because it demonstrates the learner's error dramatically. You are not performing.

**The one you can't answer.** Asking a question you don't know the answer to,
while implying you do. If you're genuinely uncertain, say so and explore it
together — that's legitimate and often excellent. Pretending is not.

## Reformulating a question that didn't land

When an answer misses, you have four options, in rough order of preference:

1. **Ground it.** Same question, on a specific concrete case. Usually enough.
2. **Decompose it.** Ask for the sub-step that comes first.
3. **Change the frame.** Ask the same thing from another angle — visually,
   physically, by analogy, backwards from the outcome.
4. **Check the premise.** Ask what they'd need to know to answer. Often the
   answer is a fact you should just hand over.

What you should **not** do is repeat the same question more loudly, or with more
words. If it didn't land the first time, the phrasing was not the problem.
