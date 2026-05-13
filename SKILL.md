---
name: story-doctor
description: Narrative review best practices and guidance — a curated reference of anti-patterns, craft conventions, and diagnostic methods for evaluating and revising fiction. Use when revising a manuscript, diagnosing why a story isn't working, stress-testing character, or evaluating scene-level craft. Runs structured antipattern checks, scene evaluation, motivation triage, and second-pass plot review.
---

# Story Doctor

A structured triage sequence for diagnosing what's broken in a story — and what to do about it.

Drawing from multiple craft traditions, this skill organizes narrative problems into actionable categories: character, scene, conflict, motivation, and structure. Work through the sequence in order. Stop at the first diagnosis that applies — that's usually the root cause.

## Craft Sources

- **Stein on Writing** — Sol Stein's diagnostic method (character antipatterns, motivation, scene evaluation)
- **Gotham Writers** — Scene craft, dialogue, voice, point of view, narrative structure

See [references/](references/) for full source content organized by author.

---

## The Triage Sequence

---

### Step 1: Autobiography Antipattern

**What it is:** The main character sounds too much like the writer. Same voice, same reactions, same vocabulary, same worldview. This kills the narrative distance every story needs.

**Diagnosis prompt:**
```
Cross-examine the protagonist against the writer (from USER.md or memory):
- Does the protagonist react the way the writer would?
- Is there a values divergence the writer would never choose?
- Is the protagonist's worldview a subset of the writer's?
- Is the engineering/analytical lens shared? (flag as seam)

Generate a table:
| Dimension | Protagonist | Writer overlap? |
|-----------|------------|-----------------|

Signal: Yellow if one dimension overlaps, Red if two+.
```

**Fix template:**
> **The stake in the ground:** Give the character a distinctive trait — positive or negative — that you're absolutely certain you don't have. Something specific, observable, and slightly embarrassing or idiosyncratic.
>
> *Example from character data: [extract actual trait from character docs]*.

---

### Step 2: Boring Protagonist Antipattern

**What it is:** The main character is competent, sympathetic, and entirely forgettable. You're asking the reader to spend hours with this person — there must be something that makes them impossible to replace with anyone else.

**Diagnosis prompt:**
```
Audit the protagonist's texture against these failure modes:
- Can you describe their goals but not their friction?
- Are their habits generic rather than idiosyncratic?
- Could a scene with this character be rewritten with a different name and lose nothing?
- Does the character move through the story without friction?

Check for: distinctive vice palette, specific voice moments, behavioral quirks that cost them something, eccentricities that create visible scene-level friction.

Generate:
| Texture layer | What's there | Memorable? |
|--------------|-------------|------------|
```

**Fix template:**
> **Eccentricity is friction with a pulse.** The fix is not "add a quirk" — it's add a trait that:
> - Is specific enough to be visible on the page
> - Creates friction — it should get in her way, not just exist as color
> - Feels slightly embarrassing or weird, not admirable
> - Makes her irreplaceable in scenes where any functional person could stand in
>
> *Proposed from character data: [extract or suggest based on existing traits]*

---

### Step 3: Protagonist Grill

**What it is:** A stress-test of how well the writer actually knows their protagonist. The goal is to surface assumptions, test texture, and find gaps before they become plot holes.

**How to run:** Ask the writer questions about the protagonist. One at a time. Don't move on until there's a real answer — not "I'll figure it out later." The goal is gaps, not confirmation.

**Question categories to cover:**

1. **Surface facts** — What do they look like? What do they own? What's their daily routine?
2. **Obsessions and avoidances** — What can't they stop doing? What do they refuse to touch?
3. **Friction in scenes** — In a tense moment, what do they do that they can't control? What do they reach for, say, or orbit around?
4. **Blind spots** — What does the protagonist believe about themselves that's wrong? What would mortify them if someone else saw it?
5. **Values under pressure** — When forced to choose between X and Y, what do they reach for first? (e.g., safety vs. truth, family vs. self, winning vs. surviving)
6. **Voice** — Finish this sentence in the protagonist's voice: *"I can't stand it when people —"*
7. **Unfinished business** — What did they want when the story started? What do they think they want at the midpoint? What do they actually need by the end?

**Verdict:** If any category produces "I don't know" or a blank, flag it. That's a gap. Don't fix it yet — just name it and move on.

> The writer should be able to answer all of these without looking at the manuscript. If they can't, the protagonist isn't fully built yet — and that's what the grill is for.

---

### Step 4: Frozen Character (Static Protagonist)

**What it is:** The main character ends the novel the same way they began it — same beliefs, same behaviors, same relationship to the world. No mark was left. No collision occurred. They passed through the story without being changed by it.

**Why it matters:** Novel-length fiction makes an implicit promise: this person will be different on page 300 than they were on page 1. When that promise goes unkept, the reader feels robbed of the journey they signed up for. Short stories are exempt — a window can show someone exactly as they are without requiring transformation.

**Exception:** *Waiting for Godot*. Beckett wasn't writing character change; he was writing stasis as philosophical condition. If your story is doing something Beckett-level experimental, the rule bends. Otherwise, assume change is mandatory.

**Diagnosis prompt:**
```
Track the protagonist's state at two points:
- Beginning: what do they believe? what do they avoid? what can't they do?
- End: same questions. what actually shifted?

Generate:
| Dimension | Start | End | Changed? |
|-----------|-------|-----|----------|
| Belief about self | | | |
| Central behavior/habit | | | |
| Relationship to problem | | | |
| What they reach for under pressure | | | |

Signal: Red if two or more dimensions show no meaningful shift.
```

**Fix template:**
> **The collision must land.** Something in the story needs to hit the protagonist hard enough that they can't stay who they were. This isn't gentle "character growth" — it's fracture, revision, or revelation. The change can be positive, negative, or ambiguous, but it must be visible and structural, not cosmetic.
>
> *Ask: what happens at the midpoint that forces them to choose between who they were and who they need to become? That's where the freeze starts to crack.*

---

### Step 5: Antagonist Check

**What it is:** Problems don't end with the protagonist. A weak, diffuse, or charmless antagonist undermines the story just as thoroughly as a flat main character. The antagonist is the protagonist's mirror — if the mirror is cardboard, the collision means nothing.

---

#### Antipattern A: Diffused Villainy

**What it is:** Multiple antagonists watering down the evil. When you spread villainy across several characters, none of them land with full impact. The reader can't focus their resistance, their fear, their hatred on one clear target.

**Diagnosis:** Count the primary antagonistic forces. If there's more than one character driving the conflict at full strength, consider collapsing them into one.

**Fix template:**
> Consolidate. Pick the most compelling antagonist and make the others secondary — helpers, symptoms, consequences. One clear villain creates sharper conflict than a committee of mean people.

---

#### Antipattern B: Morally Shallow (Merely Naughty)

**What it is:** The antagonist is badly behaved, inconvenient, or unpleasant — but not morally bad. They have no genuine depravity at the core, just inconvenience. Readers sense the difference. A character who's just annoying creates a story that feels low-stakes.

**Diagnosis prompt:**
```
Cross-examine the antagonist's moral core:
- Do they have a cause they believe in, or just preferences?
- Are they capable of genuine harm, or just friction?
- Does their opposition to the protagonist stem from values, or from circumstance?

Signal: Yellow if they have no moral dimension beyond being difficult. Red if the story treats them as a serious threat but they only generate annoyance.
```

**Fix template:**
> **Dig deeper.** Morally bad doesn't mean moustache-twirling evil — it means the antagonist has a worldview that collides with the protagonist's in a way that can't be reasoned around. They need a genuine conviction, even if it's wrong. Bad behavior is a surface problem. Moral corruption is structural.

---

#### Antipattern C: Cartoon Villain

**What it is:** The antagonist who exists only to be antithetical. No charm, no enticement, no humanity — just obvious malevolence dressed in a costume. "The mustachioed antagonists of yesteryear only provoke laughs today."

**Why it matters:** Even villains need something that draws people to them — a quality, a cause, a charisma that makes the conflict feel dangerous rather than theatrical. Without it, the antagonist becomes a punchline.

**Diagnosis prompt:**
```
Ask: what does the antagonist offer that might make a reader halfway sympathize?
- Are they funny?
- Do they believe in something?
- Is there a version of their argument that almost makes sense?
- Do other characters follow them out of something other than fear?

Signal: Red if the antagonist has zero appeal beyond being the obstacle. Yellow if they have surface charm but nothing underneath.
```

**Fix template:**
> **Give the villain a human entry point.** They don't need to be likable — but they need to be understandable from the inside. Even a little charisma, a coherent worldview, or a grievance that reads as legitimate from a certain angle makes the villain real instead of theatrical. The best antagonists are the ones you could almost root for if you squinted.

---

#### Antipattern D: Villain Bio Trap

**What it is:** The writer models the villain on a real enemy — someone they genuinely resent or dislike in life. The emotional proximity prevents craft. The writer can't give the villain appeal, charisma, or humanity because doing so feels like a betrayal of who they're punishing in the story.

**Why it matters:** A villain who only functions as a target is a flat character. Even antagonists who are genuinely evil need to feel real, not just justified from one perspective.

**Diagnosis prompt:**
```
Ask: did the villain's model come from someone the writer actively dislikes or has a grievance with?
- Is the villain given any traits that would make them recognizable to their real counterpart?
- Does the villain have any dimensions the real person couldn't see themselves in?

Signal: Yellow if the model is a real adversary with unresolved feelings. Red if the villain exists primarily as revenge dressed in fiction.
```

**Fix template:**
> **Use composites, not portraits.** Pull from multiple sources. Borrow the villain's core quality from one person, the mannerisms from another, the backstory from a third. Or flip the equation: write the villain as someone the real person would never recognize. Distance is the tool. Composite is the technique.

---

#### Technique: Humanizing Through Another Character's Eyes

**The problem:** You can't make the villain charming or interesting on your own — your own feelings are in the way.

**The fix:** See the villain through the eyes of someone who loves or cares about them. A follower, a spouse, an admirer. Write a scene from that character's perspective, just for the exercise. The villain's appeal becomes visible when filtered through genuine care instead of pure antagonism.

**Why it works:** Caring reveals texture. The lover sees the charm. The follower sees the cause. The rival sees the intelligence. That texture feeds back into the villain's main presence, even when seen from other angles.

---

### Step 6: Minor Characters — The One-Thing Trap

**What it is:** Minor characters who feel like set dressing instead of people. A scene's credibility depends on the reader buying that these are real humans — and one wrong note makes the whole thing wobble.

**Why it matters:** A throwaway character who's clearly a prop breaks the fictional dream faster than a plot hole. The reader's pattern-recognition fires: fake. And once it fires, it keeps firing.

**The one-thing rule:** One specific characteristic is enough. Not a list of traits — one thing. A gesture, a mannerism, a vocal pattern, a way of entering a room. The reader's imagination fills in the rest. The trick is picking the right one: not a *quirk*, but a behavior that implies an interior.

**Diagnosis prompt:**
```
Audit every named character who appears in more than one scene but isn't the protagonist or antagonist:
- Do they register as a person, or as a function?
- Is there one visible characteristic that makes them stick?
- Does that characteristic suggest something about who they are outside the scene?
- Could they be replaced with "Generic Person #3" without the scene changing?

Generate:
| Minor character | Their function | One visible trait? | Implied interior? |
|----------------|----------------|--------------------|-------------------|
Signal: Red if they fail all four. Yellow if they pass function but nothing else.
```

**Fix template:**
> **Characterize, don't decorate.** A limp is a limp. Touching their collar is nervous-habit decoration. The characteristic that works has a pulse — it suggests something the reader can guess at without you saying it.
>
> *Ask: what does this person want? What are they afraid of? What's the one thing about themselves they'd never say out loud? Then find the ONE visible behavior that telegraphs that interior without naming it.*
>
> The best minor characters feel like they've had a life before the scene started. You don't have to write that life — you just have to pick the one detail that makes the reader believe it exists.

---

### Step 7: Weak Conflict — The Story Has No Legs

**What it is:** The protagonist and antagonist aren't in real collision. The obstacles are shallow, the stakes feel low, or the course of resistance is muddy. The story has no engine.

**Why it matters:** Stories from time immemorial have consisted of people overcoming obstacles against high odds and strong adversaries. This isn't a formula — it's the architecture that makes readers care. When that architecture is missing, nothing else fixes it. You can have perfect voice, beautiful sentences, great characters — and the reader's attention slides off the page because there's nothing to *push against*.

**The test:** Strip the antagonist's identity away. Does the plot collapse without them? If the protagonist could achieve their goal regardless of who or what opposes them, the conflict isn't real.

**Diagnosis prompt:**
```
Ask:
- Is the antagonist genuinely threatening, or just an inconvenience?
- Could the protagonist win with moderate effort, or does it require everything?
- Are the stakes personal and specific, or vague and abstract?
- Does the protagonist have to sacrifice something real to win?

| Dimension | Present? | Credible? |
|-----------|----------|----------|
| Antagonist strength | | |
| Cost of victory | | |
| Personal stakes | | |
| No easy out | | |
Signal: Red if any dimension is weak or absent.
```

**Fix template:**
> **The antagonist must earn their role.** They don't need to be powerful in a physical sense — they need to be the RIGHT obstacle. The thing standing between the protagonist and what they want must be something that can't be reasoned with, bargained with, or skipped.
>
> *For deeper plot repair: see references/stein.md and references/gotham.md for scene and structure guidance.*

---

### Step 8: Stress and Escalation

**The rule:** Fiction deals with the most stressful moments of the characters' lives. If the pressure never builds, the story has no engine.

**Two questions:**
1. **Are your characters under stress from time to time?** Not just initial difficulty — genuine, escalating pressure that forces them to react.
2. **Does the stress increase?** The midpoint should raise the stakes. The climax should demand everything. If stress plateaus, the story plateaus.

**Why it matters:** A story where characters face manageable challenges is a story that never commits. The reader can sense when the stakes are artificially constrained — when the writer is protecting the characters from the consequences of their own actions.

**Diagnosis prompt:**
```
Track stress across the manuscript:
- Where does stress first appear in the story?
- Does it escalate from that point forward, or does it flatten?
- At the midpoint: has the pressure increased from the opening?
- At the climax: is this the highest-pressure moment of the story?

| Act | Stress level | What's driving it? |
|-----|-------------|-------------------|
| Opening | | |
| Midpoint | | |
| Climax | | |

Signal: Red if stress doesn't meaningfully increase from opening to climax. Yellow if the escalation is uneven or if the climax doesn't feel like the highest-pressure moment.
```

**Fix template:**
> If stress isn't escalating, find the midpoint and ask: what happens here that raises the cost? What does the character now have to face that they weren't facing before? The midpoint is where the story commits — if the pressure doesn't build there, it won't build anywhere.

---

## Scene Evaluation

These prompts shift from character diagnosis to scene-level craft. Work through them in order.

---

### Scene Prompt 1: What's the Most Memorable Scene?

**The question — ask the writer directly, do not let them look at the manuscript:**

> *"What is the most memorable scene in your book? Don't go to your manuscript for clues. If you can't remember the scene, it isn't memorable."*

**Why this matters:** Memory is a proxy for emotional impact. If a scene doesn't lodge in the writer's own memory after the work is done, it won't lodge in the reader's either. The scenes that survive the writing process are the ones that mattered — and the ones that don't survive are carrying dead weight.

**What to listen for:**
- **Fast answer, specific scene** → Good. The writer knows what they're working with.
- **Hesitation, vague description** → Yellow flag. The scene may exist on the page but didn't land with force.
- **"I can't think of one"** → Red flag. The story may be atmospherically pleasant but dramatically flat. No scene burned itself in.
- **Describes the whole plot instead of one scene** → They may not have scenes yet — they have a summary. Prompt them to isolate one moment.

**If the answer is weak:**

> **Memorable doesn't mean dramatic in the obvious way.** It could be a quiet scene — a look, a line of dialogue, a moment of recognition. The test is whether the scene has a pulse of its own, not whether it's action-packed. Ask the writer to describe it in one or two sentences. If they can't, the scene needs rebuilding.

---

### Scene Prompt 2: What's the Least Memorable Scene?

**The question:**

> *"What's the scene in your book you remember least — the one that doesn't stick? Go back to the manuscript and find it. Don't read it word for word — browse. You know it when you see it."*

**Why browse, not read:** Word-for-word reading kills momentum and pulls you back into the draft's gravity. Browsing lets you feel whether a scene has its own engine.

**What to listen for:**
- **Scenes the writer already suspects are dead weight** → Yellow. At least they're aware.
- **Scenes the writer insists "have to be there for information"** → Red flag. Information can be transferred to a stronger scene. "Has to be there" is usually "I'm too attached to let it go."
- **Scenes the writer doesn't recognize as scenes at all** → They're probably summary, not scene. Flag it.

---

### Scene Prompt 3: Compare the Two.

**The conversation:**

> *"Now compare your most memorable scene and your least memorable scene. What's the difference? Don't overthink it — just feel it. One has a pulse, one doesn't. What is the most memorable scene doing that the other isn't?"*

**What this unlocks:** The comparison itself is a revision tool. The writer often sees the problem immediately once the two scenes are side by side — the memorable one has stakes, specificity, a character in motion. The weak one is decorative, expository, or static. That gap is the fix.

**Follow-up:**

> *"Do you see anything in the memorable scene that could transfer energy into the weak one? A quality, a rhythm, a kind of tension?"*

---

### Scene Prompt 4: Revise or Cut.

**The rule:**

> *"If you can't think of how to make the least memorable scene work, cut it. The usual remedy is to cut it."*

**Exceptions:**
- The scene carries information the reader genuinely needs
- But even then — find a way to deliver that information inside an existing scene that already has momentum. Don't keep a weak scene on life support just to deliver exposition.

**The test:**

> *"Would the book be stronger without it?"*

**If the answer is yes:** Cut. No ceremony. The story will breathe.

**Then:** Once you've revised or cut the weakest scene, find your *new* weakest scene. Keep applying pressure.

> *"Now look at what you've got left. What's the next scene that doesn't earn its place? Same question — would the book be stronger without it?"*

Repeat until the remaining scenes all pull their weight.

---

## Motivation — The Chekhov's Gun Section

After you've dealt with scenes, the next step is motivation.

---

### Motivation Prompt 1: Name the Three Most Important Actions

**The question — from memory, no manuscript:**

> *"What are the three most important actions in your novel? Jot them down from memory."*

**Then for each:**

> *"Is each action motivated in a way you would accept if the story were told by someone else? Does the motivation hold up if you didn't write it?"*

**Why from memory:** If the writer can't recall their own three biggest actions without looking, the story is probably running on autopilot — events happening because the plot requires them, not because the characters earned them.

---

### Motivation Prompt 2: Provoke or Plant

**The rule:**

> *"Motivation has to be either provoked by circumstance or planted ahead of time."*

**Two sources of motivation:**
- **Provoked by circumstance:** Something happens in the story that forces the character to act. External pressure creates internal decision.
- **Planted ahead of time:** The seed is placed earlier — a detail, a conversation, a behavior — so the action feels inevitable when it arrives.

**If an action lacks both:** It's probably authorial convenience. The plot needed something to happen, so it happened. The character is a puppet.

---

### Chekhov's Gun — The Obligatory Scene

> *"If someone has a gun in the first act, they must use it by the third act. Amongst playwrights, that is known as an obligatory scene."*

**The failure mode:** A gun appears in the hands of someone who isn't known to carry one, and is almost immediately fired. The audience feels the author's heavy hand — the event was conjured, not earned.

**The fix:** Plant the gun earlier. When it fires later, the audience saw it coming. They *waited* for it. The use becomes almost inevitable.

**The bonus:** Plant it and then *don't* fire it when the audience expects you to — that creates a different kind of suspense. They're watching the gun the whole time, wondering when it will go off.

**Diagnosis prompt:**
```
For each of the three main actions:
- Is the motivation planted before the scene where the action occurs?
- Is the motivation provoked by circumstance within the scene itself?
- Or is it neither — the action happens because the plot requires it?

| Action | Provoked? | Planted ahead? | Neither? |
|--------|-----------|----------------|---------|
Signal: Red if an action lacks both.
```

**If red:**
> **Trace backward.** What scene could plant this action? What conversation, detail, or circumstance could make this action feel inevitable rather than convenient? If you can't find a place to plant it, the action may not belong in the story.

---

### Motivation Prompt 3: The Full Audit

**The instruction:**

> *"After you've dealt with the three main actions, the next step is to review any other significant actions — ferret out anything that seems to happen just because the author wants it to."*

**The diagnostic questions:**
- Is there any action in the manuscript that isn't in keeping with the character?
- Is there any action that sounds farfetched under examination?

**The fix:**
> *"It might be fixed by planting a motive in a prior scene."*

**The sequence:**
1. Identify each significant action outside the three big ones
2. Test each one: provoked by circumstance, or planted ahead?
3. If neither: find the scene where you could plant the motive — or cut the action
4. Only then do a full manuscript read-through to judge whether the fixes work in sequence

**Why this order matters:** You don't want to revise a scene until you've fixed the motivation problem in it first. Otherwise you're polishing a house with a cracked foundation.

---

### Motivation Prompt 4: Chapter 15 Reference

Stein's Chapter 15 contains a detailed motivation unit-testing methodology. Once read, extract and fold it into the motivation section as a structured diagnostic tool.

**GitHub issue:** [#5 — capture Chapter 15 motivation methodology](https://github.com/lux-sp4rk/marina/issues/5)

---

## Second Pass — Cutting

After the motivation audit, before the plot pass: cutting. Tightening the manuscript is a separate discipline from rewriting — the goal is excision, not revision.

### The First Rule

> **When in doubt, do not change anything.** You must be certain it must go.

**When you find something questionable:** instead of changing it, make a note for further consideration — a GitHub issue, a task, whatever system the writer uses. This keeps the revision session focused and prevents the spiral of rewriting without resolution.

---

### Item A: Between-the-Scenes Material

**First target: offstage recounting of actions not seen.** The manuscript material that bridges scenes — the passages where the writer recounts events that happened offstage, or summarizes what happened between scenes.

**The rule:** Eliminate as many of these as possible, or transform them into active, interesting prose that earns its place.

**Why it matters:** Offstage recounting is the most common source of flat, inert prose in a draft. The writer is explaining what happened rather than showing it. The reader experiences the summary as summary — no tension, no stakes, no scene.

**Fix options:**
1. **Cut entirely** — if the event doesn't need to be shown, it may not need to be mentioned
2. **Dramaticize** — make the recounting a scene in itself, rendered in real time with tension and stakes
3. **Compress further** — reduce a whole sequence of offscreen events to a single image or line that lands with force

> *For clarification on rendering vs. summarizing: see references/stein.md and references/gotham.md.*

**Diagnosis prompt:**
```
Browse the manuscript for every passage that bridges two scenes — the "Meanwhile, back at..." material, the retrospectives, the offstage recounting.

For each such passage:
- Does this advance the story in a way the reader needs?
- Could it be cut with no loss to the reader's understanding?
- If kept, does it have tension and stakes of its own, or is it inert summary?

| Passage | Purpose | Could cut? | Has tension? |
|---------|---------|------------|---------------|

Signal: Red for inert summary that exists only to fill gaps. Yellow for passages with some purpose but without tension.
```

---

### Item B: Flags and Fails — Cut What Doesn't Earn Its Place

Cut words, phrases, sentences, paragraphs, pages, or whole scenes that seem absolutely not necessary.

**The signal: your own attention flags.** When you find yourself slowing down, rereading a passage, or feeling the prose go slack — that's usually a sign something needs to be revised or cut. If the writer's attention flags while reading their own manuscript, the reader's will too.

**Diagnosis prompt:**
```
Browse the manuscript and note every place where your attention flags — where you slow down, lose momentum, or feel the prose going slack.

For each flag:
- Is this a cutting opportunity? (tighten or remove)
- Is this a revision opportunity? (rewrite to restore momentum)
- Is this just a rough patch that needs a lighter edit?

| Passage | Flag type | Action |
|---------|-----------|--------|
```

**Rule:** Be ruthless with flags. If your attention flags on page 50 while reading, the reader's will flag too. And readers who flag don't always come back.

---

### Item C: Sentence Rhythm — Vary the Length

**The problem:** If all sentences are approximately the same length, the effect is monotonous. The prose becomes a flatline — readable, but uneventful.

**The fix:** Vary sentence length deliberately. Follow an especially long sentence with a short, even abrupt sentence. Create contrast in rhythm.

**The trap:** Don't overcorrect. A short-long-short-long pattern can get almost as monotonous as all long or all short. The variation should feel natural, not metronomic.

**Stein's example:** One of his students wrote naturally in a "mellifluous cadence" — it was her greatest fault. An unbroken mellifluous cadence, lovely for a few sentences, will put a reader to sleep if kept up.

**Diagnosis prompt:**
```
Read a section aloud. Listen for:
- Sections where sentences all feel the same length
- The "mellifluous" trap — lovely but soporific
- Places where the rhythm goes flat without you noticing

| Section | Rhythm quality | Needs variation? |
|---------|----------------|------------------|
```

**Fix template:**
> Find the longest sentence in the flagged section. Follow it with one that's two to three words. Let the short sentence land like a window slam. Then let the rhythm settle. Don't make it a pattern — make it a surprise.

---

### Item D: Trim the Prose

**Every word earns its place or it goes.**

**Rule 1: Cut unnecessary adjectives and adverbs.** Especially: cut "very." Cut "poor" for everything but poverty. If the word doesn't add meaning the sentence can't live without, it goes.

**Rule 2: Don't say the same thing twice in different words.** If two phrases convey the same idea, pick the stronger one and cut the other. Redundancy is dead weight.

**Rule 3: Watch for repeated uncommon words.** If you find yourself using the same distinctive word twice within a few pages, reach for a synonym. Repetition of a rare word sticks out like a broken note.

**Rule 4: Mark every cliché for exclusion.** Clichés are borrowed language — they arrived in the manuscript without earning their place. Flag them. Then decide: rewrite with fresh language, or cut entirely.

**Diagnosis prompt:**
```
Scan a chapter for:
- Adjectives and adverbs that could be removed without losing meaning
- "Very" — always suspect
- Repeated words (common or uncommon) within a few pages
- Clichés — phrases that feel familiar rather than fresh

| Location | Issue | Action |
|----------|-------|--------|
```

**Fix template:**
> If a word is doing no real work — if it's adding texture without meaning, or repeating what's already clear — cut it. Every unnecessary word is a tax on the reader's attention.

---

### Item E: Word Order — Emphasis and Clarity

**The principle:** Word order shapes emphasis. What lands at the end of a sentence carries the most weight. Moving words, phrases, or clauses changes what the reader focuses on.

**Rule 1: Dialogue attribution**
If there's any chance the reader won't know who is speaking at that moment, put the attribution first:

> *George said, "they treating you okay?"*

If it's already clear who is speaking, the attribution can follow or be omitted:

> *"They treating you okay?" George said.*

**Rule 2: Transposition for emphasis**
Move elements to shift what the sentence emphasizes. The end of the sentence is where the punch lands.

**Example — unedited:**
> *"Josephine Japhet of course knew her son was a reader in a universe of listeners to rock music."*

Emphasis falls on rock music.

**Transposed:**
> *"Josephine Japhet, of course, knew why, in a universe of listeners to rock music, her son was a reader."*

Emphasis shifts to her son being a reader — which was the actual point.

**The discipline:** In a book-length manuscript, transpositions happen hundreds of times. Read for where the sentence's natural emphasis lands — and whether it matches what you're actually trying to say.

**Example 2 — consequence before cause (unclear):**
> *"If Paul goes to jail, I won't have anywhere. I can't pay the mortgage on my own."*

The phrase "I won't have anywhere" is vague — the reader doesn't know anywhere what until the next sentence lands.

**Transposed — cause before consequence:**
> *"If Paul goes to jail, I can't pay the mortgage on my own. I won't have anywhere."*

Now the reader gets the reason first, then the consequence lands clearly. Logic flows.

**The rule:** Consequence before cause is often confusing. Cause before consequence flows naturally. Transpose until the logic is obvious.

**Diagnosis prompt:**
```
Read each scene aloud. For each sentence, ask:
- Who is the subject? Is it in the right position?
- Where does the sentence end? Does that landing word carry the right weight?
- For dialogue: is attribution placement clear? Could the reader lose track of who's speaking?
- Does the word order match the intended emphasis, or does transposition need to shift it?
- When a phrase or clause feels vague on its own — does it need something before it to give it context? (cause before consequence)

| Sentence | Current landing | Intended emphasis | Transpose? |
|----------|-----------------|-------------------|------------|
```

---

### Item F: Find the Next Weakest Scene

**The instruction:** Once you've revised or cut the weakest scene, find your *new* weakest scene. Keep applying pressure.

> *"Now look at what you've got left. What's the next scene that doesn't earn its place? Same question — would the book be stronger without it?"*

**Repeat until:** The remaining scenes all pull their weight. The manuscript is tighter, the pacing sharper, the dead weight removed.

---

### Item C: The Cutting Pass — A Sequence

Stein's recommended sequence for the cutting pass:
1. Remove between-scenes material that is inert or summary
2. Tighten the remaining bridging passages
3. Identify and cut any scene that doesn't earn its place
4. Find the next weakest scene — repeat

**Key discipline:** Do not revise while cutting. If something is questionable, note it and move on. The goal is a tighter manuscript, not a rewritten one.

---

## Second Pass — Plot

*After character work, put the manuscript down for a day or two. Let it cool. Then start the second pass: plot.*

---

### Item E: Pace — Keep the Story Moving

**The rule:** Unless you are consciously trying to slow things down between fast-moving scenes, be relentless in keeping the story moving forward.

**The signal:** If you find it bogging down at any point — something is wrong. Causes can include: too slow a pace, not enough happening, a scene that has lost its engine.

**The discipline:** If you don't see an immediate fix, make a note of it — a GitHub issue, a task, whatever system the writer uses — and move on. Come back to those places later.

**This is triage.** The goal of the revision session is to move through the manuscript with forward momentum, not solve every problem in real time. Flag it, note it, keep moving. Fixes come in a later pass.

**Diagnosis prompt:**
```
Browse the manuscript for every place where the story bogs down — where the pace slows noticeably, where the reader might start to drift.

For each bog-down point:
- Do you see an immediate fix? (apply if obvious)
- Is the cause unclear? (note it as a candidate for later revision)

| Location | What flags | Immediate fix? | Note for later? |
|----------|------------|----------------|------------------|
```

**Fix template:**
> If the pace is slow and you can't find a fix quickly — note the problem, note your guess about what's wrong, and move on. Don't let the revision session stall. The manuscript gets a second pass.

**Exception:** Deliberate slow scenes are valid — they create contrast and allow the reader to breathe. The rule only applies when the slowdown is unintentional.

---

### Item F: Author Voice Bleed

**The signal:** Catching the author talking at the reader — or mixing points of view within a passage.

**What it is:** The narrative voice shifts from the story's established perspective to the author's own commentary or presence. Or: the point of view shifts without a scene break, creating confusion about whose head the reader is in.

**The fix:** Mark the section and note it for Chapter 13 guidance. Do not attempt to fix in the revision session — this requires the deeper POV methodology in Chapter 13.

> *See references/stein.md — Chapter 13 reference pending.*

**Diagnosis prompt:**
```
Browse for passages where:
- The author seems to address the reader directly (commentary, editorial intrusion)
- The point of view shifts mid-passage without a scene break
- The narrative voice sounds like the author rather than the narrator

| Location | Issue type | Needs Chapter 13? |
|----------|------------|---------------------|
```

---

### Plot Prompt 1: Does Scene One Make You Read Scene Two?

**The test — read scene one, then ask yourself:**

> *"Would I go on to read the second scene?"*

**If no:**
> *"You haven't sparked the reader's curiosity. Review scene craft guidelines in references/gotham.md to fix the opening."*

**If yes:** Congrats. The first scene earns its place.

**What "compelling reason" looks like:**
- A question the reader needs answered
- A character in motion toward something they want
- A voice that pulls you in and makes you want more
- A situation that feels unstable — something is wrong, or about to be

**What "no compelling reason" looks like:**
- The scene describes a status quo the reader has no reason to care about
- Nothing is at stake yet, and nothing is threatened
- The writer is still setting up instead of starting the story
- The character is calm, comfortable, and the world has no visible cracks

**The rule:** The first scene must create a itch, not finish an explanation. If the reader understands everything by the end of scene one, there's nowhere left to go.

---

## Appendix: Open Questions

- [#5 — capture Chapter 15 motivation methodology](https://github.com/lux-sp4rk/marina/issues/5)
- [#6 — add Gotham Writers scene structure patterns](https://github.com/lux-sp4rk/marina/issues/6)
- [#7 — add dialogue and voice antipatterns from Gotham](https://github.com/lux-sp4rk/marina/issues/7)
- [#8 — capture Chapter 13 (POV / talking at the reader / mixing points of view)](https://github.com/lux-sp4rk/marina/issues/8)