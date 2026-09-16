# Changelog

## 0.2.0
Rebuilt around the beginner. The skill no longer returns a plan for someone who already knows what they are doing. It interviews, builds, sets up, and tests.

- **Guided interview.** Four rounds of three to five questions, each with a why line and a checkpoint, replacing the old "ask up to five questions if needed" step. Full wording in the new `references/interview-guide.md`.
- **A real answer for people with no examples.** A three-step ladder: talk the examples out of them and write them up, reconstruct from adjacent material, or build anyway with the gap visibly flagged and dated. Never invent examples.
- **Files instead of a plan.** Output is a numbered folder where the names teach the order of operations: `1-PASTE-THIS`, `2-UPLOAD-THESE`, `3-TRY-THESE`. Paste-versus-upload is the most common beginner mistake and the structure now prevents it.
- **Click-by-click setup.** New `references/setup-walkthrough.md` covers creating the project, pasting, uploading, confirming, troubleshooting, and a diagnosis table for reading the first output.
- **Tested before handoff.** The build is not finished until the user has run a prompt and pasted the result back for diagnosis.
- **How to talk to a beginner.** New section in SKILL.md: one round at a time, say why you are asking, define every term once, ask for concrete instances instead of categories.
- **The mirror move.** Instead of asking someone to describe their own voice, pull real lines from their uploads and ask which sound like them.
- Added the `/build-project` command.
- Added `START-HERE-template.md` and `Setup_Checklist.md` to the starter kit, and renamed `README-START-HERE.md` to `HOW-TO-USE-THIS-KIT.md` so it is no longer confused with the `START-HERE.md` that ships to the user.
- Specified the two deliverables that were previously left to improvisation: what goes in `START-HERE.md`, and the exact three starter prompts, where prompt 1 is always the pressure test.
- Removed em dashes throughout, in line with the Build With Nav voice.

## 0.1.1
- Corrected the retrieval (RAG) note: automatic knowledge expansion is not limited to paid plans.
- Added the platform facts a first-time builder needs: Claude cannot see the project name or description, project files cap at 30MB with text extraction only (PDFs excepted, 1000 pages max, visual analysis only under 100 pages), and retrieval activates automatically and cannot be toggled.
- Starter kit README now warns against uploading scans and image-heavy PDFs as project knowledge.

## 0.1.0
- Initial release: the build-perfect-project skill, the instructions playbook, the five-document context blueprints, use-case patterns with a fully worked example, and a fill-in starter kit.
