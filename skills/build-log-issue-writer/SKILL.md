---
name: build-log-issue-writer
description: Turn build notes into a site teardown, a newsletter issue and a week of social posts in one pass, in a plain, unhedged voice with the failures left in
category: Content & publishing
---

# Build Log issue writer

Use this when the user has notes, a transcript, a repo or a chat log from something they built and wants it published. One input, four outputs: the long post, the email issue, the X posts, the LinkedIn post (drafted, never posted by the machine).

## 1. Intake

Before writing, extract from the material and list back:
- What was built, in one sentence a non-technical reader understands.
- What it replaced (a tool, a habit, a person's time).
- The stack, as names only.
- Three things that broke, with the cause of each.
- One constraint the user gave that got misread or over-applied.
- What it costs to run, only if the material states it.
- What the user would tell someone else to do first.

If any of these is missing, ask for it in one message. Do not write around a gap.

## 2. Voice rules

- Short paragraphs. One idea each.
- No hedging: no "may", "might be worth", "it depends". Say the thing.
- No em dashes. Use commas, full stops or brackets.
- No invented numbers. If there is no figure, describe the effect instead.
- Failures stay in. They are the point.
- No emojis, no hashtags, no "excited to share".
- Never name the user's employer.
- Health and money specifics stay out unless the user put them in the notes for publication.

## 3. The long post (site)

Structure it so it does not read like the last one. Pick a different opening device each time and say which you picked:
- Start with the output (a memo, a message, a screenshot described in words), then dig down.
- Start with the failure, then rebuild.
- Start with the constraint that got misread.
- Start with a timeline of one day.

Then: what it does, what broke, one transferable lesson, what to build first. 900 to 1,400 words. Add one diagram spec if a picture explains the mechanism better than prose: describe boxes, arrows and labels so it can be drawn as SVG.

Front matter: title, slug, issue number, date, draft: true, summary (one sentence), image placeholder.

## 4. The newsletter issue

- Opening line ties it to last week's issue in one sentence.
- Body is the long post, trimmed to the parts that matter in an inbox: cut the diagram, keep the failure and the lesson.
- Close with "Next week:" and one line, then "Reply to this email if..." with a specific ask.
- Subject line under 50 characters, no clickbait. Preview text is the summary.

## 5. Social posts

- Three X posts under 280 characters each: the reframe, the failure, the checklist or link. Link is the last line.
- One LinkedIn post: hook line, three short paragraphs, one question at the end, link as the last line. Mark it "for the user to post".
- No first-comment tricks. Links in the body.

## 6. Output order

Return: intake summary, long post, newsletter issue, X posts, LinkedIn post. Put the opening device you chose in one line at the top.
