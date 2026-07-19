# Instructions Playbook

How to decide what goes where, and how to write Project Instructions that behave like an operating system.

## The split: Instructions vs. context documents

Use this rule without exception:

| Put it in **Project Instructions** | Put it in **Context Documents** |
|---|---|
| Role, workflow, output format, tone rules, quality checks, exclusions, escalation rules. | Approved facts, real examples, past outputs, transcripts, offers, FAQs, policies, audience research, templates, source material. |
| "Write in a direct, practical voice." | Five past captions that demonstrate the direct, practical voice. |
| "Never make unverified claims." | A list of verified claims, product specs, and approved links. |
| "Return three hooks, a script, and a caption." | Top-performing posts and notes on why they worked. |

Why the split matters:

- **Instructions apply to every conversation in the project.** They are the permanent system prompt. Anything long, changeable, or example-heavy inflates every single chat.
- **Knowledge is retrieved when relevant.** On paid plans, large knowledge bases use retrieval (RAG) — Claude pulls the most relevant documents per query. A fact buried inside an unrelated mega-document may never be retrieved. One topic per document, descriptive file names.
- **Facts change; behavior doesn't.** Prices, offers, links, and claims belong in a source-of-truth document with a last-updated date, so updating them never means rewriting the Instructions.

## Operating rules for writing Instructions

1. **Concise and directive.** Use commands: "Ask," "Draft," "Verify," "Return," "Never." Instructions are operating rules, not a brand manifesto.
2. **Encode the workflow as numbered steps.** Claude follows sequences far more reliably than prose descriptions of intent.
3. **Always include a What Not To Do section.** A project without exclusions drifts into generic AI language. Make the exclusions specific to this use case's real failure modes.
4. **End with a quality check.** Three concrete pass conditions Claude verifies before sending.
5. **Point at the knowledge.** Tell Claude which documents to consult for which decisions ("Match the format in the gold-standard examples"; "Only state facts present in the Source of Truth").
6. **Don't automate ambiguity.** If the human workflow is unclear, map it first. A project should support a real workflow, not hide a broken one.

## The paste-ready Instructions template

Fill every bracket. The final version must paste into the Project Instructions field with zero editing.

```markdown
## Role and outcome
You are [role]. Your job is to turn [inputs] into [output] for [audience]. Optimize for [success definition].

## Operating workflow
1. Review the user's request and the relevant project knowledge.
2. If a critical input is missing, ask only the question that blocks quality. Otherwise state any assumption briefly and continue.
3. Do the work in this order: [step 1] → [step 2] → [step 3].
4. Verify [facts / constraints / requirements] against [source-of-truth document] before finalizing.

## Voice and standards
- Write in a [three-to-five-word voice description] voice.
- Prioritize [clarity / specificity / usefulness / evidence].
- Use real examples and concrete language.
- Match the format in the project's gold-standard examples without copying them word for word.

## Output format
Return every response in this exact order:
1. [Section]
2. [Section]
3. [Section]

## What not to do
- Do not [most common failure mode for this use case].
- Do not [banned tone / phrase / claim type].
- Do not invent facts, results, experience, quotes, or links.
- Do not [use-case-specific exclusion].

## Quality check before sending
Confirm the output is [check 1], [check 2], and [check 3]. If it is not, fix it before sending.
```

## Signs the Instructions are wrong

- They read like an essay or a mission statement → rewrite as commands and numbered steps.
- They contain examples, prices, links, or facts → move those to context documents.
- They exceed roughly a page → something belongs in knowledge instead.
- They have no exclusions → the outputs will sound like every other AI.
- The user must edit them before pasting → the build isn't done.
