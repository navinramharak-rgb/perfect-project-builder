# Perfect Project Builder

![License: MIT](https://img.shields.io/badge/License-MIT-orange.svg)
![Version](https://img.shields.io/badge/version-0.1.0-blue.svg)
![Beginner friendly](https://img.shields.io/badge/beginner-friendly-brightgreen.svg)

Turn any recurring workflow into a complete, paste-ready Claude Project. This plugin packages a proven build methodology into a skill your assistant can run: a strict split between Instructions and knowledge, a five-document context stack with fill-in templates, paste-ready Project Instructions, starter prompts, and a pressure test that proves the project works before you rely on it.

Most people build one vague "AI assistant for my business" project and wonder why the output sounds generic. This builds the opposite: one focused system per recurring job, loaded with real examples instead of theory.

## Quick start

1. **Install** the plugin (see Install below).
2. **Describe the recurring job:** "Build me a Claude Project that turns my rough voice notes into a weekly newsletter."
3. **Get the full setup:** paste-ready Instructions, the exact context documents to create (generated as real files if you want), starter prompts, and a pressure test.
4. **Paste, upload, test.** The project is usable the same day.

## What it produces

A complete Claude Project setup, never a partial plan:

- **Project Snapshot** — the one-line job, inputs, output, and human approval point.
- **Project Instructions** — one fenced block you paste without editing. Role, workflow, voice, output format, a What Not To Do list, and a quality check.
- **Context documents** — the five-document stack (`Project Brief`, `Voice and Non-Negotiables`, `Gold-Standard Examples`, `Source of Truth`, `Workflow and QA`), each with exact contents named, generated as real upload-ready files on request.
- **Starter prompts** — standard run, revision, and edge case.
- **Pressure test** — one realistic test prompt with success criteria, so you know it works before it matters.

## The core principle

> Instructions tell Claude **how to behave**. Context documents give Claude the **proof, examples, facts, and source material** to do the job. Never bury both jobs in one giant document.

"Be conversational" is theory. Five of your real captions is evidence. The skill builds with evidence.

## Install

This installs as a Cowork/Claude plugin.

- **Fastest:** download [`perfect-project-builder.plugin`](perfect-project-builder.plugin) from this repo, open it in Cowork, and click install. Prefer just the skill? Download [`build-perfect-project.skill`](build-perfect-project.skill) instead.
- **From the marketplace:** in Claude Code or Cowork, run:

  ```
  /plugin marketplace add navinramharak-rgb/perfect-project-builder
  /plugin install perfect-project-builder@build-with-nav
  ```

After installing, manage it in Settings under Capabilities. The skill activates automatically when you ask for a Claude Project setup — no manual invocation.

## How to use it

Describe the recurring job and what you already have. For example:

> "Build me a Claude Project for pitching hotels on brand deals. I have my media kit and six past emails that got replies."

Or:

> "I keep pasting the same brand context into every chat. Turn this into a proper project."

The assistant will:
1. check the job is actually project-shaped (one-off tasks get a strong reusable prompt instead);
2. ask only the questions that change the build — never a twenty-question intake;
3. write paste-ready Instructions with a use-case-specific What Not To Do list;
4. plan the smallest context stack that gives Claude real evidence, and generate the files;
5. hand you starter prompts and a pressure test to prove it works.

Trigger phrases include: "set up a Claude Project," "build a project for," "Project Instructions," "knowledge base," or describing any workflow you repeat weekly.

## What is inside

```
perfect-project-builder/
  .claude-plugin/
    plugin.json                     plugin manifest
    marketplace.json                makes the repo one-click installable
  skills/build-perfect-project/
    SKILL.md                        how the assistant builds a focused project
    references/
      instructions-playbook.md      the instructions-vs-knowledge split + paste-ready template
      context-blueprints.md         the five-document stack, fully specified
      patterns-and-example.md       use-case patterns + a fully worked example
    assets/starter-kit/             fill-in templates for the five core documents
  perfect-project-builder.plugin    one-click install file for Cowork
  build-perfect-project.skill       one-click install file for the skill alone
  LICENSE                           MIT
  CHANGELOG.md                      version history
  README.md                         this file
```

## Philosophy

- **One project, one job.** "Write my content" is too broad. "Turn rough voice notes into three Reel packages for business owners" is a usable project.
- **Evidence over theory.** Every context document holds real examples, real facts, real past work.
- **Exclusions prevent drift.** Every project gets a What Not To Do section, or it slides into generic AI output.
- **Facts live in one place.** A dated Source of Truth document, so updating an offer never means rewriting instructions.
- **Test before trusting.** Every build ends with a pressure test and named success criteria.

## License

MIT. Free to use, modify, and share, including commercially. Keep the copyright notice. See `LICENSE`.

## Credit

Made by Build With Nav. Learn more at [buildwithnav.com](https://buildwithnav.com).
