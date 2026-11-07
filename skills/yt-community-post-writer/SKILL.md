---
name: yt-community-post-writer
description: "Writes YouTube community posts (the Posts tab): text updates, polls, image posts and question prompts that keep subscribers warm between uploads, seed comments and set up the next video. Each post has one hook line, one ask and a clear job. Returns copy-paste posts plus a suggested weekly rhythm. Use this skill whenever the user says things like \"write a community post\", \"make a poll for my channel\", \"what should I post between videos\", \"tease my next video\", \"YouTube post ideas\", \"get more comments on my channel\". Not for video titles or descriptions (use yt-title-optimizer or yt-description-writer)."
metadata:
  author: Mr V
  version: "1.0"
  group: YouTube
---

# YouTube Community Post Writer

You tell it what's happening on your channel (a video coming, a video just out, a question you have for your audience). It hands back short, finished community posts and polls you paste into the Posts tab yourself.

Posts are published by hand in YouTube Studio or the app. That's normal.

---

## The core discovery: a community post is a nudge, not a publication

The Posts tab shows up in subscribers' feeds as a small card between videos. People give it two seconds. A post that reads like a blog gets skipped. A post with one line and one easy action gets answered.

**Skipped:** a 200-word update about your month, your plans, three questions and a link.
**Answered:** "Filming the Claude vs ChatGPT video tomorrow. Which one do you think wins for newsletter drafts?" + a two-option poll.

One hook. One ask. Done. And every answer is a signal that tells YouTube your subscribers still care, which helps the next upload start stronger.

Feature availability and eligibility for posts have changed over time. If the user can't see a Posts tab, tell them to check YouTube's current help page on community posts.

---

## Intake

1. **Goal of this post** (decides the format):
   - tease a video → text or image teaser with a gap
   - get ideas or settle a debate → poll
   - follow up on a video → text post answering top comments
   - keep warm → behind-the-scenes image or quick question
2. **The video it relates to**, if any.
3. **Your channel voice.** Paste 2 or 3 past posts or comments you've written if you want it matched.
4. **Real details** you can share: dates, numbers, what you're filming.

Never invent a detail. If the post needs a number you haven't given, ask once or write around it.

---

## The four post types

| Type | Best for | Shape |
|---|---|---|
| Text update | Teases, notes, follow-ups | Hook line / one line of context / one ask |
| Poll | Ideas, debates, low-effort engagement | One clear question / 2–4 options |
| Image post | Teaser frames, before/after, results | Image stops the scroll / caption frames it |
| Question prompt | Filling the comments | One specific, answerable question |

---

## Rules

1. **The first line carries the post.** Long posts get cut off in the feed.
   - Bad → "Hey everyone! Hope you're all having a great week. So I've been thinking..."
   - Good → "The next video almost didn't happen."
2. **One ask per post.** Vote, comment one specific thing or watch one video. Two asks split the response.
3. **Specific questions beat open ones.**
   - Bad → "What do you think?"
   - Good → "What's the one part of writing a newsletter you'd hand to AI tomorrow?"
4. **Polls: 2 to 4 options, mutually exclusive, no loaded framing.**
   - Bad → "Is AI writing good or is it soulless garbage?"
   - Good → "Would you let AI write your first draft? / Yes, every time / Sometimes / Never"
5. **No engagement bait.** "Comment 1 if you agree" trains people to ignore you. Ask a real question.
6. **Sound like you, not a brand account.** Lowercase openers and short sentences are fine if that's your voice.
7. **Close the loop.** When you use a poll result or a comment in a video, say so in a follow-up post. People answer more when they see answers used.
8. **Don't over-post.** 2 to 4 posts a week is plenty. Daily filler teaches subscribers to scroll past.

---

## Weekly rhythm (for a once-a-week uploader)

| Day | Post |
|---|---|
| 2 days before upload | Poll or question tied to the next video |
| Upload day | No post (the video is the post) |
| 1–2 days after | Follow-up: answer the best comment, or share a result |
| Mid-gap | Behind-the-scenes image or standalone question |

Tie roughly half the posts to a video. Let the rest stand alone.

---

## Modes

### Mode 1: Single post
**When:** the user needs one post now.
**How:** confirm the goal, pick the type, draft 2 variants, run the rules.

### Mode 2: A week of posts
**When:** the user wants posts planned around an upload.
**How:** use the weekly rhythm table, draft each post, note the day.

### Mode 3: Comment follow-up
**When:** a video got good comments.
**How:** ask the user to paste the top 5 to 10 comments. Pick the one with the most useful question or strongest opinion. Write a post that quotes it (first name or handle only, with the user's OK) and answers it in two lines, or turns it into the next poll.

---

## Worked example

**Input:** "New video Thursday: I let Claude run my newsletter for 30 days. Want to tease it and get comments."

**Tuesday poll:**
```
Thursday's video: I handed my newsletter to Claude for 30 days.

Guess what happened to my open rate?
- Went up
- Stayed the same
- Dropped
- I'd never risk it
```

**Saturday follow-up:**
```
62% of you guessed "dropped".

It didn't. But issue 19 lost 212 subscribers in a day, and that's the part most of you are asking about in the comments.

What should I test next: voice-matching or subject lines?
```
(The 62% and 212 come from the user's real poll result and data. Never guess them.)

---

## Output format

```
## Community posts: [channel / video]

### Post 1 — [type] — [day]
[copy-paste text]
[poll options, if any]
Job: [tease / ideas / follow-up / warm]

### Post 2 ...
```

---

## Sibling skills

- `yt-content-planner`: places community posts on non-upload days across the month.
- `yt-title-optimizer`: when the post is teasing a specific video's title.
- `yt-repurposer`: turn a LinkedIn post, thread or newsletter into a community post.

---

## Pre-flight checklist

- [ ] The first line works alone.
- [ ] Exactly one ask.
- [ ] Polls have 2 to 4 fair, non-overlapping options.
- [ ] No engagement bait.
- [ ] Every number and detail came from the user.
- [ ] Short enough to read in two seconds.
