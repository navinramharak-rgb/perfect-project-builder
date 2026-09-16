---
name: build-perfect-project
description: Interview a first-time builder and walk them all the way to a working Claude Project: questions, real files, setup, and a tested first output. Use when someone wants to "set up a Claude Project", "build a project for X", needs Project Instructions or a knowledge base, keeps re-pasting the same context into every chat, says they do not know where to start with Claude or how to set it up for their business, or asks how to structure a Claude Project for content, newsletters, social posts, outreach, proposals, research, client work, or customer support.
---

# Build a Perfect Claude Project

Assume the person has never built one and does not know what a Project, an Instructions field, or a knowledge base is. Do not hand them a plan and wish them luck. Interview them, build the files for them, then walk them through setup step by step and test it with them before you let them go.

> **Core principle:** Instructions tell Claude **how to behave**. Knowledge documents give Claude the **proof, examples, facts, and source material** to do the job. Never bury both jobs in one giant document.

**The promise you are keeping:** they finish this conversation with a project that works today, not a to-do list.

## How to talk to a beginner

This matters more than any template here. Get it wrong and they quit in round two.

- **One round of questions at a time.** Three to five questions, then stop and wait. Never dump twenty questions.
- **Say why you are asking** before each round, in one line.
- **Never use a term without defining it once.** Project, Instructions, knowledge, retrieval. Define on first use, in plain words, then move on.
- **Ask for concrete things, not categories.** "What did you make last week that you will have to make again?" beats "what is your recurring workflow?"
- **Accept messy answers.** Reflect back what you heard, fill the rest with a labeled assumption, say so, and keep moving. Do not re-ask.
- **Give them the win early and often.** After every round, say what you now have and what is left.
- **Never end a phase with "let me know if you want more."** Tell them the exact next thing to do.

Write in a direct, practical voice. No corporate tone, no em dashes, no filler.

Read the references as you reach each phase. Do not paste their contents into responses:
- `references/interview-guide.md`: Phases 1 to 4. The question rounds word for word, handling vague answers, and getting examples out of someone with no files.
- `references/context-blueprints.md`: Phase 5. The knowledge documents, fully specified, plus the delivered folder structure.
- `references/instructions-playbook.md`: Phase 5. The instructions-vs-knowledge split and the paste-ready Instructions template.
- `references/setup-walkthrough.md`: Phases 6 and 7. The step-by-step setup script, troubleshooting, and the diagnosis table.
- `references/patterns-and-example.md`: use-case patterns and one fully worked example at the required level of specificity.

Templates live in `assets/starter-kit/`.

## Phase 0. Orient and gate

Open with what they are about to get and how long it takes. Be honest about the shape of it: about twenty minutes of questions, plus however long it takes them to go dig up a few real examples, and they will have a working project at the end.

Then run the gate:

- **Same job, same standards, recurring weekly or daily** → build one focused project.
- **One-off task** → do not build a project. Write them one strong reusable prompt instead and say why.
- **A multi-step procedure Claude should execute** rather than a workspace with context → a skill fits better. Say it in one line: a project is what Claude knows, a skill is how Claude does something.
- **"One project for everything"** → say no, kindly, and explain the cost: a project that does everything sounds like nothing. Name the one or two recurring jobs that eat the most of their time and build the first one today. Tell them the second one can come later.
- **Shared voice, different audiences** → separate projects, or one shared brand document reused across focused projects.

## Phases 1 to 4. The interview

Four rounds, each ending in a checkpoint. Run them from `references/interview-guide.md`, which has the exact wording.

1. **The job.** What they repeat, who receives it, what they start with, what they hate. Ends with the one-sentence job written back and confirmed.
2. **The material.** Send them to find real examples, with a specific list and specific places to look. This round decides whether the project is good or generic. Do not skip it or soften it. When they come back with nothing, work the three-step ladder in the interview guide: talk the examples out of them and write them up, then reconstruct from adjacent material, then as a last resort build anyway with the gap flagged and dated. Never invent examples.
3. **Voice and hard rules.** What sounds like them, what makes them cringe, what they cannot say, what must appear every time.
4. **Facts and approvals.** What must be right every time, what Claude must never guess, who signs off, what goes stale.

Stop interviewing after Round 4. If something is still missing, write it into `03_Source_of_Truth.md` under "Never assume" and build.

## Phase 5. Build the files

Deliver a numbered folder. The structure and the naming rules are in `references/context-blueprints.md`; follow them exactly, because the folder names are what teach paste-versus-upload.

Four things that folder must contain, none of which are optional:

1. **`1-PASTE-THIS/project-instructions.md`** from the template in `references/instructions-playbook.md`. Every bracket filled. Paste-ready with zero editing.
2. **`2-UPLOAD-THESE/`** with the knowledge documents from `references/context-blueprints.md`. Five for a standard build, plus a sixth topic file only when the use case genuinely needs one.
3. **`3-TRY-THESE/starter-prompts.md`** with exactly three prompts, in this order: **prompt 1 is the pressure test**, the standard run they will type first; prompt 2 works from a supplied reference or a hard edge case; prompt 3 asks the project to review a draft against its own rules. Prompt 1 is the one Phase 7 tests, so it has to be the realistic everyday job.
4. **`START-HERE.md`**, built from `assets/starter-kit/START-HERE-template.md` and personalized. It carries the project snapshot, the two paste-versus-upload warnings, the build steps, the pressure test with its pass criteria, the improvement loop, and any flagged gap with its due date. Copy `Setup_Checklist.md` in alongside it.

**Where it goes.** Write the folder into the user's connected or working folder, named `[Project Name] Claude Project`, then send the files to them so they can actually open them. A folder they cannot see is the same as no folder.

**In plain chat with no file tools:** same names, same structure, delivered as separate copy-paste blocks, each with a line at the top saying what to name it and whether it gets pasted or uploaded.

Nothing ships with an unfilled bracket in it.

## Phase 6. Set it up with them

Run Steps 1 to 6 of `references/setup-walkthrough.md`, one at a time, waiting for a "done" or a "stuck" before the next one. Do not paste all the steps at once.

Say both beginner traps out loud before they start, not after they hit one: the Instructions get pasted into the Instructions box and never uploaded, and Claude cannot see the project name or description.

## Phase 7. Test it, then set the first week

Do not declare it done. Prove it.

Steps 7 and 8 of the walkthrough: they run prompt 1 in the new project and paste the result back to you. Read it and diagnose against the table in `references/setup-walkthrough.md`, then say plainly which of those it is. A beginner cannot tell a thin knowledge base from a broken project, and if you do not name it they will assume the whole thing does not work.

Close with the improvement loop and a date for anything you flagged as missing. Both are already written in their `START-HERE.md`, so keep it to three lines here.

## Platform facts that change how you build

- **Claude cannot see the project name or description.** Those fields are for humans browsing the project list. Every instruction and every fact has to live in the Instructions field or in an uploaded document. This is the most common first-timer mistake: writing the brief into the description and wondering why Claude ignores it.
- **Knowledge is retrieved per query on large knowledge bases.** When project knowledge approaches the context window, Claude automatically switches on retrieval, expanding capacity by up to 10x and pulling only the most relevant content for each question. It turns on by itself and cannot be toggled. So keep every document focused on one topic with a descriptive file name, because that is what makes retrieval find it. A fact buried in an unrelated mega-document may never surface.
- **Uploads have real limits.** Project files have a size cap, currently 30MB each, well below the chat upload limit. Claude extracts text only, except for PDFs, which cap at 1000 pages with visual elements analyzed only under 100 pages. A scan or a screenshot is close to useless as project knowledge. Convert it to text, or paste the parts that matter into a markdown file.
- **Projects are available on all plans**, and free plans cap how many you can have. Projects keep their own memory space and can generate an editable summary from conversations. Team and Enterprise plans can share a project with view or edit permissions.

## Non-negotiables

- Interview before building. Never generate a project from a one-line request without asking anything.
- One focused recurring job per project. No assistant for everything.
- Every document contains real material or is clearly marked empty with a date to fix it. Never invent examples, results, quotes, or links.
- Instructions are paste-ready. No unfilled brackets, no "adapt as needed."
- Voice guidance plus a What Not To Do section, always.
- The job is not done when the files exist. It is done when they have tested it and you have read the result.
