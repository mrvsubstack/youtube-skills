---
name: yt-hook-scripter
description: "Scripts the spoken opening that decides whether people keep watching: the first 30 seconds of a long-form YouTube video, beat by beat with timestamps, or the first 3 seconds of a Short plus a loop ending. Confirms the title's promise, opens a loop and makes a watch-contract with no greeting and no intro. Use this skill whenever the user says things like \"write my intro\", \"how should this video start\", \"script the first 30 seconds\", \"people leave in the first minute\", \"hook for my Short\", \"fix my cold open\", \"my retention drops at the start\". Not for the title (use yt-title-optimizer), the written description (use yt-description-writer) or the thumbnail (use yt-thumbnail-brief)."
metadata:
  author: Mr V
  version: "1.0"
  group: YouTube
---

# YouTube Hook Scripter

You give it the title, what the video delivers and its strongest moment. It hands back the words you say on camera for the opening: 30 seconds, beat by beat, for long-form, or a frame-one line plus a loop ending for a Short.

The title earns the click. The opening earns the watch.

---

## The core discovery: the viewer is asking "did I click the right thing?"

For the first ten seconds, a viewer isn't watching your video. They're checking whether it matches the title. Every second you spend on "hey guys, welcome back" is a second they spend doubting.

**Opening that loses them:** "Hey everyone, welcome back to the channel. Before we start, make sure you subscribe. So today I wanted to talk about..."
**Opening that keeps them:** "I let Claude write my newsletter for 30 days. Open rates held. But issue 19 lost me 212 subscribers in a day, and I'll show you exactly why."

The second one confirms the click, raises the stakes and promises a payoff. In 12 seconds.

---

## Intake

1. **The title** (the promise you must keep).
2. **The one payoff** of the video.
3. **The strongest moment or proof** available: a result, a clip, a before/after.
4. **Who is watching.**
5. **Long-form or Short.**
6. **Real specifics** you can say out loud: numbers, dates, names.

Never invent a specific. If the user has no number for a beat, ask once. If there's still nothing, drop the claim. A made-up number said on camera is permanent.

---

## The four opening shapes

| Code | Shape | Surface | Use when |
|---|---|---|---|
| H1 | Restate and Raise | Long-form | Curiosity titles. Say the promise, then make it bigger or harder. |
| H2 | Cold-Open Tease | Long-form | You have a strong result on film. Flash it, then cut back to the start. |
| H3 | Question and Contract | Long-form | Search and how-to videos. Answer fast, then open a deeper question. |
| H4 | Frame-One Hook | Short | Payoff or tension on screen in second one, with a loop at the end. |

Pairing rule: a "How I" title pairs with H2. A curiosity-gap title pairs with H1. A search-phrase title pairs with H3.

---

## Long-form: the 30-second map

| Time | Beat | Job |
|---|---|---|
| 0:00–0:03 | Cold line or clip | The promise or the peak moment. No greeting. |
| 0:03–0:10 | Restate | Say what the title promised, in your own words. |
| 0:10–0:18 | Raise | The obstacle, surprise or cost. This opens the loop. |
| 0:18–0:28 | Contract | "By the end, you'll have..." plus a bonus if real. |
| 0:28–0:30 | Pivot | Hard cut into section one. |

## Short: the 3-second map

| Time | Beat | Job |
|---|---|---|
| 0:00–0:01 | Frame one | The most arresting line or visual, with on-screen text so it works muted. |
| 0:01–0:03 | Stakes | One line that makes them need the end. |
| Middle | Deliver | No filler. |
| End | Loop line | The last line flows straight back into the first. |

---

## Rules

1. **No greeting, logo or intro animation before the hook.** Ever.
   - Bad → "What's up everyone, it's Sam."
   - Good → "This $40 light made my $2,000 camera look cheap."
2. **Restate the promise by 0:10.** The viewer needs confirmation they're in the right place.
3. **Open a loop by 0:18.** An unanswered question, a tease, an unresolved stake.
   - Bad → "I'll go through my whole process."
   - Good → "Step three is the one that almost made me quit."
4. **Show proof early when you have it.** A result on screen in the first 10 seconds beats any claim.
5. **Never tease what isn't in the video.** A cold open from a moment that doesn't exist is a broken promise, and the retention graph punishes it.
6. **No subscribe ask in the first 30 seconds.** Earn it first.
7. **Write it to be said.** Short spoken sentences. Use ".." for a pause on the teleprompter. Read it aloud once before delivering.
8. **No staged rhythm.** No "No fluff. No filler. Just results." No "The result? Chaos." No "let me be honest" with nothing honest after it. These read as scripted.
9. **Re-hook at every section break.** One line teasing what's next ("the third one moved the numbers most") keeps the curve flat after the opening.

---

## Modes

### Mode 1: Fresh opening
**When:** the video isn't filmed yet.
**How:** intake, pick a shape, write the beats with timestamps, mark B-roll and on-screen text.

### Mode 2: Retention rescue
**When:** a published video drops hard in the first minute.
**How:** ask for the transcript of the first 60 seconds and the retention graph shape (where the drop happens). Match the failure to the fix:

| Failure | Fix |
|---|---|
| Greeting first | Cut it. Open on the promise. |
| Promise never restated | Add a restate line by 0:10. |
| No loop | Add a tease or unresolved stake by 0:18. |
| Overpromised | Soften the open to what the video truly delivers. |
| Slow Short | Move the payoff to frame one with on-screen text. |

Then rewrite the opening, ideally as a re-edit of existing footage plus a short pickup line.

### Mode 3: Shorts hook + loop
**When:** a Short needs its first 3 seconds and its ending.
**How:** write the frame-one line and on-screen text, then a final line that implies the first. Loops count as rewatches.

---

## Worked example

**Input:** Title "I Plan a Month of Newsletters in One Afternoon". Payoff: a 4-step Claude process. Proof: a filled Notion calendar. Viewer: solo newsletter writers.

**Output (H2 Cold-Open Tease):**

```
0:00  [B-roll: Notion calendar scrolling, 12 issues filled]
      "That's every newsletter I'm sending in March. I planned it on a Sunday afternoon."
0:05  "I used to do this every single week. Sit down Tuesday, stare at a blank page, panic."
0:11  "The problem wasn't ideas. It was that I planned one issue at a time,
       so nothing connected.. and readers could tell."
0:18  "By the end of this video you'll have the 4 prompts I run in Claude,
       in order, and the one I almost skipped that fixed the whole month."
0:27  [Hard cut] "Prompt one. Your reader's actual problem."
```

Why it holds: proof on screen at 0:00, promise restated by 0:05, stakes by 0:11, contract plus loop ("the one I almost skipped") by 0:18.

---

## Output format

```
## Opening script: [title]
Shape: [H1–H4]   Surface: [long-form / Short]

[timestamped beats with stage directions in brackets]

Promise kept: [what the title promised → where the script confirms it]
Loop opened: [the line] → paid off at: [section/time]
```

---

## Sibling skills

- `yt-title-optimizer`: the promise this opening has to keep.
- `yt-thumbnail-brief`: the emotion the first frame should match.
- `yt-description-writer`: the written hook under the video (a different job).
- `yt-repurposer`: when the opening is coming from a blog post or thread you already wrote.

---

## Pre-flight checklist

- [ ] No greeting, logo or subscribe ask before the value.
- [ ] Promise restated by 0:10 (long-form) or on frame one (Short).
- [ ] A loop is open by 0:18, and it's paid off later in the video.
- [ ] Every number and name came from the user.
- [ ] Nothing teased that isn't in the video.
- [ ] Reads naturally aloud. No staged staccato or announced honesty.
- [ ] Shorts: on-screen text on frame one and a loop ending.
