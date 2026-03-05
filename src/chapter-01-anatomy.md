# Chapter 1: The Anatomy of a Good Question

Not all questions are worth asking.

This statement bothers some people, who have been told since childhood that there are no stupid questions. There are. Plenty. The question "have we considered all the alternatives?" asked after a three-month implementation is largely rhetorical. The question "why does this always happen to me?" contains no path to an answer. The question "did we check the logs?" when you already know the answer is a performance of diligence, not an inquiry.

The uncomfortable truth is that questions have quality, and most people have never been taught to evaluate it.

Let's fix that.

---

## What a Question Is Actually Doing

Before examining properties, it helps to be precise about function. A question does one or more of the following:

1. **Requests information** — fills a gap in what you know
2. **Challenges an assumption** — tests a belief you or someone else is holding
3. **Opens a search space** — identifies a domain worth exploring
4. **Forces a decision** — makes an implicit choice explicit

Dead-end questions usually fail on all four dimensions. "Does everyone agree?" does not genuinely request information (people rarely disagree in meetings). It does not challenge an assumption. It does not open a search space. It does not force a real decision. It is a ritual utterance that happens to have a question mark attached.

Generative questions tend to score on multiple dimensions simultaneously. "What would have to be true for this plan to fail within 90 days?" requests real information (failure modes), challenges the assumption (that the plan is sound), opens a search space (the space of possible failures), and forces a decision (whether to act on the failure modes you identify).

Same grammatical structure. Radically different function.

---

## Five Properties of Questions Worth Asking

### 1. Specificity

Vague questions produce vague answers, which produce vague actions, which produce vague results. Specificity is not pedantry — it is the mechanism by which a question can be answered at all.

Compare:
- "Why isn't this working?" (vague)
- "Under what conditions does this fail that don't apply when it succeeds?" (specific)

The second forces you to think about the structure of the problem before you can even begin answering. That pre-answer thinking is frequently where the insight lives.

Specificity also constrains the answer space usefully. A specific question is a hypothesis in disguise. It implies a structure of what an answer would look like, which makes it possible to recognize an answer when you find one.

### 2. Falsifiability

A question is falsifiable if it is possible to get an answer that proves it wrong. "How can we improve this?" is not falsifiable — no answer could establish that improvement is impossible. "Is there a configuration of this system that performs better on benchmark X?" is falsifiable — you run the benchmark and find out.

Falsifiability matters for two reasons. First, it means the question is answerable in principle, not just in theory. Second, it provides protection against motivated reasoning. If you cannot specify in advance what a wrong answer looks like, you will interpret all evidence as confirming your preferred conclusion.

This applies to questions in strategy, not just in science. "How do we know if this initiative is working?" is a version of falsifiability. Ask it before you start, not after the results come in.

### 3. Generativity

Some questions, once asked, produce more questions. These are generative. They open territory rather than closing it.

The question "why do people abandon shopping carts online?" is generative. Attempts to answer it produce follow-on questions about intent, timing, friction, alternatives, and context — each of which is worth exploring. The question "how do we reduce cart abandonment?" is less generative because it pre-supposes that reduction is the right goal and that the mechanism is intervention on abandonment rather than, say, changing what you define as abandonment.

Generativity is a property to seek in early-stage inquiry and to limit in late-stage execution. When you are trying to understand a problem, generative questions are how you avoid premature closure. When you need to ship something, you need questions that converge.

Knowing which mode you are in is itself worth a question.

### 4. Assumption Exposure

Good questions reveal what you are assuming without knowing it.

"Should we build feature X?" contains assumptions: that the product should grow, that X is the right increment, that building is the appropriate response to the underlying need, that you have correctly identified the need. Most of these assumptions are invisible until you ask a question that surfaces them.

"What problem does feature X solve, and how do we know users have that problem?" exposes the assumptions directly. If you can't answer it, you have learned something important before spending engineering time.

Assumption-exposing questions are uncomfortable, which is why they're underused. They imply that you haven't done the thinking you claimed to have done. In practice, asking them is evidence of good thinking, not its absence.

### 5. Scope Fit

A question that is too broad produces analysis paralysis. A question that is too narrow misses the point.

"What should we do about climate change?" is too broad to be actionable. "Should we switch our CI pipeline from GCP to AWS?" may be too narrow if it avoids the question of whether the CI pipeline is the right bottleneck to address at all.

Scope fit is relative to your position. A company-level strategy question and a team-level implementation question have different appropriate scopes. The error is usually scope mismatch: asking implementation-level questions when you should be asking strategy-level ones, or drowning in strategy when you need to make a concrete decision.

The right scope for a question is one where an answer would change what you do next.

---

## Diagnosing Your Own Questions

Here is a simple test to apply to questions before you ask them:

1. **Can this be answered?** If you cannot describe what an answer would look like, the question is probably not specific enough.
2. **Would a wrong answer surprise me?** If no, the question may be unfalsifiable.
3. **Does it expose an assumption?** If you answer it without challenging anything you believe, it probably didn't need asking.
4. **Who needs to hear the answer?** If nobody's behavior would change based on the answer, the question is probably not worth the conversation.

This is not a filter to apply mechanically before every question you ask. It is a diagnostic tool for the moments when you notice you are asking questions but not making progress.

The feeling of asking lots of questions while getting no traction is a reliable sign that your questions have a quality problem. The fix is not to ask fewer questions — it is to ask better ones.

---

## The Question Behind the Question

One more property worth naming: recursion.

Often the most useful question is the one behind the question you started with. You ask "why is the deployment slow?" and the question behind it is "are we measuring the right thing?" You ask "should we hire another engineer?" and the question behind it is "is headcount the constraint, or is it something else?"

The question-behind-the-question is usually more generative than the original, often exposes more assumptions, and is almost always more uncomfortable to raise. This is not a coincidence.

A useful discipline is to take whatever question you were about to ask and ask "what is that question really about?" at least once before raising it. You will not always find a better question. But when you do, the improvement is usually significant.

---

In the next chapter, we get into the harder problem: not what makes a question good, but how to find the questions that nobody has thought to ask at all.
