---
name: yt-content-planner
description: "Builds a YouTube content plan from your niche, audience and capacity: 3 to 5 pillars, a long-form and Shorts mix you can actually hold, and video ideas sorted into search videos (people type them) and browse videos (the feed serves them), each slot pre-paired with a title angle, thumbnail angle, opening shape and goal. Use this skill whenever the user says things like \"plan my YouTube content\", \"give me video ideas\", \"build me a YouTube calendar\", \"what should I upload next\", \"how many Shorts should I post\", \"I keep running out of video ideas\", \"plan a month of videos\". Not for writing one title, description or hook (use yt-title-optimizer, yt-description-writer or yt-hook-scripter)."
metadata:
  author: Mr V
  version: "1.0"
  group: YouTube
---

# YouTube Content Planner

You give it your niche, your viewer, how many videos you can really make and what's worked so far. It hands back a plan: pillars, a weekly rhythm, and a list of video ideas each sorted by how people will find it and pre-paired with packaging.

It plans. The other YouTube skills write each piece.

---

## The core discovery: every video is either found or served

There are two ways a viewer reaches a video.

- **Search videos** get found. Someone types "how to set up ConvertKit" and your video answers. They grow slowly, then keep pulling views for years.
- **Browse videos** get served. YouTube shows them on the home feed and next to other videos because people click and stay. They spike, then fade.

Most channels plan by topic and never ask which kind they're making. So they write a search video with a curiosity title nobody types, or a browse video with a dry title nobody clicks.

**Topic-only plan:** "Week 3: Notion video."
**Mapped plan:** "Week 3: 'How to build a content calendar in Notion' (search, steady). Week 4: 'I deleted Notion after 4 years' (browse, spike)."

A healthy channel mixes both. Search builds the floor. Browse raises the ceiling.

---

## Intake

1. **Niche and viewer.** Who watches and what they're trying to do.
2. **Capacity.** Long-form videos and Shorts per week you can hold for 12 weeks. Be honest.
3. **Stage.** Rough subscriber count and how long you've been posting.
4. **What's worked.** Paste your top 5 and bottom 5 videos by views or watch time, if you have them.
5. **Goal.** Subscribers, watch time, leads for an offer or newsletter, or sales.
6. **Your edge.** What can you show that others can't (access, results, a skill)?

Defaults: 1 long-form plus 3 Shorts a week, goal = subscribers.

---

## Step 1: Pick 3 to 5 pillars

A pillar is a recurring lane the channel owns. Fewer than 3 feels thin. More than 5 and nobody can predict what you make.

Find them where four things overlap:

| Filter | Question |
|---|---|
| Expertise | What can you teach that most viewers can't? |
| Demand | What do people search for and click in this niche? |
| Edge | What angle is yours alone? |
| Stamina | What could you make every week for a year? |

---

## Step 2: Set the mix

| Stage | Weekly starting point |
|---|---|
| New (under ~1k subscribers) | 1 long-form + 4 to 5 Shorts |
| Growing (~1k to 50k) | 1 long-form + 3 Shorts |
| Established (50k+) | 1 to 2 long-form + 2 to 3 Shorts |

These are starting points, not rules. The real rule: a cadence you can hold for 12 weeks beats an ambitious one you drop in week 3.

Shorts bring new people in. Long-form keeps them. Every Short needs a link to the long-form library: an excerpt, a standalone tip from the same pillar, or a tease of the next upload. A Short with no through-line earns views that never become watch time.

---

## Step 3: Generate ideas, then sort them

For each pillar, generate ideas from these sources:

1. **Search demand.** Type the pillar into YouTube search and note the autocomplete phrases. If web search is available, check what already ranks. Label anything you couldn't check.
2. **Your comments.** Questions viewers keep asking.
3. **Your winners.** A sequel, a deeper cut or the opposite angle of your best video.
4. **Competitor gaps.** Popular videos in the niche that are outdated or shallow.
5. **Your edge.** Experiments only you can run.

Then tag each idea:

| Tag | Means | Title leans |
|---|---|---|
| S (search) | People type this phrase | The exact phrase, plainly |
| B (browse) | Wins on curiosity and emotion | Promise + tension |
| S+B | Both (rare, valuable) | Phrase + a twist |

Aim for roughly 40% search, 60% browse for a growing channel. Shift toward search if views are spiky and unreliable. Shift toward browse if growth has stalled on a solid library.

---

## Step 4: Pair every slot

No naked "post a video" slots. Each one gets:

- format (long-form / Short)
- pillar
- S / B tag
- title angle (formula code from `yt-title-optimizer`: T1 curiosity, T2 how I, T3 transformation, T4 mistake, T5 list, T6 versus, T7 their story)
- thumbnail angle (what it carries that the title doesn't)
- opening shape (H1 to H4 from `yt-hook-scripter`)
- goal (clicks, watch time or subscribes)
- the Short that points at it

---

## Step 5: Balance check

- [ ] No pillar takes more than half the month.
- [ ] Both search and browse ideas are in the mix.
- [ ] Every week has at least one watch-time video and one subscribe-driver.
- [ ] Every Short points somewhere.
- [ ] The cadence matches stated capacity.
- [ ] Community posts on non-upload days (hand to `yt-community-post-writer`).

Measure long-form watch time and returning viewers separately from Shorts views. Shorts reach can make a stalled channel look like it's growing.

---

## Worked example

**Input:** Niche: AI for solo newsletter writers. Capacity: 1 long-form + 3 Shorts. ~800 subscribers. Best video: "My Claude setup for writing faster".

**Pillars:** AI writing workflows / Newsletter growth / Tool teardowns / Experiments.

| Week | Format | Pillar | Idea | Tag | Title angle | Goal |
|---|---|---|---|---|---|---|
| 1 | Long | Workflows | How to make Claude write in your voice | S | Search phrase | Watch time |
| 1 | Short | Workflows | The one line I add to every prompt | B | T1 | Clicks → wk 1 video |
| 2 | Long | Experiments | I let Claude run my newsletter for 30 days | B | T2 | Subscribes |
| 2 | Short | Experiments | Day 19 went badly wrong | B | T1 | Clicks → wk 2 video |
| 3 | Long | Teardowns | Claude vs ChatGPT for newsletter drafts | S+B | T6 | Watch time |
| 4 | Long | Growth | How I got my first 1,000 subscribers | S+B | T2 | Subscribes |

---

## Output format

```
## YouTube plan: [channel] — [month]

Pillars: [list with one-line description each]
Rhythm: [long-form / Shorts per week]
Search/browse split: [x% / y%]

| Week | Format | Pillar | Idea | Tag | Title angle | Thumbnail angle | Opening | Goal | Points to |

Balance check: [pass/fail per item]
Next: send each slot to yt-title-optimizer, yt-thumbnail-brief, yt-hook-scripter, yt-description-writer.
```

---

## Sibling skills

- `yt-title-optimizer`, `yt-thumbnail-brief`, `yt-hook-scripter`, `yt-description-writer`: write each planned slot.
- `yt-community-post-writer`: posts for the days between uploads.
- `yt-repurposer`: turn newsletters and posts you already have into video ideas for the plan.

---

## Pre-flight checklist

- [ ] 3 to 5 pillars that pass all four filters.
- [ ] A cadence the user confirmed they can hold.
- [ ] Every idea tagged search, browse or both.
- [ ] Every slot fully paired. No naked slots.
- [ ] Balance check run and reported.
- [ ] Search demand checked or labelled "unverified".
