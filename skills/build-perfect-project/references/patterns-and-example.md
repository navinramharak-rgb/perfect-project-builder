# Use-Case Patterns and a Fully Worked Example

## Patterns

Use these to move faster. Adapt them; never copy them blindly.

| Use case | Instructions should control | Context documents should prove |
|---|---|---|
| **Short-form content (Reels/TikTok/Shorts)** | Content pillars, hook-to-payoff flow, script and caption structure, platform CTA rules, approval process. | Top-performing posts, captions, audience comments, pillar notes, brand-deal terms, production references. |
| **Newsletter writing** | Recurring issue structure, topic filter, research-to-draft workflow, source-checking, subject-line options, final QA. | Past issues, audience positioning, issue analytics, sponsor rules, approved sources, voice examples. |
| **Outreach / pitching** | Personalization workflow, pitch structure, follow-up cadence, deliverable boundaries, rate and approval rules. | Past sent emails and replies, media kit, audience data, previous deliverables, prospect research, approved case studies. |
| **Proposals / estimates** | Discovery-to-draft workflow, scope language rules, pricing presentation, what requires human sign-off. | Won proposals, service descriptions, approved pricing, testimonials, objection answers. |
| **Support / voice-agent knowledge base** | Greeting, qualification flow, question handling, data collection, handoff conditions, escalation rules. | FAQs, service menu, policies, hours, real transcripts, objection handling, CRM field definitions. |
| **Research / briefing** | Source standards, summary structure, what counts as a claim vs. an inference, citation format. | Past briefs rated good, trusted source list, terminology glossary, decision-maker preferences. |

## Fully worked example: Short-Form Content Engine

This is the required level of specificity for every build. A creator who teaches business owners practical AI publishes three Reels a week and wants each raw idea turned into a filmable package.

### 1. Project Snapshot

| Item | Setup |
|---|---|
| **Project name** | Short-Form Content Engine |
| **One-line job** | Turn raw ideas, trends, and audience questions into filmable short-form content packages that teach business owners practical AI. |
| **Best for** | A creator publishing practical Instagram/TikTok content on a fixed weekly schedule. |
| **Primary output** | Reel package: hook options, spoken script with visual notes, on-screen text, caption, CTA. |
| **Inputs needed each time** | Topic, audience, desired outcome, raw notes or a trend link, any sponsor constraints. |
| **Human approval point** | Final claims, point of view, sponsorship language, on-camera delivery. |

### 2. Project Instructions — paste this into Claude

```markdown
## Role and outcome
You are a content strategist and scriptwriter. Turn raw ideas, viral formats, audience questions, and approved sponsor details into useful short-form content that teaches business owners how to use AI right now.

## Operating workflow
1. Identify the audience problem and the practical outcome before writing the hook.
2. If a viral reference is supplied, extract the format or insight. Never copy the creator's words or claim it as original research.
3. Write a three-beat opening: belief challenge → promise → relatability.
4. Build the middle around what to show, what to say, the exact steps, and any copy-paste prompt.
5. End with an action step, the approved CTA when relevant, and a bridge to the next piece of content.
6. For sponsored content, show the real use case first. Introduce the product naturally near the end.

## Voice and standards
- Direct, useful, conversational. Write like a real operator, not a social-media manager.
- Teach simple, no-code actions people can use immediately.
- Make the output specific enough to film from without guessing.
- If the caption uses a comment trigger, put that CTA at the start of the caption.

## Output format
Return, in order:
1. The content angle and why it matters.
2. Three hook options.
3. The spoken script with visual/demo notes.
4. On-screen text suggestions.
5. A caption with a clear CTA.
6. One copy-paste prompt when the topic requires it.

## What not to do
- Do not use generic hooks such as "Stop scrolling" or "You need to hear this."
- Do not write salesy sponsor copy or lead with the product.
- Do not make up performance claims, product features, or trend data.
- Do not use corporate filler, empty motivation, or excessive emojis.
- Do not turn every post into a tutorial when the strongest idea is a point of view or story.

## Quality check before sending
Confirm the piece has one clear promise, a usable action, natural language, and no unsupported claims.
```

### 3. Context documents

| File | Purpose | Put this inside |
|---|---|---|
| `00_Project_Brief.md` | Lock the content job. | Audience, content goal, platforms, content pillars, required output. |
| `01_Voice_and_Non_Negotiables.md` | Make scripts sound like the creator. | Ten approved phrases, ten banned phrases, CTA rules, sponsor rules, real writing samples. |
| `02_Gold_Standard_Examples.md` | Show formats that already work. | Ten top posts with hook, script, caption, format, topic, and why each performed. |
| `03_Source_of_Truth.md` | Prevent bad claims. | Approved offers, links, sponsor details, disclosure requirements, claims with last-checked dates. |
| `04_Workflow_and_QA.md` | The weekly loop. | Idea intake → package → review → film → post → best performer added back to examples. |
| `05_Audience_Questions.md` | Ground content in real needs. | Comments, DMs, sales-call questions, grouped by theme, in the audience's own words. |

### 4. Build order

1. Collect ten real posts, three transcripts, and twenty audience questions.
2. Create the voice file using exact sentences from approved content.
3. Add sponsor facts only after they are verified.
4. Paste the Instructions into the project.
5. Run the pressure test and improve the documents based on the failure.

### 5. Starter prompts

```markdown
Turn this raw thought into a Reel package for business owners: [paste thought]. The goal is [goal].
```

```markdown
This post format is working: [paste link or description]. Find the useful insight behind it, then create an original tutorial with a three-beat intro and a practical screen-share section.
```

```markdown
Review this draft against the project rules. Flag anything generic, salesy, unsupported, or hard to film. Then rewrite only what needs fixing.
```

### 6. Pressure test

**Test prompt:** "I want to teach business owners how to turn a messy meeting transcript into a follow-up plan with AI. Make it a 45-second Reel."

**A good answer must include:** a concrete hook, the screen-share sequence, the exact copy-paste prompt, a simple action step, and a caption that doesn't sound like a tutorial template.

**If it fails:** add real transcript-to-content examples and more audience language to the knowledge base.

### 7. What not to do

Don't load the project with generic social-media advice, duplicate conflicting brand guides, unverified sponsor claims, or random inspiration screenshots without a written note on what the project should learn from each one.
