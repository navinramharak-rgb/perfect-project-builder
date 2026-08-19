---
name: build-perfect-project
description: Turn any recurring workflow into a complete, paste-ready Claude Project — Project Instructions, a context-document plan with fill-in templates, starter prompts, and a pressure test. Use when someone wants to "set up a Claude Project", "build a project for X", needs Project Instructions or a knowledge-base plan, wants a repeatable system for content creation, newsletters, outreach, research, proposals, or support, keeps re-pasting the same context into every chat, or asks "how should I structure my Claude Project".
---

# Build a Perfect Claude Project

Build Claude Projects that do one recurring job well. Never build a vague "AI assistant for my business." Build a focused system with clear behavior, real context, and an output the user can ship.

> **Core principle:** Instructions tell Claude **how to behave**. Context documents give Claude the **proof, examples, facts, and source material** to do the job. Never bury both jobs in one giant document.

Write in a direct, practical voice — like a smart operator explaining exactly what to do next, not a corporate consultant.

Reach for the references as needed (progressive disclosure). Do not paste their full contents into responses unless the task needs it:
- `references/instructions-playbook.md`: the instructions-vs-knowledge split, the paste-ready Instructions template, and the operating rules for writing them.
- `references/context-blueprints.md`: the five-document context stack with full blueprints for each file.
- `references/patterns-and-example.md`: use-case patterns and one fully worked example at the required level of specificity.

Fill-in template files live in `assets/starter-kit/`. When working in an environment with file access, offer to generate the context documents as real files the user can upload straight into their project — not just a plan describing them.

## 0. Gate: should this even be a project?

Run this check before building anything:

- **Same workflow, same standards, recurring weekly or daily** → build one focused project.
- **One-off task** → don't build a project. Write the user one strong reusable prompt instead.
- **The work is a multi-step procedure Claude should execute** (not a workspace with context) → suggest a skill, not a project.
- **"One project for everything"** → refuse politely. Break it into the 1–3 recurring workflows with the most leverage and build the first one.
- **Shared voice, different audiences or facts** → separate projects, or one shared brand-context document reused across focused projects.

## 1. Collect only what changes the build

Start with what the user already gave. If the brief is clear enough, state reasonable assumptions and build. If critical information is missing, ask only the smallest set of questions that changes the build — never more than five at once.

What matters: the recurring job, the finished output and who it's for, what the user will supply each time, real examples of "good" (past work, transcripts, approved outputs), voice and hard rules, and constraints (approvals, compliance, formats, deadlines).

## 2. Define the job in one sentence

> "This project helps **[person]** turn **[input]** into **[specific output]** for **[audience]**, while following **[core standards]**."

If this sentence is fuzzy, the project will be fuzzy. Tighten it before anything else. Then map the operating loop: trigger → inputs → Claude's work → human review → final output → best outputs added back to project knowledge as new examples.

## 3. Split instructions from knowledge

The rule, without exception: role, workflow, output format, tone rules, quality checks, and exclusions go in **Project Instructions**. Approved facts, real examples, past outputs, transcripts, offers, policies, and templates go in **context documents**. "Write in a direct voice" is an instruction; five past captions that demonstrate the voice are knowledge. Full playbook: `references/instructions-playbook.md`.

## 4. Build the context stack

Use the smallest stack that gives Claude enough evidence — the five-document core in `references/context-blueprints.md` (`00_Project_Brief`, `01_Voice_and_Non_Negotiables`, `02_Gold_Standard_Examples`, `03_Source_of_Truth`, `04_Workflow_and_QA`), adding files only when the use case demands. Real examples beat theory every time: past newsletters over "be conversational," actual sent emails over outreach advice.

### Platform facts that change how you build

- **Claude cannot see the project name or description.** Those fields are for humans browsing the project list. Every instruction and every fact has to live in the Instructions field or in an uploaded document. This is the most common first-timer mistake: writing the brief into the description and wondering why Claude ignores it.
- **Knowledge is retrieved per query on large knowledge bases.** When project knowledge approaches the context window, Claude automatically switches on retrieval, expanding capacity by up to 10x and pulling only the most relevant content for each question. It turns on by itself and cannot be toggled manually. The practical consequence: keep every document focused on one topic with a descriptive file name, because that is what makes retrieval find it. A fact buried in an unrelated mega-document may never surface.
- **Uploads have real limits.** Project files cap at 30MB each, well below the chat upload limit. Claude extracts text only, except for PDFs. PDFs cap at 1000 pages, and visual elements are analyzed only in PDFs of 100 pages or fewer. So a scanned or image-heavy document is close to useless as project knowledge. Convert it to text first, or paste the parts that matter into a markdown file.
- **Projects are available on all plans**, with free accounts capped at five projects. Projects also keep their own memory space and can generate an editable summary from conversations. Team and Enterprise plans can share a project with view or edit permissions.

## 5. Write the Instructions

Use the template in `references/instructions-playbook.md`. Instructions are an operating system, not an essay: role and outcome, operating workflow, voice and standards, exact output format, a what-not-to-do list, and a final quality check. The result must be paste-ready — one fenced block the user copies without editing. Every project gets a **What Not To Do** section; a project without exclusions drifts into generic AI output.

## 6. Starter prompts and pressure test

Give three to five copy-paste starter prompts: one standard run, one revision, one hard edge case. Then create one realistic test prompt and state what a good answer must include. If the project can't pass with the supplied documents, name the missing context before declaring it done.

## 7. Deliver the full setup

Return **all** sections, in order — never a partial plan:

1. **Project Snapshot** — name, one-line job, best for, primary output, inputs needed each time, human approval point.
2. **Project Instructions** — complete, in one fenced block.
3. **Context documents to create** — table of file, purpose, exact contents, structure. Offer to generate them as real files from `assets/starter-kit/`.
4. **Build order** — from "collect examples" to "test the project," followable by a non-technical user.
5. **Starter prompts.**
6. **Pressure test** — prompt, success criteria, what to add if it fails.
7. **What not to do** — project-specific failure modes, not generic warnings.

## Non-negotiables

- One focused recurring job per project. No "assistant for everything."
- Instructions are paste-ready. No placeholders left unfilled, no "adapt as needed."
- Every recommended context document names real material to put in it.
- Voice guidance plus a What Not To Do section, always.
- Missing facts become questions or labeled assumptions — never invented instructions.
- Do not end with "let me know if you want more." The job is to make the project usable now.
