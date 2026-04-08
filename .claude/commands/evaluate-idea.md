# Evaluate a Research Idea

Collaboratively evaluate, refine, and strengthen a research idea.

## Step 1: Get the Idea

Ask the user how they want to provide the idea:

> How would you like to provide the idea?
> 1. **Describe it** — tell me about it and we'll build it up together
> 2. **Paste it** — paste an existing idea description or file path

Accept whatever they provide. To evaluate thoroughly, you need:
- **Title**: Concise, descriptive
- **Research question**: What specific question does this address?
- **Approach**: High-level methodology
- **Why it matters**: Connection to AI safety

Fill in missing pieces conversationally. Every idea must be mapped to at least one AI safety research field before proceeding (e.g., Mechanistic Interpretability, AI Control, Adversarial Robustness, Alignment, Governance, Evaluations).

## Step 2: Score Against Criteria

Score the idea across 4 dimensions (1–5 scale):

**1. Theory of Impact** — How clearly does this connect to AI safety outcomes?
- 5: Direct causal path to reducing catastrophic risk, clearly articulated
- 4: Strong indirect connection, well-reasoned
- 3: Plausible connection but requires several intermediate steps
- 2: Weak or speculative connection
- 1: No clear connection to AI safety

**2. Accessible Complexity** — Can this be executed given realistic constraints?
- 5: Doable by a motivated student with standard resources
- 4: Requires some specialized knowledge but broadly accessible
- 3: Requires significant expertise or resources but feasible for a research team
- 2: Very difficult; requires frontier access or rare expertise
- 1: Currently infeasible

**3. Narrow Scope** — Is this focused enough to complete in the available time?
- 5: Crisp, well-defined scope; clear done condition
- 4: Clear scope with minor ambiguities
- 3: Scope needs further bounding
- 2: Too broad; would require significant narrowing
- 1: Ill-defined; no clear completion criteria

**4. Novelty** — Is this meaningfully different from existing work?
- Use WebSearch to check for related prior work before scoring
- 5: No direct prior work found
- 4: Related work in adjacent areas, but this specific angle is open
- 3: Prior work exists but this approach/combination is unexplored
- 2: Mostly covered; remaining gap is minor
- 1: Already solved — existing work fully addresses this

Present all scores with reasoning.

## Step 3: Collaborative Refinement

Enter a refinement loop. Ask what the user wants to work on:

> **What would you like to work on?**
> 1. **Discuss** — talk through any aspect of the idea
> 2. **Strengthen** — improve the weakest scoring dimensions
> 3. **Reframe** — explore 2-3 alternative angles on the core insight
> 4. **Sharpen approach** — make the methodology more concrete
> 5. **Check novelty** — search the literature for related work
> 6. **Save** — write the idea to a file
> 7. **Done** — end session
>
> Or just tell me what's on your mind.

### If discuss:
Engage with whatever the user wants to explore — feasibility, framing, scope, related work, comparisons. Follow their lead.

### If strengthen:
Identify the lowest-scoring dimensions. For each: explain why the score was low, suggest specific concrete improvements, rewrite the relevant sections, re-score.

### If reframe:
Generate 2-3 alternative framings of the core insight, each taking a different methodological or conceptual angle. Include estimated scores for each so the user can compare tradeoffs.

### If sharpen approach:
Make the methodology concrete: specific tools, datasets, and models; key assumptions; minimum viable experiment; what success looks like.

### If check novelty:
Run a literature search using WebSearch:
- Search for the underlying problem (method-agnostic) first
- Then search for the specific approach proposed
- Check arXiv, Semantic Scholar, Alignment Forum, and LessWrong
- Report what was found and update the Novelty score accordingly

### If save:
Write the idea as a markdown file. Include: title, research field(s), research question, approach outline, scores and reasoning, theory of impact, proposed first experiments (if discussed), and relevant prior work found.

Return to the refinement menu until the user chooses "Done".

## Session Summary

When done:
- Summary of changes made to the idea
- Final scores
- Whether the idea was saved
- Suggested next steps (e.g., `/novelty-check`, `/research-topic`)
