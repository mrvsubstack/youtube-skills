---
name: yt-title-optimizer
description: "Turns a video topic, a draft title or a finished video into 3 to 5 honest, high-click YouTube titles, each tagged with its formula, character count and job (browse or search), plus a pick for YouTube's Test & Compare. Use this skill whenever the user says things like \"give me title ideas for this video\", \"fix my YouTube title\", \"this title is boring\", \"what should I call this video\", \"title options for A/B testing\", \"make this title more clickable without clickbait\", \"title for my Short\". Not for the thumbnail (use yt-thumbnail-brief), the description (use yt-description-writer) or the spoken opening (use yt-hook-scripter)."
metadata:
  author: Mr V
  version: "1.0"
  group: YouTube
---

# YouTube Title Optimizer

You give it a topic, a rough title or a video that already exists. It hands back 3 to 5 titles that earn the click honestly, each labelled with the formula it uses, its character count and the job it does. You pick. YouTube's Test & Compare settles the argument.

---

## The core discovery: a title is a promise, not a label

Weak titles describe the video. Strong titles promise the viewer something they want and leave one question open.

**Label:** "My Editing Workflow 2026"
**Promise:** "I Cut My Editing Time From 9 Hours to 2"

Same video. The second names a result, carries a number and makes you wonder how. That is the whole skill: find the real payoff inside the video, then package it so the click feels obvious.

The catch: the promise has to be kept in the first 30 seconds. A title that overpromises gets the click and loses the viewer, and YouTube reads a fast exit as a bad video. Honest curiosity wins. Bait loses twice.

---

## Intake (ask before drafting)

1. **What happens in the video?** The real payoff in one sentence. Not the topic. The result.
2. **Who is it for?** Beginner, practitioner, buyer, fan.
3. **Long-form or Short?**
4. **Browse or search?** Is this a video people will type into the search bar ("how to set up OBS"), or one that has to win on the home feed?
5. **The search phrase**, if any.
6. **Numbers and proof** the video actually contains (time saved, money made, days taken).
7. **The thumbnail idea**, if one exists. Title and thumbnail split the work.

Defaults when the user skips: assume long-form, assume browse, ask once for a real number and drop the number if none exists. Never invent one.

---

## The seven title formulas

| Code | Formula | Shape | Best when |
|---|---|---|---|
| T1 | Curiosity Gap | Surprising result, hidden mechanism | The how is genuinely interesting |
| T2 | How I [Result] | First-person outcome + number + time | You have a real personal result |
| T3 | Transformation | Before → after over a timeframe | There is a visible arc |
| T4 | Mistake | The costly thing the viewer is doing wrong | The video corrects a common error |
| T5 | Number List | A finite, scannable payoff | The video is genuinely a list |
| T6 | Versus | Two named options in tension | Decision or comparison videos (search-friendly) |
| T7 | Their Story | A named person or type who went from zero to a big number | Case-study and interview videos |

In creator and business niches, T1, T2 and T3 tend to outperform. T5 and T6 do their best work in search. Verify current patterns in your own niche by looking at the top 20 results for your search phrase before trusting any table, including this one.

---

## Rules

1. **Promise, don't label.** Every title names a payoff or a tension.
   - Bad → "Notion Tutorial"
   - Good → "The Notion Setup That Replaced 4 Apps"
2. **Front-load the click.** The words that decide the click come first. Mobile cuts long titles, so aim for 40 to 60 characters and treat 100 as the hard ceiling.
   - Bad → "In This Video I Show You How I Grew to 10K Subscribers"
   - Good → "10K Subscribers in 6 Months: What Actually Worked"
3. **Curiosity plus a concrete noun.** Never pure mystery. Never a dry label.
   - Bad → "This Changes Everything"
   - Good → "This $12 Mic Beat My $400 Setup"
4. **One real number where the video earns it.** "In 28 days" beats "fast". If the video has no number, don't fake one.
5. **First person beats generic when the result is yours.** "How I" over "How to" when there is a real outcome behind it. Search videos are the exception: lead with the exact phrase people type.
6. **Title and thumbnail never say the same words.** The title carries the claim. The thumbnail carries the emotion, the result or the object. Write down the split every time.
7. **Clean typography.** No ALL CAPS sentences (one emphasised word is fine), 0 or 1 emoji, a colon instead of a dash.
8. **Scrub machine phrasing.** In a one-line title, a single "game-changer", "unlock", "ultimate guide" or "here's what nobody tells you" already reads as AI. Replace it with the specific thing.
9. **Always return at least 3 variants across at least 2 formulas.** Five rewordings of one idea is not a test.

---

## Modes

### Mode 1: Fresh titles
**When:** the video is planned or filmed and has no title yet.
**How:** run the intake, decide browse vs search, shortlist 2 to 3 formulas, draft 5 titles, run the rules, flag the lead.
**Example:** topic "I tested 5 AI note-takers on real client calls" → T6 "Otter vs Fireflies vs Granola: Which Got the Notes Right?" / T1 "One AI Note-Taker Missed Half the Call" / T2 "I Ran 5 AI Note-Takers on 20 Real Calls".

### Mode 2: Rescue an underperformer
**When:** a published video has low click-through.
**How:** ask for the current title, the impressions click-through rate from YouTube Studio and the thumbnail. Diagnose which rule the title breaks (usually rule 1 or 3), then write 3 replacements that change one big thing each. Swap one at a time so you know what moved the number.
**Example:** "My Morning Routine as a Freelancer" (label) → "The 90-Minute Morning That Doubled My Client Work" (promise + number).

### Mode 3: Shorts title
**When:** a Short needs a title.
**How:** Shorts titles get read less than long-form ones because the video autoplays. Keep it under 40 characters, make it describe the payoff so it works in search and on the Shorts shelf, and never repeat the on-screen text.

---

## Worked example

**Input:** "Video where I show how I plan a month of newsletter posts in one afternoon using Claude. I went from planning weekly to monthly. Audience: solo newsletter writers. Thumbnail: me with a wall calendar full of sticky notes."

**Output:**

| # | Title | Formula | Chars | Job |
|---|---|---|---|---|
| 1 | I Plan a Month of Newsletters in One Afternoon | T2 How I | 46 | Browse |
| 2 | The Claude Prompt That Plans My Whole Month | T1 Curiosity | 43 | Browse |
| 3 | Stop Planning Your Newsletter Every Week | T4 Mistake | 40 | Browse |
| 4 | How to Plan a Month of Newsletter Content With Claude | Search phrase | 53 | Search |

**Lead the Test & Compare with #1.** It names a result and a timeframe the video proves on screen.
**Thumbnail split:** the title carries "one afternoon". The thumbnail carries the full calendar and the relieved face. No words repeated.

---

## Output format

```
## Titles for: [video in one line]

Job: [browse / search]   Format: [long-form / Short]

| # | Title | Formula | Chars | Job |
|---|---|---|---|---|

Lead for Test & Compare: #[n], because [one line]
Thumbnail split: title carries [x], thumbnail should carry [y]
Promise check: the first 30 seconds must show [z]
```

---

## Sibling skills

- `yt-postiz-publisher` — schedule the finished post through Postiz after you approve it.
- `yt-thumbnail-brief`: the other half of the click. Build them as a pair.
- `yt-hook-scripter`: scripts the opening so the title's promise lands in the first 30 seconds.
- `yt-description-writer`: the description, chapters and search keywords.
- `yt-content-planner`: when you need titles planned across a whole month.

---

## Pre-flight checklist

- [ ] Every title promises a payoff or tension. None is a label.
- [ ] Click-deciding words come first. 40 to 60 characters where possible, never over 100.
- [ ] Every number is real and comes from the user.
- [ ] At least 3 variants across at least 2 formulas.
- [ ] Title and thumbnail split noted. No repeated words.
- [ ] No ALL CAPS sentences, at most 1 emoji, no AI phrasing.
- [ ] The first 30 seconds of the video can keep every promise made.
