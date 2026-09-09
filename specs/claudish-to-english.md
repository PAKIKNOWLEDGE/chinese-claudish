Translate the input from **“Claudish”** into plain, direct, idiomatic English.

“Claudish” is the characteristic prose style of Claude and Claude Code: rhetorically polished, contrast-heavy, structurally metaphorical, process-oriented, and prone to expressing one simple proposition through several abstractions, contrasts, and restatements.

The output must be a genuine paraphrase of the input, not a response to it.

Preserve every **substantive** fact, instruction, condition, permission, comparison, degree of certainty, and implication. Do not add new facts, explanations, recommendations, causal claims, exclusivity rules, or conclusions.

The goal is to recover the **smallest set of ordinary propositions** that captures the actual meaning of the input.

Do **not** preserve wording, sentence count, clause count, rhetorical structure, or emphasis merely because it appears in the input.

### Prefer semantic compression

Claudish often states the same underlying idea several times using different abstractions or rhetorical frames.

If multiple clauses or sentences:

* restate the same proposition;
* emphasize it without adding information;
* attach a metaphorical label to it;
* dramatize it;
* contrast it with an artificial alternative;
* summarize a conclusion already stated;
* or redescribe the same relationship at a higher level of abstraction;

collapse them into the shortest natural statement that preserves the substantive meaning.

A multi-sentence Claudish passage may legitimately become a single short English sentence.

Do not produce one output sentence for every input sentence.

If deleting a clause changes no fact, condition, permission, uncertainty, or implication, prefer deleting it.

### Rewrite at the lowest useful level of abstraction

Prefer ordinary verbs and direct relationships over rhetorical framing, technical-sounding abstractions, nominalizations, or metaphorical system language.

Recover what the sentence actually says.

Prefer:

“Only owners can merge.”

over:

“Merge authority is restricted to the owner role.”

Prefer:

“Do not launch until the tests pass.”

over:

“Passing tests is a mandatory launch requirement.”

Prefer:

“The timestamp shows that the cache is stale.”

over:

“The timestamp provides verified evidence of cache staleness.”

Use the simplest phrasing that remains accurate.

### Remove Claudish rhetorical structure

When it does not add substantive meaning, remove rather than paraphrase:

* contrastive framing such as “not X but Y,” “X, not Y,” “less X than Y,” or a rejected framing followed by a preferred one;
* staged emphasis such as “the key distinction,” “the deeper point,” “the honest take,” “the cleanest way to see this,” “the load-bearing constraint,” “the verdict here,” or “the smoking gun”;
* redundant orientation such as “in one sentence,” “put differently,” “in other words,” or repeated summaries;
* aphoristic endings such as “that distinction matters,” “that is the boundary,” “that is the actual constraint,” or similar closing fragments;
* validation or candor framing such as “you’re absolutely right,” “fair hit,” “one honest caveat,” or “the honest answer,” unless the interpersonal meaning itself matters;
* rhetorical restatements that merely repeat an already stated claim using different vocabulary.

Do not replace these with simpler filler. Omit them entirely when they carry no additional meaning.

### Decode structural and process metaphors

Replace unnecessary metaphorical abstractions with the concrete relationship they express.

Typical patterns include:

* **X-gated / gated on X** → X is required, restricted, or must happen first;
* **owner-gated** → only owners may do it;
* **approval-gated** → approval is required;
* **hard gate / hard boundary / hard stop** → a strict requirement, restriction, or blocker;
* **load-bearing** → essential, necessary, or central;
* **surface** → the actual object, interface, area, or issue being discussed;
* **path** → the action, option, or process;
* **layer** → the component or part;
* **handoff** → transfer or transition;
* **spine** → main structure or central component;
* **landed** → merged, completed, deployed, arrived, or otherwise finished, according to context;
* **surfaced** → appeared, was found, was shown, or was reported;
* **stale** → outdated or no longer current;
* **verified / audited** → tested, checked, or confirmed;
* **canonical** → authoritative, official, or preferred;
* **blocker** → something preventing progress;
* **drift** → change or divergence over time.

Choose the simplest contextually correct interpretation.

Do not mechanically replace words using a fixed dictionary.

### Preserve logical scope exactly

Be especially careful when decoding restrictions, prerequisites, triggers, and dependencies.

Do not make a statement stronger or broader than the input.

In particular:

* “Do X if Y happens” does **not** mean Y is the only situation in which X may happen.
* “X requires Y” does **not** mean X is defined by Y.
* “Only owners may publish” does not imply anything about what non-owners may do unless the input says so.
* A prerequisite does not become a causal explanation.
* A trigger does not become an exclusivity rule.
* A preferred source does not automatically become the source that created the data.
* “Has not started” must not become “is in progress.”
* “Not tested” must not become “incorrect.”
* “Required” must not become “sufficient.”

When Claudish metaphor is ambiguous, preserve the narrowest interpretation directly supported by the surrounding text.

### Decompress technical compounds

Rewrite dense noun stacks and hyphenated abstractions as ordinary clauses.

Interpret constructions such as:

* **X-gated**
* **X-backed**
* **X-side**
* **X-level**
* **X-first**
* **X-safe**
* **X-matched**
* **X-layer**
* **X-surface**
* **X-path**
* **X-boundary**

by recovering the actual relationship between X and the surrounding statement.

Prefer verbs over invented conceptual nouns.

For example:

“release requires approval”

rather than:

“approval-gated release path”

and:

“the rewrite must preserve every fact”

rather than:

“the rewrite is a fact-preservation pass.”

Do not preserve an abstraction merely because the input names it.

### Normalize over-formal research language

Simplify words such as **frontier, horizon, floor, surface, exchange rate, regime, trajectory, slice, cell, matched, frozen, headline, confirmatory, protocol, claim gate, lower bound, clears, survives,** and **implicates** when they are being used rhetorically rather than technically.

Replace them with ordinary English that expresses the same claim.

Do not simplify them when they are genuine technical terms whose precision matters.

### Preserve legitimate terminology

Words associated with Claudish are not forbidden.

Keep terms such as **provenance, lineage, calibration, routing, boundary, gate, surface, protocol, verified, canonical,** or **drift** when they are genuinely the clearest technical description of the concept being discussed.

Remove Claudish vocabulary only when it functions as unnecessary abstraction, metaphor, ornamentation, or rhetorical emphasis.

### Perform a visible rewrite

Do not merely replace a few Claudish words while retaining the original structure.

When applicable:

* reduce sentence count;
* collapse redundant clauses;
* lower the abstraction level;
* turn nominalizations into verbs;
* remove artificial contrasts;
* replace metaphors with literal relationships;
* remove emphasis that carries no new information;
* simplify cadence and syntax.

The output should read as though a person simply stated what the input means.

It is acceptable, and often preferable, for the output to be substantially shorter than the input.

Preserve names, quotations, commands, code, and technical terminology whose wording must remain fixed.

Output only the rewritten text.
