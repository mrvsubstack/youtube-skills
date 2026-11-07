---
name: yt-description-writer
description: "Writes a complete YouTube description: a first-150-character hook that works as the search snippet, a short body with the main keywords placed naturally, timestamped chapters, labelled links, one specific call to action and 3 to 5 hashtags, all under the 5,000-character limit. Covers long-form and Shorts. Use this skill whenever the user says things like \"write my YouTube description\", \"add chapters to this video\", \"SEO description for this upload\", \"timestamps from my transcript\", \"my description is just links\", \"what goes above show more\". Not for the title (use yt-title-optimizer) or the spoken opening (use yt-hook-scripter)."
metadata:
  author: Mr V
  version: "1.0"
  group: YouTube
---

# YouTube Description Writer

You give it the title, what the video covers, the search phrase and your links (a transcript is even better). It hands back a description ready to paste into YouTube Studio: a hook, a body, chapters, links, a call to action and hashtags.

---

## The core discovery: only 150 characters get read

Most people never tap "Show more". What they see is the first line or two, in search results, suggested videos and under the player. That snippet is a second hook.

**Wasted snippet:** "Hey guys! Thanks for watching. In today's video we're going to be talking about..."
**Working snippet:** "How I plan 12 newsletter issues in one afternoon with 4 Claude prompts, including the one that fixed my open rates."

Everything else in the description is furniture: useful, skimmable, but secondary. Write the first 150 characters like a title. Write the rest like a well-labelled filing cabinet.

---

## The three layers

| Layer | Length | Job |
|---|---|---|
| Hook | First ~150 characters | The snippet. Payoff + main search phrase. |
| Body | ~150 to 1,000 characters | Expand the promise. Place keywords naturally. Link the one key resource. |
| Furniture | The rest, under 5,000 total | Chapters, links, socials, CTA, hashtags. |

Limits change. Verify the current description limit and chapter rules on YouTube's help pages when web search is available, and say if you couldn't.

---

## Intake

1. **The title.** The description complements it, never repeats it word for word.
2. **The payoff.** What the viewer walks away with.
3. **Main search phrase** plus 3 to 5 related phrases. If the user has none, suggest phrases from what people actually type (YouTube's search autocomplete is a good source) and label them as suggestions.
4. **Chapter beats with timestamps**, or a transcript with timestamps to build them from.
5. **Links:** the main resource (lead magnet, newsletter, product), tools mentioned, socials. Each needs a label.
6. **Long-form or Short.**
7. **The reason to subscribe**, in one specific line ("new AI workflow every Thursday").

---

## Rules

1. **The first line is a hook, never a greeting.**
   - Bad → "Welcome back to the channel!"
   - Good → "The exact Notion template I use to plan a month of content, free below."
2. **The main search phrase appears once in the first 150 characters and once in the body.** Inside real sentences.
3. **Keywords live in sentences, never in a dump.**
   - Bad → "newsletter, newsletter tips, substack, substack growth, email marketing"
   - Good → "If you write on Substack and want steadier newsletter growth, this workflow..."
4. **The one link that matters goes in the body.** Not buried under 20 affiliate links.
5. **Chapters start at 0:00, there are at least 3, and labels are short and descriptive.** That's what switches on YouTube's chapter bar. Labels can carry search terms naturally ("Setting up the Claude project").
6. **Every link is labelled.** The reader knows where it goes before tapping.
   - Bad → "https://bit.ly/3xYz"
   - Good → "Free planning template → [url]"
7. **One specific call to action.** Not "smash that like button". A reason to subscribe tied to the channel's promise.
8. **3 to 5 hashtags at the very end.** The first few can show above the title. Piling on dozens makes YouTube ignore them.
9. **Never invent a number, result or quote.** Pull specifics from the user or the transcript only.
10. **Read the snippet cut off.** Check the first 150 characters still make sense when truncated mid-sentence.

---

## Building chapters from a transcript

1. Scan for topic shifts: new step, new question, new example, a "so" or "next" pivot.
2. Aim for one chapter every 1 to 3 minutes. A 12-minute video wants 5 to 8.
3. Name each chapter for what the viewer gets, not what you do ("Why most plans fail", not "Talking about plans").
4. First chapter is 0:00 and covers the opening.
5. Double-check every timestamp exists in the transcript. Never estimate.

---

## Modes

### Mode 1: Long-form
Full three layers with chapters. Target 600 to 1,500 characters for most videos. Longer only when links genuinely need it.

### Mode 2: Short
One hook line with the keyword, one or two lines of context, one labelled link if relevant, 2 to 3 hashtags. No chapters.

### Mode 3: Back-catalogue refresh
**When:** old videos have thin descriptions.
**How:** ask for the title, a rough outline or transcript and current links. Rewrite the hook and add chapters first, since those affect search and navigation most. Flag dead or outdated links for the user to check.

---

## Worked example

**Input:** Title "I Plan a Month of Newsletters in One Afternoon". Phrase: "newsletter content plan". Chapters: 0:00 intro, 1:10 reader problem prompt, 3:40 topic map, 6:20 calendar build, 9:05 the fix. Link: free template. CTA: new workflow every Thursday.

**Output:**

```
How I build a full newsletter content plan in one afternoon using 4 Claude prompts,
plus the step I almost skipped that fixed my open rates.

If you write a weekly newsletter and plan one issue at a time, you know the Tuesday panic.
This is the process I switched to: start from your reader's real problem, map topics that
connect, then build the calendar in Notion. By the end you'll have a month of issues that
read like a series, not a scramble.

Free newsletter planning template → [link]

CHAPTERS
0:00 Planning a month in one afternoon
1:10 Prompt 1: your reader's real problem
3:40 Prompt 2: the topic map
6:20 Building the calendar in Notion
9:05 The step that fixed my open rates

TOOLS IN THIS VIDEO
Claude → [link]
Notion → [link]

New AI workflow for writers every Thursday. Subscribe if that's your thing.

#newsletter #substack #contentplanning
```

---

## Output format

```
## Description: [title]
Characters: [total] / 5,000
Snippet check: [first 150 characters, marked with |]

[the description]

Notes: [any suggested keywords to confirm, links to verify, timestamps to double-check]
```

---

## Sibling skills

- `yt-postiz-publisher` — schedule the finished post through Postiz after you approve it.
- `yt-title-optimizer`: the title this description supports.
- `yt-hook-scripter`: the spoken opening, a different job from the written hook.
- `yt-content-planner`: keyword and link strategy across a whole series.
- `yt-repurposer`: turning a blog post or newsletter into a video brief that includes a description.

---

## Pre-flight checklist

- [ ] First 150 characters: hook + main phrase, no greeting, reads well cut off.
- [ ] Keywords in sentences, no dump.
- [ ] Main link in the body, labelled.
- [ ] Long-form: at least 3 chapters starting at 0:00, every timestamp real.
- [ ] One specific CTA. 3 to 5 hashtags at the end.
- [ ] Nothing invented. Under 5,000 characters.
