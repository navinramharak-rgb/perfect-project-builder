# How to use this kit

The numbered files in this folder are the knowledge base for one focused Claude Project. `Setup_Checklist.md` is not one of them: it is for you, to tick off while you set the project up, and it never gets uploaded.

Fill them in, or have Claude fill them in with you during the interview, then upload all of them to your project's knowledge.

**Two things that trip up everyone the first time:**

1. **The Project Instructions get pasted, not uploaded.** They go in the Instructions box inside the project. The numbered files get uploaded. Mixing this up is the most common reason a project seems to ignore its own rules.
2. **Claude cannot see your project name or description.** Those fields are for you, browsing your own project list. Anything Claude needs to know goes in the Instructions or in one of these files.

**Rules that make this work:**

1. **One topic per file.** Retrieval finds focused documents. It misses facts buried in mega-documents.
2. **Real material only.** Paste actual past work, actual sent emails, actual approved claims. "Be conversational" teaches nothing. Five real captions teach everything. Never invent examples to fill a gap. A fabricated example teaches Claude a voice you do not have, and you will not be able to tell why the output feels wrong.
3. **Keep `03_Source_of_Truth.md` current.** When a fact changes, change it there and nowhere else. Never leave two versions alive.
4. **Feed the loop.** When an output performs, add it to `02_Gold_Standard_Examples.md` with a note on why it worked. When you correct the same thing twice, make it a rule in `01_Voice_and_Non_Negotiables.md`.
5. **Upload text, not scans.** Project files cap at 30MB each and Claude extracts text only, except for PDFs. If your source is a scan, a screenshot, or an image-heavy PDF, copy what matters into one of these markdown files instead of uploading the original.

**Fill-in order: 00 → 02 → 01 → 03 → 04.** Examples before voice, because the voice file is much easier to write once real examples are sitting in front of you.

**No examples yet?** Do not skip `02_Gold_Standard_Examples.md` and do not make some up. Leave the empty-file header in place with a date on it, build the project anyway, and come back and fill it. The project will work. It will just sound more generic than it should until you do.
