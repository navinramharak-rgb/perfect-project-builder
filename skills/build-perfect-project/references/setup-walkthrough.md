# Setup Walkthrough

Handing someone a folder of files is not finishing the job. Most beginners stall at exactly this point: they have the files, they open Claude, and they do not know where anything goes.

Run this with them, one step at a time. Wait for a "done" or a "stuck" before moving to the next step. Do not paste all eight steps at once.

## What they are getting

```
[Project Name] Claude Project/
  START-HERE.md                        the setup guide, personalized to them
  Setup_Checklist.md                   ticked off as they go, never uploaded
  1-PASTE-THIS/
    project-instructions.md            pasted into a box in Claude, never uploaded
  2-UPLOAD-THESE/
    00_Project_Brief.md                uploaded as files, never pasted
    01_Voice_and_Non_Negotiables.md
    02_Gold_Standard_Examples.md
    03_Source_of_Truth.md
    04_Workflow_and_QA.md
  3-TRY-THESE/
    starter-prompts.md                 copy one of these into the project to start
```

The numbers are the order of operations. Say that out loud once: folder 1 gets pasted, folder 2 gets uploaded, folder 3 is what they type first.

## The two things every beginner gets wrong

Say both of these before they start, not after they have made the mistake:

1. **The Instructions get pasted, not uploaded.** If they upload `project-instructions.md` as a knowledge file, it becomes reference material Claude might look at instead of the rules Claude always follows. It has to go in the Instructions box.
2. **Claude cannot see the project name or description.** Those fields are for them, browsing their own project list. Anything Claude needs to know goes in the Instructions or in an uploaded document.

## The steps

Deliver these one at a time. Steps 1 to 6 are Phase 6 of the skill. Steps 7 and 8 are Phase 7, the pressure test, and they are not optional.

**Step 1. Open Projects.** Go to claude.ai and find Projects in the left sidebar. Ask them to confirm they see it before continuing.

**Step 2. Create the project.** Click Create project. Name it `[their project name]`. The description is optional and Claude never reads it, so anything they find useful is fine.

**Step 3. Open the Instructions.** Inside the new project, find the instructions area. Depending on what they see it may be labeled Instructions, or sit behind a Set instructions or Edit button near the top of the project.

**Step 4. Paste.** Open `1-PASTE-THIS/project-instructions.md`, select all, copy, paste into the Instructions box, save. Tell them not to edit it. It is written to be pasted as is.

**Step 5. Upload the knowledge.** Find the project knowledge area, usually labeled Project knowledge or an Add content or plus button. Upload all five files from `2-UPLOAD-THESE/` together.

**Step 6. Confirm.** Ask them how many files are listed in project knowledge. It should match the number of files in `2-UPLOAD-THESE/`, which is five for a standard build and six if you added an optional sixth topic file. If it is fewer, something did not attach and they should retry the missing one.

**Step 7. First run.** Open `3-TRY-THESE/starter-prompts.md`, copy **prompt 1**, start a new chat inside the project, paste it, send. Prompt 1 is always the pressure test, so this is the only prompt that matters right now.

**Step 8. Bring the result back.** Ask them to paste the output back into this conversation so you can read it and diagnose. This is the pressure test and it is not optional. Do not let them leave before this step.

## When something goes wrong

Keep these short and non-technical. Do not ask them to check anything they cannot see.

- **"I do not see Projects."** They may be on a very old app version or signed into the wrong account. Ask them to refresh the page or sign out and back in.
- **"It says I have reached my project limit."** Free plans cap how many projects you can have. They can delete one they do not use, or upgrade.
- **"The file will not upload."** Project files have a size cap, currently 30MB each. If it is a scan, a screenshot, or an image-heavy PDF, Claude gets little or nothing from it anyway. Ask them to paste the text into one of the markdown files instead.
- **"Which box is the Instructions box?"** Ask them to describe what they see on the project page. Layouts change; their description is more reliable than any label memorized here.
- **"The output ignored my rules."** First thing to check: did the instructions get uploaded as a file instead of pasted into the box? This is the most common cause by a distance.

## Reading the first result

When they paste the output back, diagnose against the knowledge base, not against the instructions alone:

| What you see | What is actually wrong | What to tell them to do |
|---|---|---|
| Generic, could be anyone | `02_Gold_Standard_Examples.md` is thin or empty | Add three real examples. Name which ones. |
| Invented a fact, price, or link | That fact is missing from `03_Source_of_Truth.md` | Add the fact with its source. |
| Wrong shape or missing sections | The Output format section is too vague | Tighten it, give them the replacement text. |
| Right content, wrong tone | `01_Voice_and_Non_Negotiables.md` has no real before and after examples | Add two real lines they would say, and two they would never say. |
| Asked a question instead of doing it | Good behavior if a fact was genuinely missing. Add the fact. | Confirm this is working as intended. |

Say plainly which of these it is. A beginner cannot tell the difference between a bad project and a thin knowledge base, and if you do not name it they will assume the whole thing does not work.

## The close

Three lines, no more:

1. When something comes out great, paste it into `02_Gold_Standard_Examples.md` with one line on why it worked.
2. When you correct the same thing twice, make it a rule in `01_Voice_and_Non_Negotiables.md`.
3. When a price, link, or date changes, change it in `03_Source_of_Truth.md` and nowhere else.

Then give them the date to come back and fill any gap you flagged.
