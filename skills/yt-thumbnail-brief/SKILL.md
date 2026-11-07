---
name: yt-thumbnail-brief
description: "Turns a video idea and its title into a designer-ready thumbnail brief: one focal subject, a face and a named emotion (or the hero object), 4 words of overlay text or fewer that never repeat the title, contrast, composition and a phone-size read test, delivered as 2 to 3 concepts for YouTube's Test & Compare. Use this skill whenever the user says things like \"what should my thumbnail be\", \"write a thumbnail brief\", \"thumbnail ideas for this video\", \"brief for my designer\", \"prompt for a thumbnail image\", \"my thumbnail isn't getting clicks\", \"A/B thumbnail concepts\". Not for the title words (use yt-title-optimizer) or for designing the image itself (hand the brief to youtube-thumbnail-design or your designer)."
metadata:
  author: Mr V
  version: "1.0"
  group: YouTube
---

# YouTube Thumbnail Brief

You give it the title, what happens in the video and what assets you have (your face, a screen, a product). It hands back 2 to 3 thumbnail concepts, each a brief a designer or an image tool can execute without asking you a single question.

This skill writes words, not pixels. The brief is the deliverable.

---

## The core discovery: the thumbnail finishes the title's sentence

The title and the thumbnail are read together in under a second. When they say the same thing, you've wasted half your packaging.

**Wasted:** title "I Quit My Job to Freelance", thumbnail text "I QUIT MY JOB".
**Split:** title "I Quit My Job to Freelance", thumbnail shows a bank app reading £0.00 and your face mid-wince. Text: "MONTH 1".

The title makes the claim. The thumbnail adds the emotion, the stakes or the proof. Together they tell a story neither tells alone. Every concept in this skill starts by writing that split down.

---

## Intake

1. **The title** (final or working). If there isn't one, run `yt-title-optimizer` first or draft both together.
2. **The payoff and the tone.** What does the viewer get, and how should it feel (relief, shock, curiosity, calm)?
3. **Assets.** Can you appear on camera? Is there a screen, product, result or location worth showing?
4. **The single most visual moment** in the video.
5. **Your channel look.** Colours, fonts or a recurring style, if any.
6. **Long-form or Short.** Shorts thumbnails show far less often. Brief them lightly.

Default if no face is available: build around the object or the result. Never fake a moment that isn't in the video.

---

## The five non-negotiables

1. **One focal point.** One face or one object owns the frame.
   - Bad → you, a laptop, three logos and a graph.
   - Good → your face on the right third, one glowing graph line behind you.
2. **A real, readable emotion.** If there is a face, name the emotion (dread, delight, disbelief, focus) and make sure the video earns it.
   - Bad → shocked face on a calm tutorial.
   - Good → quiet satisfied grin on a "finally fixed it" video.
3. **High contrast and separation.** The subject pops from the background. Pick a colour your niche feed isn't already drowning in.
4. **Four words or fewer, never the title's words.** No punctuation, no full sentences.
   - Bad → "HOW I GREW MY NEWSLETTER FAST!"
   - Good → "0 → 5,000"
5. **Passes the phone test.** Shrink it to the size of a fingertip. The emotion and the text must still read. If a detail turns to mush, cut it.

---

## Steps

1. **Write the split.** "Title says: ___. Thumbnail carries: ___."
2. **Pick the lever to test.** Each concept varies one big thing so the A/B result means something:
   - face vs object
   - text vs no text
   - warm vs cool dominant colour
   - before vs after
3. **Fill the brief for each concept** using the template below.
4. **Run the five non-negotiables** on each. Flag any concept at risk on the phone test.
5. **Recommend the lead concept.** Test & Compare judges by watch time, not raw clicks, so favour the concept that attracts the right viewer over the one that attracts the most curious one.
6. **Add an image-tool prompt** if the user wants to generate it. One paragraph describing subject, emotion, composition, lighting and background. Text overlays are added afterwards in a design tool, because image models still mangle lettering.

---

## Brief template (one per concept)

```
CONCEPT [A/B/C]: [short name]
Lever being tested: [face vs object / text vs none / colour / before-after]

SPLIT
Title says: [...]
Thumbnail carries: [...]

FOCAL SUBJECT
[face + named emotion, or the single object/result]

TEXT OVERLAY
Words: [4 or fewer, no punctuation, none from the title]
Placement: [opposite the face / upper left / etc.]
Style: [weight, colour, one emphasised word]

BACKGROUND & CONTRAST
[colour, lighting, how the subject separates]

COMPOSITION
[rule-of-thirds position, gaze direction, crop]

PHONE TEST
[what must survive at fingertip size; what to drop if it doesn't]
```

---

## Worked example

**Input:** Title "I Let Claude Run My Newsletter for 30 Days". Payoff: open rate held, one issue flopped badly. Face available. Channel colours: navy and orange.

**Concept A: The nervous handover**
- Split: title says "Claude ran it for 30 days". Thumbnail carries the risk.
- Focal subject: your face, eyebrows up, teeth clenched (nervous anticipation).
- Text: "DAY 30" in orange.
- Background: dark navy, a laptop glow lighting your face from below.
- Composition: face on the right third looking left at the text.
- Phone test: face and "DAY 30" must read. Drop any visible screen text.

**Concept B: The result, no face**
- Lever: object vs face.
- Focal subject: a single phone screen showing an inbox with one subject line highlighted in red.
- Text: none. The red highlight does the work.
- Phone test: the red line must read. If not, enlarge the phone to fill 70% of the frame.

**Lead with A.** The video is a personal experiment and the emotion sells the risk. B tests whether your audience clicks on proof over personality.

---

## Output format

```
## Thumbnail brief: [title]

Split: title says [x] / thumbnail carries [y]

[Concept A brief]
[Concept B brief]
[Concept C brief, optional]

Lead concept: [A/B/C], because [one line]
Image-tool prompt (optional): [one paragraph, no text in the image]
```

---

## Sibling skills

- `yt-title-optimizer`: write or sharpen the title first. They're a pair.
- `yt-hook-scripter`: the opening seconds should match the thumbnail's emotion.
- `yt-content-planner`: plans title and thumbnail angles across a month.
- `youtube-thumbnail-design` (if installed): turns this brief into an actual image.

---

## Pre-flight checklist

- [ ] The split is written down for every concept.
- [ ] One focal point each. A named, earned emotion if there's a face.
- [ ] Overlay text is 4 words or fewer, no punctuation, no title words.
- [ ] Every concept passes the phone test, or the risk is flagged.
- [ ] Concepts vary one big lever, not five small ones.
- [ ] Nothing shown that doesn't happen in the video.
- [ ] A lead concept is named with a reason.
