# Pedagogy

Why the rules in `SKILL.md` are what they are, and when the method is the wrong
tool.

> Apply this file's own doctrine to itself: the frameworks and findings below
> are real and well established, but specific effect sizes and dates are exactly
> the kind of detail worth checking (`epistemics.md`). Cite them to a learner as
> "there's a well-known result that..." rather than as precise figures you'd
> stake something on.

## The honest case against pure Socratic method

Start here, because it is the part most versions of this skill omit.

**Unguided discovery learning is empirically weak for novices.** This is not a
minor caveat; it is one of the better-supported findings in instructional
psychology. Kirschner, Sweller and Clark's "Why Minimal Guidance During
Instruction Does Not Work" (*Educational Psychologist*, 2006) assembles decades
of evidence that learners without sufficient prior knowledge learn more from
direct instruction and worked examples than from being asked to discover
principles themselves.

The mechanism is cognitive load. A novice searching a problem space spends
working memory on the search rather than on the structure worth learning.
Sweller's **worked example effect** shows novices learn more from studying a
worked solution than from solving an equivalent problem.

Two corollaries that should change your behavior:

- **Expertise reversal effect** (Kalyuga et al.): the guidance that helps a
  novice actively *harms* an expert, who is slowed by being walked through what
  they already know. This is the formal statement of why Socratic treatment of
  an expert stuck on one detail is a mistake.
- **Guidance fading effect** (Renkl & Atkinson): the right trajectory is worked
  example → partially worked → independent problem. Support should be withdrawn
  progressively, not withheld from the start.

**What this means here.** The assistance ladder in `SKILL.md` is fading
implemented backward: start with questions, and drop to worked examples when the
learner lacks the prior knowledge to make questioning productive. Rung 6 — full
explanation followed by immediate re-derivation — is not the method failing. For
a genuine novice it is the method working correctly.

The premise/conclusion distinction is the same principle in another form.
Premises are cognitive load with no learning value; hand them over and spend the
learner's working memory on the reasoning that's actually worth building.

## When Socratic method is the wrong tool

- **The learner has no relevant prior knowledge.** Nothing to build from. Teach
  first, question after.
- **The content is arbitrary.** Conventions, vocabulary, dates, names, syntax.
  Cannot be derived; retrieval practice is the correct tool.
- **The learner is an expert stuck on a detail.** Expertise reversal. Answer.
- **Time pressure.** Urgency and pedagogy conflict; urgency wins.
- **Stakes are high and immediate.** Safety, medical, legal, destructive
  operations. State the truth.
- **The learner has declined it.** Consent is not optional.
- **You don't know the answer and the answer matters.** Say so; investigate
  together rather than performing tuition.

## Frameworks that shape the rules

### Zone of proximal development (Vygotsky, 1978)

Learning happens in the band between what someone can do alone and what they can
do with help. Questions must land inside that band. Above it they stall; below it
you waste their time. The band is a property of the learner at this moment, not
of the material — which is why step size must be re-judged every turn.

**Scaffolding** (Wood, Bruner & Ross, 1976) is the support that makes the band
reachable, with the explicit requirement that it be *removed* as competence
grows. Scaffolding that is never withdrawn is just dependence.

### Conceptual change (Posner, Strike, Hewson & Gertzog, 1982)

People do not acquire correct models by being told; they hold intact prior models
that must be *displaced*. The conditions for displacement: the learner must
become dissatisfied with their existing conception, and the new one must be
intelligible, plausible, and fruitful.

This gives the **elicit → predict → confront → resolve** cycle:

1. **Elicit** — get the learner's actual model stated explicitly
2. **Predict** — have them commit to what it implies for a specific case
3. **Confront** — examine the case; let the misprediction be theirs
4. **Resolve** — build the corrected model, and check it against the same case

Dissatisfaction is the load-bearing step and it cannot be delivered by
assertion. A learner told they are wrong updates their answer; a learner
surprised by their own prediction updates their model. This is the entire reason
`SKILL.md` forbids correcting by assertion.

The persistence of misconceptions is well documented — the Force Concept
Inventory (Hestenes, Wells & Swackhamer, 1992) famously showed that traditional
physics instruction leaves the force-implies-motion misconception largely
intact, which motivated much of modern physics education research.

**But:** if confrontation fails twice, tell them. An unresolved contradiction the
learner cannot resolve produces confusion and discouragement, not conceptual
change.

### Self-explanation and active engagement (Chi)

Learners who explain material to themselves while studying learn substantially
more than those who don't — the **self-explanation effect** (Chi et al.). Chi &
Wylie's later **ICAP framework** orders engagement as Interactive > Constructive
> Active > Passive: dialogue that makes the learner *generate* beats dialogue
that makes them select, which beats attentive listening.

This is the mechanism behind the whole approach. It is also why "question +
multiple choice options" is a genuine step down: recognition is weaker than
generation, which is why `SKILL.md` reserves it for learners who are stuck.

### Desirable difficulties (Bjork)

Conditions that slow acquisition and *feel* worse often improve retention and
transfer: retrieval practice over re-reading (Roediger & Karpicke), spacing over
massing (Cepeda et al.), interleaving over blocking (Rohrer & Taylor),
generation over presentation.

The corollary that matters most in practice: **learners systematically
mis-evaluate what is working.** Deslauriers et al. (*PNAS*, 2019) found students
in active-learning classrooms learned more while reporting that they had learned
less, because fluency feels like understanding and effort feels like failure.

So: expect a learner to feel worse about a session that taught them more, take
"this feels inefficient" as weak evidence about efficiency, and never accept
felt understanding as evidence (`assessment.md`).

### Bloom's taxonomy (1956; Anderson & Krathwohl, 2001)

Remember → Understand → Apply → Analyze → Evaluate → Create. Useful as a check
on whether your questions are climbing. If forty minutes of dialogue has stayed
at Remember and Understand, you are quizzing, not tutoring.

Bloom's separate **"2 sigma problem"** (1984) — that one-to-one tutoring
produced dramatically larger gains than classroom instruction — is the reason
tutoring is interesting at all, though later work (VanLehn, 2011) put realistic
human-tutoring effect sizes well below two standard deviations, and found
well-designed automated tutoring roughly comparable to human tutoring.

### Metacognition and calibration

Learners are poor judges of their own knowledge, and confidence is a weak signal
in both directions. This justifies asking for confidence alongside answers, and
treating confident-and-wrong as a distinct diagnostic state from hedged-and-wrong
(`assessment.md`).

## The Meno problem

In Plato's *Meno*, Socrates elicits a geometric proof from an untutored slave
boy, arguing this shows knowledge is recollection. Read the dialogue with an eye
on the questions and the argument collapses: Socrates supplies the construction,
the framing, and every consequential step. The boy mostly assents.

This is the founding instance of the method's characteristic failure —
**funnelling**, where a chain of leading questions produces the appearance of
discovery while the tutor does the work. It is worth knowing because the failure
is seductive: the dialogue feels wonderful from the tutor's side, and the learner
ends up with nothing.

The diagnostic: **would you have accepted a correct answer phrased differently?**
If not, you were funnelling. A real question has a space of acceptable answers.

## Expert blind spot

Experts are systematically bad at estimating what is hard for novices, because
their own knowledge is compiled and automatic — the steps they skip are
invisible to them. This is why your step size will tend to be too *large*, why
"I don't know" so often means a premise is missing rather than reasoning
failing, and why the diagnosis in `SKILL.md` is "if three questions produced no
movement, the problem is your questions."

## The short version

- Give premises, withhold conclusions — cognitive load theory
- Question inside the ZPD, re-judge every turn — Vygotsky
- Elicit and confront rather than assert — conceptual change
- Make them generate, not select — ICAP
- Descend to worked examples when prior knowledge is absent — guidance fading
- Don't tutor an expert through what they know — expertise reversal
- Never accept felt understanding as evidence — desirable difficulties
- Would another phrasing have been accepted? — the Meno test
