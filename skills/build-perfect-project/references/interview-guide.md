# Interview Guide

Four rounds. Three to five questions each. A checkpoint after every round. Roughly twenty minutes end to end.

The person you are talking to has probably never built a Claude Project and may not be sure what one is. They will not answer abstract questions well. Every question below is written to be answerable by someone describing their actual week.

**Rules for every round:**

- Say why you are asking, in one line, before the questions.
- Ask the questions as a short numbered list. Then stop. Wait.
- If they answer three of four, take what you got. Fill the gap with a labeled assumption and say so. Do not re-ask.
- If an answer is a category ("content", "emails", "client stuff"), ask one follow-up for a specific instance. Categories produce generic projects.
- End with a checkpoint: what you now have, what is next, how much is left.

---

## Round 1: The job

**Why line:** "First I need to know exactly what we are building this for. One specific thing you make over and over, not a category."

**Questions:**

1. What is something you made in the last two weeks that you know you will have to make again? Name the actual thing, not the category.
2. Who reads it or receives it? What do they already know, and what do they care about?
3. When you sit down to make it, what do you start with? Notes, a call recording, a blank page, a request from someone?
4. Roughly how long does it take you now, and which part of it do you hate most?

**Handling vague answers:**

- "Content" → "Pick one: a Reel, a LinkedIn post, a newsletter, a blog article. Which one do you make most often?"
- "Emails" → "What kind? Pitching someone new, following up, answering the same customer question, or something else?"
- "It depends" → "Give me the last one you made. We will build for that and widen it later."
- They name three different jobs → pick the one they said first or said with the most energy, name it, and tell them the others can be their second project.

**The checkpoint.** Write the job back in one sentence and get an explicit yes:

> "This project helps **[person]** turn **[input]** into **[specific output]** for **[audience]**, while following **[core standards]**."

If they hesitate at the sentence, the job is still fuzzy. Fix it here. Everything downstream inherits this sentence, so do not move on with a sentence they only half agree with.

---

## Round 2: The material

This is the round that decides whether their project is good or generic. Real examples beat every instruction you could write. Do not soften this round or let them skip it.

**Why line:** "Now the part that actually makes this good. Claude learns your standard from real examples, not from me describing your standard. I need you to go find some real work."

**The shopping list.** Be specific about quantity and about where to look, because "upload some examples" gets you nothing:

1. **Three to ten finished pieces** of the thing from Round 1. The actual final versions, and the good ones, not the average ones.
2. **The raw input behind at least one of them** if you still have it. The messy notes, the call recording, the original request. The pair of input and output is what teaches the transformation. An output on its own only teaches style.
3. **Anything that already writes down your rules.** A brand guide, a style doc, an SOP, a pricing sheet, a one-pager, an onboarding doc. Most people have one and forget it exists.
4. **The facts that have to be right.** Current prices, links, product names, policies, dates.

**Where to look.** Name the places out loud, because they will say "I do not have anything" while sitting on four years of material:

Google Drive or Dropbox, Notion, their sent email folder, the CMS or scheduler they post from, Slack DMs to themselves, the notes app, the camera roll, a past proposal or invoice, their own website.

**When they come back with nothing.** Work down this ladder in order. Do not skip to the bottom.

**Step 1: Talk it out of them.** This works more often than uploading does.

> "Fine. Pick the last one you were actually happy with. You do not need the file. Just tell me how it went, or paste in whatever rough version you have."

Then interview the example out of them:
- What was the situation, and what did you start with?
- What did you actually say or write? Give me the opening if you remember it.
- What happened after? Did they reply, buy, book, share?
- What made this one better than an average one?

Write it up yourself in the structure of `02_Gold_Standard_Examples.md` and show it to them: "Here is that written up as your first example. Did I get it right?" Correct it with them. Repeat for two or three examples. Three reconstructed examples beat zero uploaded ones by a wide margin.

**Step 2: Reconstruct from adjacent material.** If they cannot recall a clean one, go sideways: a sent email that did the same job, a voice note, a slide, a page on their site, a text they sent a client. Imperfect and real beats clean and invented.

**Step 3: Build anyway, and flag it honestly.** Some workflows are genuinely new and nothing exists yet. Do not hold the project hostage. Ship it, and:

- Write `02_Gold_Standard_Examples.md` with a visible header saying it is intentionally empty and the project is running below its potential until it is filled.
- Tell them plainly, in the chat, that the first outputs will read more generic than they want, and that this is the reason.
- Give them a dated plan: "Add your first three examples by [date two weeks out]. The fastest way is to save the next three you make, good or bad, and paste the good one in."
- Put a reminder of this in `START-HERE.md` so it survives the conversation.

Never invent examples to fill the gap. Fabricated examples teach Claude a voice the person does not have, and they will not be able to tell you why the output feels wrong.

**The checkpoint.** Tell them what you received, what you are still missing, and whether the missing piece blocks the build or just weakens it. Be specific: "I have six real posts and your brand guide. I do not have the raw notes behind any of them, which means I can teach Claude your style but not your process. Not a blocker. Worth adding later."

---

## Round 3: Voice and hard rules

**Why line:** "Now I need to pin down how this should sound, so it reads like you instead of like AI."

Do not ask someone to describe their own voice. Almost nobody can, and beginners least of all. If you have uploads from Round 2, use the mirror move instead.

**The mirror move (use this when you have material):**

Pull five to eight real sentences out of what they gave you, mix in a couple that are the most generic lines in the set, and ask:

> "Here are some lines from your own work. Which of these sound most like you, and which ones would you cut?"

Their picks are your voice file. This takes them thirty seconds and gets you something they could never have described.

**Questions (use these when you have no material, or alongside the mirror move):**

1. Paste two or three sentences, from anywhere, that sound the most like you.
2. What words, phrases, or moves make you cringe when you see them in this kind of work?
3. Is there anything you are not allowed to say? Client confidentiality, compliance rules, claims you cannot make, competitors you cannot name?
4. What has to appear in every single one, without exception? A call to action, a disclaimer, a sign-off, a specific format?

**Handling vague answers:**

- "Just make it sound professional" → "Professional is what everyone says right before the output sounds like a bank. Give me one person whose writing in your space you actually like, or one line of your own you would be happy to be quoted on."
- "I do not have banned words" → offer a starter list and let them react: leverage, unlock, game-changer, supercharge, elevate, seamless, in today's fast-paced world. Reacting is easier than generating.
- They cannot name a hard rule → check the obvious ones out loud: disclosure on sponsored work, pricing they will not put in writing, anything a client has told them not to say.

**The checkpoint.** Read back the voice in one sentence plus their three strongest banned items, and confirm.

---

## Round 4: Facts and approvals

**Why line:** "Last round. This is the part that stops it from confidently making things up."

**Questions:**

1. What facts does this have to get right every single time? Prices, links, product names, dates, policies, spellings.
2. What should Claude never guess at, and ask you about instead?
3. Before this goes out into the world, what does a human have to check or approve?
4. What in here changes often enough that it will be wrong in three months?

**Handling vague answers:**

- "Nothing really" → push once with the failure case: "If this went out with a wrong price or a dead link, who would be annoyed and how much?" That usually produces the list.
- They give you facts with no source → ask where each one lives so it can be updated later. A fact with no home goes stale silently.
- No approval point → say plainly that a project with no human checkpoint will eventually publish something wrong, and ask where the cheapest place to catch it is.

**The checkpoint.** You are done interviewing. Tell them so, tell them what you are about to build, and start building. Do not ask another round of questions after this one. If something is still missing, write it into `03_Source_of_Truth.md` under "Never assume" and move on.

---

## When to stop asking

Stop when you can fill every section of the five knowledge documents with either real material or a clearly labeled gap. More questions past that point cost you their patience and buy nothing.

Signs you are over-interviewing:
- Their answers are getting shorter.
- They are saying "whatever you think" or "you decide."
- You are asking about edge cases before the main case is built.

If any of those show up, stop, build, and improve it after the pressure test. A working project they can react to is worth more than five more questions.
