# Context-Document Blueprints

The five-document core stack, with the exact structure for each file. Use the smallest stack that gives Claude enough evidence to work. Don't upload everything the user owns. Fill-in versions of all five live in `assets/starter-kit/` and can be generated as real files for the user.

Numbered, descriptive file names keep the knowledge base easy to maintain and easy for retrieval to find. One topic per document. When a fact goes stale, replace it in `03_Source_of_Truth.md`, never in five places at once. Conflicting versions are worse than a missing fact.

## `00_Project_Brief.md`: the job, locked

```markdown
# [Project Name]: Project Brief

## The job
[One sentence describing the recurring job.]

## Who this is for
[Audience, sophistication level, needs, and objections.]

## Inputs Claude will receive
- [Input 1]
- [Input 2]

## Required output
[Exact deliverable and format.]

## Success looks like
[Measurable or observable quality bar.]

## Constraints
[Deadlines, approvals, platform rules, compliance rules, required tools.]
```

## `01_Voice_and_Non_Negotiables.md`: sound like the user, never generic

```markdown
# Voice and Non-Negotiables

## Voice in one sentence
[Example: Direct, conversational, and specific, like a founder explaining the shortcut to a smart friend.]

## Do this
| Trait | What it means | Real example |
|---|---|---|
| Direct | Lead with the point. | "[Real sentence from approved work]" |
| Practical | Show the next action. | "[Real sentence from approved work]" |

## Do not do this
| Avoid | Why | Bad example | Better version |
|---|---|---|---|
| Corporate filler | It sounds fake. | "Leverage this robust framework." | "Use this simple workflow." |

## Required language and CTA rules
[Approved terms, banned terms, CTA placement, disclosures, spelling conventions.]
```

The before/after table is the highest-value part. Pull the "real example" sentences from actual approved work, not invented ones.

## `02_Gold_Standard_Examples.md`: proof of what good looks like

```markdown
# Gold-Standard Examples

## Example 1: [Name]
### Original input
[The rough brief, transcript, or raw material.]

### Final output
[The actual approved output.]

### Why this worked
- [Specific pattern to reuse.]
- [Specific audience response or quality marker.]

### Do not copy blindly
[What was context-specific.]
```

### When they have no examples yet

Never invent examples to fill this file. Fabricated work teaches Claude a voice the person does not have, and they will not be able to tell you why the output feels off.

If the ladder in `interview-guide.md` produced nothing, ship the file with this header so the gap is visible every time anyone opens it:

```markdown
# Gold-Standard Examples

> **This file is intentionally empty.** The project works without it, but the outputs
> will read more generic than they should until there are real examples in here.
> This is the one thing that will improve the output most.
>
> **Fill this in by: [date, two weeks out]**
> Fastest way: save the next three you make. Paste the best one in below, with one
> line on why it worked.
```

Include three to ten real examples. Quality beats quantity. The input to output pairing is what teaches the transformation. An output on its own teaches style but not process. Remove private information only where necessary.

## `03_Source_of_Truth.md`: facts that must be accurate

```markdown
# Source of Truth
**Last updated:** [Date]

## Approved facts and claims
| Topic | Approved fact | Proof / source | Use conditions |
|---|---|---|---|
| [Topic] | [Fact] | [Link or internal source] | [When it is safe to use] |

## Offers, links, and current details
[Current offers, links, product names, pricing, availability, event dates, contact details.]

## Never assume
[Facts Claude must ask about or flag instead of guessing.]
```

The "Never assume" list is the guardrail most projects skip and most need.

## `04_Workflow_and_QA.md`: the repeatable process and review rubric

```markdown
# Workflow and Quality Control

## Standard workflow
1. [Step]
2. [Step]
3. [Step]

## Final checklist
- [Requirement]
- [Requirement]
- [Requirement]

## Escalate or ask before proceeding when
- [A fact is missing.]
- [An approval is required.]
- [The request falls outside scope.]
```

## When to add more documents

Add beyond the core five only when the use case demands it, one topic per file. Common additions: audience questions and objections in their own words (comments, DMs, sales-call questions), partner/sponsor requirements with approved claims and disclosure rules, platform-specific format specs, or a library of past deliverables for a second output type. If a proposed document doesn't give Claude evidence it will actually use, don't create it.

## The improvement loop

The knowledge base is alive. After each strong output, add it to `02_Gold_Standard_Examples.md` with a note on why it worked. After each correction the user makes repeatedly, encode it as a rule in `01_Voice_and_Non_Negotiables.md` or the Instructions. A project that never updates its examples plateaus at its launch quality.

## How these files get delivered

Do not hand over five loose files and hope. Deliver a numbered folder so the order of operations is built into the names:

```
[Project Name] Claude Project/
  START-HERE.md                        personalized setup guide
  1-PASTE-THIS/
    project-instructions.md            goes in the Instructions box
  2-UPLOAD-THESE/
    00_Project_Brief.md                every file in here gets uploaded
    01_Voice_and_Non_Negotiables.md
    02_Gold_Standard_Examples.md
    03_Source_of_Truth.md
    04_Workflow_and_QA.md
  3-TRY-THESE/
    starter-prompts.md
```

Folder 1 gets pasted. Folder 2 gets uploaded. Folder 3 is what they type first. Beginners confuse pasting and uploading constantly, and these folder names do that teaching without you having to repeat it.

In a plain chat with no file tools, keep the same names and deliver each document as its own copy-paste block, with a line at the top of each saying what to name it and whether it is pasted or uploaded.
