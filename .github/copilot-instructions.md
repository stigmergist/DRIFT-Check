# DRIFT LLM Wiki Operating Schema (Copilot)

This workspace uses a persistent wiki pattern inspired by Karpathy's LLM Wiki idea.

## Mission

Build and maintain a living knowledge wiki in `wiki/` from immutable raw sources. The wiki is not a summary layer and not a schema dump. It is a place where ideas are understood: where a reader can come to genuinely grasp what a concept means, why it matters, and how it connects to the rest of the thinking.

Every page should read like a wiki article written by someone who actually understands the idea. Each concept gets its own page. Pages should be as long as they need to be and no longer. Structure should serve the idea, not constrain it.

Raw sources are source-of-truth and must not be modified.

## What This Wiki Documents

DRIFT is a **tool**, not a decision framework. The distinction matters. DRIFT provides concepts and decision patterns that can be applied **alongside** existing frameworks, methods, and governance structures. It helps structure judgement in messy conditions, but it does not prescribe decision rights, authority, or process. Pages should make this distinction clear: DRIFT extends and clarifies thinking, it does not replace domain expertise, governance, or accountability.

## Directory Contract

- Raw sources (immutable): `README.md`, `DRIFT_PRINCIPLES.md`, `DRIFT_CHECK_THINKING.md`, `METHOD_COMPARISON.md`, all `docs/*`, all `background/*`
- Maintained wiki (LLM-writable): all files under `wiki/`
- Control files in `wiki/`: `index.md` (catalog), `log.md` (append-only timeline), `sources.md` (source registry)

## Session Start Routine (required)

Before making wiki edits:
1. Read `wiki/index.md`.
2. Read latest entries in `wiki/log.md`.
3. Read `wiki/sources.md` and identify pending or stale sources.
4. Confirm operation intent.

## Ingest

When asked to ingest source(s):

1. Read the source file(s) fully.
2. Before writing anything, identify the atomic ideas in the source: the smallest meaningful concepts that could stand alone and be referenced from elsewhere.
3. Give each atomic idea its own page. Do not bundle unrelated ideas together just because they appeared in the same source.
4. Write each page as a genuine explanation of that idea. Lead with what it actually means in plain language. Then explain why it matters, what it implies, how it goes wrong, and how it connects to other ideas. Let the structure emerge from what the idea needs.
5. Link pages to each other where the relationship is real and meaningful. If page A depends on page B, both should usually link to each other.
6. Note tensions and contradictions. Do not flatten disagreement.
7. Update control files: `wiki/index.md`, `wiki/sources.md`, `wiki/_concepts_vocabulary.md` (add any new concept pages), and append to `wiki/log.md`.

### What good pages look like

Good pages are written for someone who wants to understand, not someone who wants to look up a definition. They:

- Open with a direct explanation of what the idea is, in plain English.
- Say why it matters: what breaks when you ignore it, what becomes possible when you have it.
- Explain the subtleties and common mistakes.
- Connect outward to related ideas by name and link.
- Use headers only where a section break genuinely helps, not to fill a template.
- Are as short or as long as the idea requires.

There is no prescribed template. A short concept might need only a few paragraphs. A complex concept with multiple failure modes might need several sections. Follow the idea, not the form.

### Granularity

Prefer many small focused pages over fewer large ones. Each concept, signal type, failure mode, or relationship worth understanding should have its own page. If two ideas are genuinely inseparable, a combined page is fine, but the default is to split.

Examples: `capability.md`, `capability_stack.md`, `value.md`, `progress.md`, `misfit.md`, `observation.md`, `context.md`, `stabilise.md`, `rationalise.md`, `optimise.md`, `alignment.md`, `uncertainty.md`, `fragility.md`, `absorption_capacity.md`, `programme.md`, `reversibility.md`, `agency.md`, `scaling.md`, `judgement.md`, `innovation.md`.

### Writing style

- Write in clear, direct, readable prose.
- Avoid bullet walls. Use short paragraphs.
- Bold key terms only where emphasis genuinely helps.
- Avoid the words "robust", "leverage", and "utilise".
- Do not pad. If there is nothing more to say, stop.

### Cross-linking and concept highlighting (required)

Every page should identify and link to related DRIFT concepts. This creates a dense knowledge graph that helps readers navigate between ideas and makes the wiki discoverable from multiple entry points.

**The canonical key concepts vocabulary is maintained in [`wiki/_concepts_vocabulary.md`](_concepts_vocabulary.md).** This file is updated as new concept pages are created during ingest. When writing or editing pages:

1. **Link key concepts on first mention.** Consult `wiki/_concepts_vocabulary.md` to identify which concept pages exist, then link to them when mentioned.
2. **Bold canonical concepts at first mention in a new context.** Example: "This is why **misfit** emerges—applying the wrong action to the current state."
3. **In 'See also' sections, link every genuinely related concept.** Aim for 4–8 links per page; verify each link by consulting `wiki/_concepts_vocabulary.md`.
4. **Update `wiki/_concepts_vocabulary.md` when creating new concept pages.** Add the concept name, category, and one-line description.

The vocabulary file doubles as a browseable index; readers can visit it to explore the concept landscape.

### Accessibility for decision-makers (required)

Pages must be readable and useful for board members, executives, senior technologists, and product leaders. This means:
- **Lead with observable problems, not concepts.** Example: "When the same team action produces different results week to week, reliability is weak and optimization will amplify the chaos" instead of "variability signals capability is not yet stable".
- **Show what to look for in real situations.** "Decisions are repeatedly reopened", "teams interpret strategy differently in execution", "incidents keep recurring", not abstract definitions.
- **Clarify what this tool is, not what it isn't.** DRIFT is a tool that works alongside existing frameworks and governance; it clarifies thinking, not an alternative to domain expertise or accountability. Don't defend it; describe the real problems it helps see more clearly.
- **Make everything concrete.** "Is the team producing consistent outcomes, or does success depend on who's leading?" beats "observation reveals capability state".
- **Name real use cases.** "When metrics improve but nothing actually changes" or "When board alignment sounds complete but execution fragments" tells readers immediately whether they need this.

### Plain-language guardrail (required)

Write for a busy decision-maker reading quickly.

- Keep most sentences between 8 and 18 words.
- Avoid sentences longer than 24 words unless needed for precision.
- Prefer concrete verbs: test, check, stop, change, decide, compare.
- Avoid dense abstract phrasing where possible.
- If a dense sentence is necessary, follow it with a plain rewrite that states what to do next.

Required rewrite pattern:

- Technical line: <original>
- In plain terms: <simple action/outcome sentence>

### Visual explanations (required)

Use a diagram when visual structure will improve understanding.

Add a diagram when the concept includes:

- layered dependencies
- state transitions
- feedback loops
- trade-offs between speed, risk, and reversibility
- propagation (failure, delay, misfit, value drift)

Diagram rules:

- Prefer Mermaid diagrams embedded directly in markdown pages.
- Keep diagrams simple (usually 5 to 12 nodes).
- Use plain labels and avoid dense jargon in node text.
- Add one short lead-in sentence before each diagram.
- Add one short interpretation after each diagram in this form:
   - In plain terms: <what to do with this diagram>
- If Mermaid is not practical, include a static SVG or PNG plus one plain-language summary line.

Maintenance rules:

- Ensure diagrams and surrounding text stay consistent when concept meaning changes.
- Ensure diagrammed pages still include meaningful See also links.


## Query

When asked a question against the wiki:
1. Read `wiki/index.md` to find candidate pages.
2. Read relevant pages.
3. Synthesize an answer with explicit citations.
4. If the output is durable, propose filing it as a new wiki page.

## Lint

When asked to lint:
1. Check for orphan pages (no inbound links).
2. Check broken links.
3. Check contradictions across major pages.
4. Check concept vocabulary and linking:
   - Read `wiki/_concepts_vocabulary.md` to identify current concepts.
   - Scan pages for concept mentions that are not linked.
   - Ensure 'See also' sections link genuinely related concepts (aim for 4–8 per page).
   - Verify entry-point pages (`drift_check.md`, `context.md`, `capability.md`) link liberally outward.
5. Check readability and language density:
   - Flag sentences longer than 24 words.
   - Flag abstract phrasing that hides practical action.
   - Ensure each section includes at least one concrete action cue.
   - Propose a plain-language rewrite for flagged sentences.
6. Check visual clarity opportunities:
   - Flag pages where visual structure would improve understanding but no diagram exists.
   - Prioritise diagrams for entry-point and dependency-heavy pages.
   - Ensure each diagram includes a plain-language interpretation line.
7. Propose concrete fixes and apply if requested.
8. Append lint entry to `wiki/log.md`.

## Refresh Index

When asked to refresh index:
1. Enumerate all content pages in `wiki/` except `index.md`, `log.md`, `sources.md`.
2. Ensure each page appears exactly once in `wiki/index.md` with a one-line description.
3. Log the update.

### Index Quality Standards

The index is the navigator's first encounter with the wiki. It must be more than a bare catalog; it is part of the user experience.

**Opening Section (required):**
- Lead with a 2–4 sentence explanation of what the wiki is for and what problems it solves (observable, decision-maker language).
- Include 2–3 brief entry points: "Start here if you're concerned about...", "Start here if you're not sure whether...", "Start here if you want to understand...".
- These entry points should name observable situations, not abstract concepts.

**Section Narratives (required):**
- Each section header should hint at why concepts cluster. Not just categorical labels, but brief framing.
- Example bad: "System Concepts"
- Example good: "What Actually Happens: Signals, Fragility, and the Limits of Control"

**Descriptions (required):**
- Descriptions should be 1–2 sentences, not definitions.
- Lead with what matters, not what the concept is. "When decisions are repeatedly reopened" beats "Alignment is consistency".
- Use decision-maker language: observable problems, behavioural signals, consequences, decision points.
- Include one plain action or consequence cue where possible.

**Connection Hints (optional but valuable):**
- For entry-point pages, add a subtle hint about next steps.
- Example: "Start with [capability.md](capability.md); if you notice outcomes are inconsistent, read [state.md](state.md) to see what's happening."

**Validation Checklist:**
- Is there a narrative intro explaining the purpose?
- Are there 2–3 user-type entry points using observable language?
- Do section headers give structure meaning, not just category names?
- Is each description 1–2 sentences and problem-focused?
- Are entry-point pages linked with next-step hints for common scenarios?

## Log Entry Format

`## [YYYY-MM-DD] <operation> | <title>`

Fields: Scope, Files changed, Summary, Follow-ups (optional).

## Source Registry Format

Per source: source path, category (core/docs/background), ingested (yes/no), last ingested date, linked wiki pages, notes.

## Command Vocabulary

- `ingest <path>`
- `ingest all pending`
- `refresh index`
- `show recent activity`
- `query wiki: <question>`
- `lint wiki`
- `show source coverage`

## Guardrails

- Do not edit raw source files.
- Do not delete existing wiki pages without explicit request.
- Keep index and source registry synchronized with every ingest.

