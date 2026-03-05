# Chapter 2: Finding Questions Worth Asking

The previous chapter described what makes a question good. This chapter addresses the harder problem: how do you find the questions that nobody has asked yet?

It is harder because it requires working in the dark. You cannot evaluate a question you haven't formed. The techniques here are about generating candidates — questions that might be worth asking — before applying quality criteria. The goal is to enter the space of unexplored questions and come out with something you didn't have before.

---

## Why the Best Questions Are Hard to Find

The questions worth asking are, by definition, not obvious. If they were obvious, someone would have asked them. The fact that they haven't been asked is usually evidence of one of three things:

1. **They challenge a shared assumption** — everyone in a domain holds the same belief, so the question of whether that belief is correct doesn't arise naturally.

2. **They cross boundaries nobody crosses** — they require combining knowledge from two fields, or asking about the interaction between two systems that are usually managed separately.

3. **They're uncomfortable** — they have implications that people would rather not examine.

The first two produce the most valuable questions. The third is more situational but worth noting.

Knowing this helps orient the search. You are not looking for questions that feel natural, that fit neatly within the current frame, or that everyone in the room will immediately appreciate. You are looking for the off-center ones.

---

## Technique 1: Assumption Audit

Every domain of knowledge rests on a foundation of beliefs that practitioners have mostly stopped questioning. These are not secrets — they are simply so widely held that questioning them doesn't occur to anyone.

An assumption audit works by making these beliefs explicit and then asking: *what if this is wrong?*

Start with the core belief of whatever you're examining. For a product: "users want more features." For a hiring process: "the interview is a good predictor of job performance." For a technical architecture: "horizontal scaling is the right response to growth."

Write the belief down. Then ask:
- Under what conditions would this be false?
- Has anyone checked whether this is true?
- What would we do differently if it were false?

The uncomfortable version of this exercise is to apply it to your own work. "What does our current approach assume that might not be true?" is a question that produces useful answers and is rarely asked by the people best positioned to act on it.

The productive version is to apply it systematically. Go through the decisions your team made in the last quarter and state the assumptions they relied on. Then run the falsifiability test from Chapter 1. Most will survive. Some won't. The ones that don't are where the interesting questions live.

### Where Assumptions Cluster

Assumptions tend to accumulate in the same places:

**Definitions.** The way you define the problem determines which solutions look viable and which look irrelevant. "Customer churn" defined as subscription cancellations produces different questions than "customer churn" defined as declining engagement. The definition is an assumption, and it is almost never examined.

**Constraints.** "We can't do X because Y" often encodes a constraint that was true at some earlier time and has since changed — or was never true to begin with. "We can't do real-time processing because the latency is too high" may have been accurate three years ago and be demonstrably false now.

**Success criteria.** "This is working" conceals the question: working by what measure? The implicit success metric is usually inherited from whoever last designed the evaluation. It is rarely the right metric, because the right metric is specific to current conditions and current goals, which change.

---

## Technique 2: Perspective Rotation

Any problem looks different depending on who is looking at it. The technique here is to deliberately adopt a perspective that is not yours and ask what questions would be obvious from that vantage point.

This is not "empathy" in the workshop-activity sense. It is a structured inquiry technique.

**The outsider perspective.** Someone encountering your domain for the first time, without your priors, will ask different questions. What would a competent person from a completely different field find obviously strange about the way you operate? What would a new hire, before they've been trained out of their naivety, notice and wonder about?

The outsider perspective is difficult to manufacture once you're deep in a domain, which is why organizations that import talent from adjacent fields frequently get innovations that insiders had the same information to make and didn't.

**The critic perspective.** If someone were trying to show that your approach is wrong, what questions would they ask? This is not the same as steelmanning a counterargument — it is asking: where are the soft spots? The critic's first move is always to question the premise, which is why it is a useful perspective to adopt before a critic does.

**The successor's perspective.** Imagine someone five years from now looking back at the decision you're making. What would they find obviously misguided? What questions would they wish had been asked? The successor's perspective is particularly useful for avoiding the errors of the current moment — the assumptions that will be obviously wrong in retrospect and are invisible to everyone now.

**The user's perspective.** Not the idealized user from your persona document, but an actual person using the thing you built, in the conditions they actually experience. What would they ask about your product that you have never asked? The distance between the questions your users have and the questions you have been asking is usually very large.

---

## Technique 3: Boundary Examination

The most generative questions often live at boundaries: between disciplines, between teams, between phases of a process, between the system you're building and the environment it operates in.

Boundary questions are underasked because the boundary itself is usually invisible. It is the place where one team's responsibility ends and another's begins — which means neither team is asking about what happens at the handoff. It is the place where two fields of knowledge could be combined — which means the people who know field A don't know field B, and vice versa.

To examine boundaries systematically:

1. Identify the handoffs in your process. Where does work pass from one person or team to another? Where does your system interface with another system? Where does your product meet the user's environment?

2. Ask what is assumed at each handoff. What does the receiver assume the sender has guaranteed? What does the sender assume the receiver knows? What falls between the two?

3. Ask what questions exist at the boundary that neither side is asking. These are usually about the interaction between the two systems, not about either system in isolation.

**Cross-disciplinary boundaries** are particularly productive. The question "what does machine learning have to say about this economics problem?" or "what would an operations researcher do with this design problem?" often produces original questions because the transfer of methods across domains is genuinely novel.

---

## Technique 4: Working Backward from the Conclusion

If you know where you want to end up — or where the conventional wisdom says you'll end up — you can find good questions by working backward from that conclusion and asking what would have to be true for it to hold.

This is the mechanism behind pre-mortems, scenario planning, and a number of other structured foresight techniques. It works because it reverses the natural direction of reasoning. Instead of working forward from current conditions toward a future state, you posit a future state and ask what must be true in the present for the path to exist.

Working backward surfaces hidden dependencies, implicit assumptions, and necessary conditions that forward reasoning tends to skip over.

Applied to questions: if the answer everyone expects is X, ask "what would have to be true for the answer to be not-X?" The answers to that question are usually the productive questions. If none of the conditions for not-X can be ruled out, you have found a reason to question X.

---

## Technique 5: The Question You Won't Ask

The most reliable indicator of an important question is that you don't want to ask it.

Avoidance is informative. When you notice that a question is hovering at the edge of a conversation and nobody is raising it, or when you find yourself working hard to frame something in a way that doesn't raise a particular issue, that is a signal. The question being avoided is usually more important than the ones being asked.

This applies to both individual and group dynamics. In a one-on-one, the questions you walk away from a conversation not having asked are often the ones that would have changed something. In a team, the silence after a proposal is sometimes the sound of everyone not asking the same question.

The technique is straightforward: at the end of any significant inquiry or meeting, ask explicitly — "What question didn't we ask?" or "What question are we avoiding?" The discomfort with doing this is proportional to the value of what you'll find.

---

## Combining the Techniques

None of these techniques work mechanically. They are prompts for a mode of thinking, not algorithms. The value is in developing the habit of looking for questions, not in executing any particular method.

What they share: they all redirect attention from *what is* to *what is assumed*, from *the current frame* to *adjacent frames*, from *what has been asked* to *what hasn't been*.

The disposition they cultivate is a productive dissatisfaction with the existing question set. Most people treat the questions on the table as given. The rarer skill is treating them as a draft — a starting point to be refined and extended rather than a fixed agenda to be worked through.

---

Knowing the techniques for finding good questions is necessary but not sufficient. There is a prior problem: most of those techniques will fail in real organizational settings because of the forces arrayed against good questioning. That's Chapter 3.
