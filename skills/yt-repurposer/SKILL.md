---
name: yt-repurposer
description: "Works both ways around a YouTube video. Out: turns a video or its transcript into Shorts (with timestamps and frame-one hooks), a newsletter issue, a LinkedIn or X post and a community post. In: turns a blog post, newsletter or thread into a video brief (title options, opening script, chapter outline). Keeps the core claim and real numbers, rebuilds the delivery for each platform. Use this skill whenever the user says things like \"turn this video into Shorts\", \"repurpose my YouTube video\", \"make a newsletter from this video\", \"clip ideas from my transcript\", \"turn my blog post into a video\", \"get more out of this upload\". Not for a fresh title (use yt-title-optimizer) or a blank-page community post (use yt-community-post-writer)."
metadata:
  author: Mr V
  version: "1.0"
  group: YouTube
---

# YouTube Repurposer

You give it a video transcript (or the video link and its timestamps) and say where you want it to go. It hands back finished pieces for each platform: Shorts with exact timestamps, a newsletter issue, social posts and a community post. Or you give it something written and it hands back a video brief.

---

## The core discovery: keep the spine, rebuild the skin

Every good video has a spine: one claim, one story or one number that made it worth making. Everything else is delivery for that platform.

Bad repurposing keeps the words and loses the point. It pastes a transcript paragraph into LinkedIn and wonders why nobody reacts.

**Copied:** "So in today's video I wanted to walk you through my process for planning content, which has three main steps..."
**Rebuilt:** "I used to plan my newsletter every Tuesday. Now I plan a whole month on one Sunday afternoon. Here are the 4 prompts."

Same spine. A skin that fits the feed.

---

## Intake

1. **The source.** A transcript with timestamps is best. YouTube Studio can export captions, or the user can paste the auto-transcript. A link alone isn't enough, because Claude may not be able to watch the video.
2. **Direction.** Video out to other formats, or written content into a video brief.
3. **Targets.** Which outputs: Shorts, newsletter, LinkedIn, X, community post, all.
4. **Goal.** Drive views back to the video, grow the newsletter, or stand alone.
5. **Voice samples** for each platform, if the user has them.

---

## Step 1: Find the spine and the clips

Read the whole transcript, then list:

- **The spine:** the single claim worth keeping, in one sentence.
- **Clip moments:** 3 to 6 stretches of 15 to 60 seconds that make sense alone. Look for:
  - a strong opinion said plainly
  - a number that surprises
  - a before/after or a reveal
  - a mistake and its fix
  - a quotable line
- **Proof:** every real number, name and result in the video.

Every timestamp must come from the transcript. Never estimate.

---

## Step 2: Rebuild for each target

### Shorts (vertical clips)
- Start the clip on the strongest line, not where the sentence technically starts. Cut the wind-up.
- Write the frame-one on-screen text (works muted).
- Write a loop ending: the last line flows back into the first.
- Add the through-line: on-screen "Full video on the channel" or a related-video link.
- Output: start time, end time, frame-one text, loop note, Short title.

### Newsletter issue
- Open with the spine as a personal story or claim, not "I made a video".
- Turn the video's steps into skimmable sections with one takeaway each.
- Add something the video didn't have (a template, a lesson learned after publishing, a reader question). Give subscribers a reason to read even if they watched.
- Link the video once, near the top or end, with a reason to watch ("the demo is easier to see than read").

### LinkedIn / X post
- Lead with the spine as a standalone line. No "new video!" opener.
- One idea. Line breaks as beats.
- Video link in the comments or at the end, depending on what the user's platform favours. Say that link handling varies and is worth testing.

### Community post
- Hand the format to `yt-community-post-writer` rules: one hook line, one ask.

---

## Step 3: Written content → video brief (the reverse direction)

1. **Spine:** the single most quotable claim in the piece.
2. **Format:** a listicle or step-by-step piece becomes a long-form video with one chapter per item. A hot take becomes a Short or a community poll.
3. **Title:** 3 options using `yt-title-optimizer` formulas.
4. **Opening:** a 30-second script using `yt-hook-scripter` beats.
5. **Chapters:** one per section of the original, renamed for the viewer's payoff.
6. **What the video adds:** a demo, a screen recording, a face. If the video adds nothing the post didn't have, it may not deserve to exist.

---

## Rules

1. **The claim and the numbers never change.** Repurposing changes the delivery, never the meaning.
2. **Lead with the payoff on every platform.**
   - Bad → "In this video I'm going to show you..."
   - Good → "The prompt that saved me 6 hours a week."
3. **Strip the source's artefacts.** No "link in bio" on YouTube, no "as I said in the video" in a newsletter, no "1/" thread numbering anywhere else, no hashtag walls.
4. **Each piece must stand alone.** Someone who never sees the video should still get value.
5. **One natural mention of your offer, at most.** Repurposed pieces aren't ads.
6. **Never invent clips, quotes or results.** If it isn't in the transcript, it isn't in the output.

---

## Worked example

**Input:** 14-minute transcript, "I let Claude run my newsletter for 30 days". Targets: Shorts, newsletter, LinkedIn.

**Spine:** AI kept my open rate steady but lost subscribers when it tried to be funny.

**Shorts:**
| # | Start–End | Frame-one text | Hook line | Loop note |
|---|---|---|---|---|
| 1 | 6:42–7:20 | "Day 19 went wrong" | "212 people unsubscribed in one day." | Ends on "and that's why" → loops to "212" |
| 2 | 2:05–2:48 | "The one rule I gave it" | "I gave Claude one rule for my voice." | Ends on the rule → loops to "one rule" |

**LinkedIn opener:** "I let AI write my newsletter for 30 days. My open rate didn't move. Then it tried a joke."

**Newsletter:** subject "The joke that cost me 212 subscribers", 4 sections (setup / what held / what broke / the rule I'd add now), video linked under section 3.

---

## Output format

```
## Repurpose plan: [source title]
Spine: [one sentence]

### Shorts
[table: start–end, frame-one text, hook, loop, Short title]

### Newsletter
[subject line options + full draft]

### LinkedIn / X
[draft(s)]

### Community post
[draft]

Proof used: [list of numbers/names, each with its transcript timestamp]
```

---

## Sibling skills

- `yt-postiz-publisher` — schedule the finished post through Postiz after you approve it.
- `yt-title-optimizer`, `yt-hook-scripter`, `yt-description-writer`: polish each part of a video brief.
- `yt-community-post-writer`: write the community post from scratch.
- `yt-content-planner`: place repurposed Shorts in the weekly rhythm.
- The LinkedIn, X and Substack skills in this library: final polish for each platform.

---

## Pre-flight checklist

- [ ] The spine is written in one sentence.
- [ ] Every timestamp and number comes from the transcript.
- [ ] Every piece leads with the payoff and stands alone.
- [ ] Source artefacts stripped.
- [ ] Shorts have frame-one text and a loop.
- [ ] The newsletter adds something the video didn't.
