---
name: yt-channel-optimizer
description: "Audits a YouTube channel page and rewrites what's failing: name and @handle, banner (with the mobile and TV safe area), profile picture, description and keywords, the trailer non-subscribers see, the featured video subscribers see, playlists and section order, watermark and links. Returns a 10-part scorecard, ranked fixes and before → after rewrites. Use this skill whenever the user says things like \"audit my YouTube channel\", \"optimize my channel page\", \"rewrite my channel description\", \"fix my banner\", \"what should my channel trailer be\", \"organise my playlists\", \"people watch but don't subscribe\". Not for individual video titles (use yt-title-optimizer) or thumbnails (use yt-thumbnail-brief)."
metadata:
  author: Mr V
  version: "1.0"
  group: YouTube
---

# YouTube Channel Optimizer

You give it your channel link or screenshots of your channel page, plus your goal. It hands back a scorecard of 10 parts, the fixes ranked by impact and a rewritten version of every part that fails.

---

## The core discovery: the channel page is a second chance at a subscriber

Someone watches one of your videos, likes it and taps your name. That visit is the most valuable moment you get. They're curious. They're deciding whether you're worth coming back to.

Most channel pages answer with a default banner, a random latest upload and a one-line description written three years ago. The visitor leaves.

**Default page:** banner with your name, "Uploads" as the only section, description: "Welcome to my channel! I make videos about tech."
**Working page:** banner reading "AI workflows for solo writers. New video every Thursday", a 60-second trailer, a "Start here" playlist on top, a description that tells them who it's for and what they get.

Same videos. Different decision.

**Two audiences, two first impressions.** Non-subscribers can be shown a channel trailer. Subscribers see a featured video. Audit both.

---

## Intake

1. **Channel link or @handle**, plus screenshots of the home tab signed out and signed in if possible (Claude may not be able to load the page directly).
2. **Goal:** subscribers, views, authority or sales/leads. The trailer, description and section order change by goal.
3. **Best videos** by views and watch time, to pick the trailer and featured video.
4. **Existing playlists.**
5. **The one link that matters** (newsletter, offer, site).

Verify current banner dimensions, description length and channel-feature availability on YouTube's help pages when web search is available. The figures below were standard at the time of writing.

---

## The 10-part scorecard

Score each Pass / Needs work / Fail.

| # | Part | Passes when |
|---|---|---|
| 1 | Name + @handle | Real name or brand, plus a searchable topic if it fits. Handle short, no stray numbers. |
| 2 | Banner | Value line + upload rhythm inside the centre safe area (about 1235×338 of a 2560×1440 canvas). High contrast. |
| 3 | Profile picture | Clear face or clean logo. Reads at the tiny circle size. |
| 4 | Description | First two lines carry who it's for and what they get. Real search phrases in sentences. Contact email. |
| 5 | Trailer | Set, 30 to 90 seconds, made for strangers, matched to the goal. |
| 6 | Featured video | Set for returning subscribers. Your best or most goal-relevant video. |
| 7 | Playlists | 3+ named playlists by topic or series. |
| 8 | Section order | Trailer/featured first, then the playlist that converts. Generic uploads lower down. |
| 9 | Watermark | Branded subscribe watermark set. |
| 10 | Links | One primary link matched to the goal. Extras only if they earn their place. |

---

## Rules

1. **Lead with the visitor's benefit, not your mission.**
   - Bad → "Hi, I'm Sam! I started this channel in 2021 because I'm passionate about productivity."
   - Good → "Weekly AI workflows for solo newsletter writers. Spend less time drafting and more time growing."
2. **The banner promise lives in the safe area.** Edges get cropped on phones and TVs. Name and value line go dead centre.
3. **The banner adds the rhythm.** "New video every Thursday" sets an expectation and makes a subscribe feel like a decision.
4. **The trailer is a pitch, not a highlight reel.** Who you are, what they get, why subscribe now. Under 90 seconds.
   - Bad → your most-viewed video set as the trailer.
   - Good → a 60-second "here's what this channel does for you" video.
5. **Playlists sell the channel at a glance.** Name them for outcomes ("Start here: AI writing basics"), not formats ("Videos 2024").
6. **Curated rows above "Uploads".** The visitor should see your best path, not your latest experiment.
7. **Keywords in sentences.** Never a comma-separated list in the description.
8. **One primary link.** A wall of links splits the click.
9. **Don't promise a cadence you can't hold.** If you upload every two weeks, say "every other Tuesday".

---

## Steps

1. **Intake** and confirm the goal.
2. **Score all 10 parts.**
3. **Rank fixes by impact.** Usual order: trailer → banner → description → section order → playlists → the rest.
4. **Rewrite each failing part.** Before → after for text. A brief for visuals (banner, profile picture). A script outline for the trailer.
5. **Pick the trailer and featured video** with one line of reasoning each.
6. **Run the one-visit test.** A stranger who arrives from one video sees the banner, trailer and first two description lines. Do they know what they'll get and want it? If not, fix again.

---

## Trailer outline (60 seconds)

```
0:00  The viewer's problem, in their words
0:08  Who you are, in one line, with one proof
0:15  What the channel delivers (2–3 specific video examples on screen)
0:40  The rhythm ("every Thursday")
0:50  The ask: subscribe, plus what they'll get next
```

---

## Worked example

**Input:** @samwritesai, 1,200 subscribers, goal = newsletter sign-ups. Banner shows "Sam Writes AI" over a stock photo. No trailer. Description: "Videos about AI and writing. Business: sam@..."

**Scorecard excerpt:**
- Banner: Fail. No value line, no rhythm, stock image.
- Trailer: Fail. Not set.
- Description: Fail. No benefit, no keywords.

**Rewrites:**
- Banner → "AI workflows for solo newsletter writers · New video every Thursday" centred, navy background, face on the right inside the safe area.
- Description → "Weekly AI workflows for people who write a newsletter alone. Learn how to plan, draft and grow faster with Claude and ChatGPT without losing your voice. Free prompt library → [newsletter link]. Business: sam@..."
- Trailer → record the 60-second outline above. Until then, set "My Claude setup for writing faster" (best watch time) as a stopgap.
- Section order → Trailer / "Start here" playlist / "Experiments" playlist / Popular uploads.

---

## Output format

```
## Channel audit: [@handle]
Goal: [ ]

### Scorecard
| # | Part | Score | Note |

### Top fixes (by impact)
1. ...

### Before → After
[part]: before / after

### Trailer + featured picks
### One-visit test: [pass / still failing because...]
```

---

## Sibling skills

- `yt-title-optimizer` and `yt-thumbnail-brief`: the video grid is part of the channel's first impression.
- `yt-content-planner`: the plan behind the rhythm the banner promises.
- `yt-description-writer`: per-video descriptions, a different job from the channel description.
- `yt-hook-scripter`: script the trailer's first seconds.

---

## Pre-flight checklist

- [ ] Both audiences audited: non-subscriber (trailer) and subscriber (featured).
- [ ] All 10 parts scored.
- [ ] Banner text inside the safe area. Dimensions verified or labelled.
- [ ] Description opens with the visitor's benefit. Keywords in sentences.
- [ ] One primary link matched to the goal.
- [ ] Every rhythm promised is one the user can hold.
- [ ] One-visit test run and reported.
