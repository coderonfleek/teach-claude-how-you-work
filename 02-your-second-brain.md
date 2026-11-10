# Lesson 2 — Your Second Brain

## Lesson goal

By the end of this lesson you'll have:
- a **wiki** about you and your work, written by Claude from your own material, with a contents page (`index.md`) and a diary of changes (`log.md`)
- **judgment pages**: your voice, what good looks like to you, how you edit, a review checklist and your **visual style** (for our writer, how her diagrams look)
- the three **wiki habits**: *add* new material, *ask* your wiki questions, and *tidy* it
- a proper home for your corrections, so you never have to tell Claude the same thing twice

**Why this lesson matters:** this is the "brain" in second brain. Every skill you build in Lesson 4 reads these pages. A skill can only write in your voice, review like you or draw like you if the wiki says *exactly* how you do it.

⏱ About **2 hours**. Claude works for about 40 minutes of that: the first add takes about 8 minutes, the judgment pages about 7, the visual-style page about 6, and each later step 1–4 minutes. The rest is you reading pages and answering about 25 questions on your taste, in rounds of 3.

> **Usage note:** this is the heaviest lesson in the course for Claude usage: Claude reads everything you collected, then keeps your whole wiki in mind for the rest of the chat. On a Pro plan you'll probably hit your usage limit at least once. When you do, just continue in the same chat when it resets.

> **Click Allow when Claude asks to run something.** To read Word files or measure your images exactly (colour codes, sizes), Claude may ask to run a small command or script. Click **Allow**. If you click Deny, it still works, but it will estimate by eye and mark those values as guesses.

### The three parts of this lesson

| Part | What you do | What you get |
|---|---|---|
| **A** | Set up the wiki and let Claude write the first pages | `wiki/` with `index.md`, `log.md` and your first pages |
| **B** | Teach Claude your judgment | Voice, standards, editing, review-checklist and visual-style pages |
| **C** | Learn the three wiki habits | Add, ask and tidy, plus a home for your corrections |

---

## Before you start

- Lesson 1 is done: you have `work-map.md`, `baseline/before-notes.md` and `gathering-list.md`.
- Work through your **gathering list** and copy what you collected into the `raw/` folders. **Copy, don't move**: your originals stay where they are.

| Folder | What goes in | Sample pack |
|---|---|---|
| `raw/past-work/` | 5–10 pieces of your work | 10 articles |
| `raw/visuals/` | 5–10 pictures (PNG or JPG) of diagrams, designs or other visuals you make | 5 diagram images |
| `raw/feedback/` | Notes from editors, managers or clients, before-and-after edits, comments from readers or customers | Dan's emails, 3 before-and-after drafts, reader comments |
| `raw/notes/` | Idea lists, voice memo transcripts, style notes, briefs | Idea list, 7 voice memo transcripts |

> **Using the sample pack?** Copy the contents of each of its `raw/` folders into the matching folder in `my-work-brain`. **Don't copy the `later/` folder yet**: you'll use it in Part C.

> **File names don't matter.** PDFs, Word files, screenshots, text files and pictures all work. Claude reads them all.

Open a **new chat** in `my-work-brain` for this lesson (click **New session**, or the **+** button). Claude reads `CLAUDE.md` at the start, so it picks up your rules from Lesson 1.

---

## Part A — Setting up the wiki

### Step 1 — Write the rules for your wiki

**What this does:** before Claude writes a single page, it writes down *how* the wiki works: what goes where, how pages link to each other, and the three habits. This is Andrej Karpathy's **LLM Wiki** idea: you supply the material, Claude does all the writing and filing, and a short set of rules keeps it consistent. The rules live in `CLAUDE.md`, so every future chat follows them.

**Send this to Claude** (works for any job as it is):

```text
We're going to turn this folder into my second brain, using Andrej Karpathy's "LLM Wiki"
method: raw/ holds my original material and never changes, wiki/ is written and maintained
entirely by you, and CLAUDE.md holds the rules. I don't write wiki pages myself, I only
read them.

Please add a "My wiki" section to CLAUDE.md with these rules, in plain words:
1. Sources: everything in raw/, plus work-map.md and baseline/before-notes.md. Never change
   anything in raw/.
2. Pages: one topic per page, as Markdown files in wiki/. Each page starts with a one-line
   summary, and lists the sources it came from at the bottom. Link related pages to each
   other using normal Markdown links, e.g. [my voice](voice.md).
3. Facts vs judgment: keep facts (what I've written, who I work with) separate from
   judgment (how I decide, what I like and hate, how I edit). Judgment pages matter most.
   Use my own words in quotes wherever you can.
4. index.md: the contents page. Every page, grouped by type, with its one-line summary.
   Read it first whenever you need to find something.
5. log.md: a diary you only add to. Every change gets a dated line that names the raw/
   files it used, e.g. "2026-11-09 · add · raw/past-work/ (all 10 files): created
   voice.md and 6 other pages".
6. The three habits, so I can just say the word:
   - "add <file>": read a new source, update every page it affects, update index.md and
     log.md, and tell me what changed. Just "add", with no file: find every file in raw/
     that log.md doesn't show as added yet, and add each one
   - "ask <question>": answer from the wiki (not from general knowledge), say which pages
     you used, and offer to save a useful answer as a new page
   - "tidy": check the whole wiki for contradictions, out-of-date claims, pages nothing links
     to, and gaps, then give me a short report and suggest fixes before making them
7. When there's a contradiction (e.g. my old work does X but I now say I hate X), don't
   pick one. Keep what the wiki says for now, and add a numbered question to the open
   questions on wiki/judgment-notes.md: both sides in quotes, where each came from, and
   your suggested answer. Then ask me. When I answer, now or later, apply it, mark the
   question answered with my words, and log it.

Also create wiki/index.md and wiki/log.md (empty apart from a heading), and add a line to
CHANGELOG.md. Don't write any other pages yet. When you're done, explain the rules back to
me in 5 short bullet points.
```

**What you should see:** Claude adds the section (click **Allow**), creates the two files and explains the rules back to you in plain bullets, something like *"Your originals stay untouched in raw/. I write and maintain everything in wiki/. index.md is the contents page…"*

**Check it worked:** open `CLAUDE.md`. There's a new **My wiki** section, and the rest of the file from Lesson 1 is still there.

**If it's not right:** *"You replaced my Lesson 1 rules. Please put them back and add the wiki section underneath."*

### Step 2 — The first "add": let Claude read everything

**What this does:** Claude reads all your material, then writes the first wiki pages: who you are, who you write for, what you write about, a short page for each piece of past work, and the people you work with. This is the *add* habit, done for everything at once.

**Send this to Claude** (works for any job as it is):

```text
add everything in raw/, plus work-map.md and baseline/before-notes.md.
This is the first add, so it's a big one. Work through it in this order and tell me
briefly what you're doing as you go:
1. Past work: read each piece and write a short page for it in wiki/work/ (what it is,
   who it's for, its main point, how it's structured, anything notable)
2. Feedback, notes and the rest: read each one
3. Then write the main pages, for example: about me, who my work is for (readers,
   customers, users, clients), what I work on, the people I work with, and how I work
   (my process, from the work map)
Leave the judgment pages (voice, standards, editing, review checklist, visual style) for
the next step: just collect notes for them for now.
Update index.md and log.md, then show me the list of pages you made and anything you
couldn't read.
```

**What you should see:** Claude works through your files, reporting as it goes (*"Reading 10 articles… Reading Dan's 6 emails…"*). This takes **about 8 minutes**. It ends with a list of new pages, something like:

- `wiki/about-me.md`: who you are and what you're known for
- `wiki/readers.md`: who you write for
- `wiki/topics.md`: what you write about, and how it fits together
- `wiki/people.md`: your editor, and anyone else who shows up in your work
- `wiki/process.md`: how you go from idea to published article
- `wiki/feedback-history.md`: what your editor has said, and how your first drafts changed before publishing
- `wiki/work/…`: one short page per article
- `wiki/judgment-notes.md`: notes for the next step, plus a list of **questions and contradictions** it found

The questions are the interesting part. With the sample pack, expect about 10, for example *"Your first drafts say you didn't time things, but the published pieces have exact numbers. Where did the numbers come from?"* Don't answer them yet: Claude asks them properly in Step 3.

**Check it worked:**
1. Open **`wiki/index.md`**. Every page is listed with a one-line summary.
2. Open **`wiki/about-me.md`** and **`wiki/readers.md`**. Do they describe you accurately? Are there quotes in your own words?
3. Click a link inside a page. It should open the linked page.
4. Open **`wiki/log.md`**. There's a dated line for this add.

**If it's not right:**
- *"readers.md is too vague. 'Busy professionals' could be anyone. Ask me questions to make it specific."*
- *"Dan isn't my boss, he's my editor at one publication. Please fix every page that says otherwise."*
- *"You couldn't read the Word files? Tell me what you need me to do."*

> **Nicer view (optional):** your wiki is just a folder of linked pages, so it works in **Obsidian**, a free notes app. Download it from **https://obsidian.md**, choose **Open folder as vault**, and pick `my-work-brain`. You'll see your pages as a clickable wiki, plus a graph of how they link. Claude keeps writing the pages; Obsidian is only for reading.

---

## Part B — Teaching Claude your judgment

The pages so far are *facts*. Facts help a little. Judgment helps a lot: *"I always cut the first paragraph because it's throat-clearing"* changes what Claude writes; *"I write about productivity"* barely does. This part is the most important part of the course.

### Step 3 — Your voice and your standards

**What this does:** Claude studies *how* you write: the patterns across your past work, the before-and-after edits, your editor's feedback and your notes on the "before" article. It turns them into rules specific enough to follow.

**Send this to Claude** (works for any job as it is):

```text
Now write my judgment pages. Use everything you've read, especially the before-and-after
edits in raw/feedback/, the feedback from other people, and baseline/before-notes.md
(where I said what was wrong with your generic attempt).

1. wiki/voice.md: how I sound. Tone, sentence and paragraph length, how I open and close,
   how I use "I" and "you", words and phrases I use, words and phrases I never use.
   Give 2–3 short real examples from my work for each rule.
2. wiki/standards.md: what "good" means to me, for each task in my work map: what makes
   the result good overall, and what makes each important part of it good (for an article:
   the idea, headline, opening and ending; for a spec: the problem, scope and success
   measures).
3. wiki/editing.md: what I change when I revise my work. Compare my before and after
   versions and name each pattern (e.g. "cuts the first paragraph", "replaces vague claims with a
   number"), with how often you saw it.
4. wiki/review-checklist.md: a checklist someone could use to review a draft the way I
   (and my editor) would, built from editing.md, standards.md and the feedback I've had.
   Most important checks first.

Rules must be specific enough to check. "Write clearly" is useless; "paragraphs of 2–4
sentences, never more than 2 one-sentence paragraphs in a row" is useful.
Where my past work and what I say disagree, note both and ask me. Mark guesses as GUESS.
Then interview me: ask 2–3 questions at a time about the guesses and disagreements, with
suggestions, and update the pages with my answers.
```

**What you should see:** after about 7 minutes, Claude has written four pages and tells you what it found by comparing your drafts with your published work, often with real counts, e.g. *"'I think' appears 11–12 times in each first draft and 0 times in every recent published piece."* Then it interviews you, about 4 rounds of 3 questions, each with options and a suggestion, for example:
- *"Where did the numbers in your published pieces come from? Your drafts say 'I didn't time the notes at first'. a) real records you checked during the edit, b) careful estimates."*
- *"Biscuit or your partner appears in the first two paragraphs of all 7 recent pieces. Is that a rule or a habit?"*
- *"When can 'maybe' stay? a) only when the sentence says what you don't know, at most twice a piece. (My suggestion.)"*

Answer with letters, e.g. *"1a. 2a. 3b."* After each round Claude updates the pages and tells you which guesses are now rules.

Answer briefly. Disagreements between your old work and what you say now are normal: your taste changes, and the wiki should follow the *current* you.

**Check it worked:**
1. Open **`wiki/voice.md`**. Read it as if you'd never met yourself. Could someone write a convincing paragraph as you from this page alone?
2. Open **`wiki/review-checklist.md`**. Are the checks the ones you (or your editor) actually make? Are the most important ones first?
3. Ask Claude: *"Which rules in voice.md come from what I said, and which did you work out from my articles?"* The ones it worked out are often the most useful: habits you didn't know you had.

**If it's not right:**
- *"This rule is too vague. Make it something you could check in a draft."*
- *"I don't always do that. It's only for my publication pieces. Please say so on the page."*
- *"You missed something big: I never use bullet points in the middle of a story."*

### Step 4 — Your visual style

**What this does:** Claude studies your images and writes down your style precisely enough to make new ones that look like yours in Lesson 4: shapes, colours, lettering, arrows, layout and how much text. Pictures beat descriptions, so this page comes from your real visuals, not from what you think they look like. For our writer, these are the diagrams in her articles.

> **Don't make visuals?** Skip to Step 5.

**Send this to Claude** (works for any job as it is):

```text
Look closely at every image in raw/visuals/ and write wiki/visual-style.md: the rules for
making a new visual that looks like mine. Use exact values wherever you can, measured from
the images, not vague words:
1. Overall look: hand-drawn or neat, background colour, image size and shape (width x height)
2. Shapes: which shapes I use (boxes, circles…), corners, line thickness, fill or no fill
3. Colours: every colour with its colour code, and what each one is used for (e.g. the
   accent colour only for the one thing that matters most)
4. Lettering: the style of font (e.g. handwritten), sizes for titles and labels, capitals
   or not
5. Arrows and lines: style, thickness, arrowheads, straight or curved
6. Layout: direction (left to right, top to bottom), spacing, how many elements
7. Text: maximum number of labels, words per label, whether there's a title
8. What my visuals are for: which kinds of ideas or content each type shows (process,
   before/after, comparison, announcement…)
   with one example image for each
9. Never: things that would make a visual look not-mine
Then show me a short summary, and list anything you're not sure about as a question.
Also link visual-style.md from voice.md and standards.md, and update index.md and log.md.
```

**What you should see:** a summary like *"Your diagrams are hand-drawn in Excalidraw, about 2000 px wide on white, with a handwritten font. Rounded boxes for steps, diamonds for decisions, circles for start and end points. You use soft pastel fills where each colour has a job: green for the first step, blue for inputs and questions, yellow for results, pink for the decision. Solid arrows always happen; dashed arrows are hand-offs or loops."*, followed by about 7 questions, e.g. *"Your flowchart uses pink for the safest answer, but your articles describe pink as 'the part to keep an eye on'. Should one fixed colour key apply to every diagram?"* or *"Should anything over 5 steps run top to bottom so it reads on a phone?"* It will also list a *never* section, including the grey 'Frame' label left on one export.

With exact measuring allowed, the colour codes are exact (the sample pack's are Excalidraw's own pastels, e.g. green `#b2f2bb`). Without it, they're marked as estimates.

**Check it worked:**
1. Open **`wiki/visual-style.md`** next to two or three of your images. Does every rule match what you see?
2. Ask Claude: *"Describe, piece by piece, how you'd make the visual idea from baseline/before.md in my style."* The description should sound like one of yours: which shapes, which colour each one gets and why, the arrows and the labels. (Claude makes real images in Lesson 4.) Don't be surprised if Claude also questions the idea itself. With the sample pack, it may point out that the diagram illustrates a different idea from the one the writer said was worth keeping, and suggest a better one.

**If it's not right:**
- *"The blue is wrong. It's lighter, like the boxes in 03-react-loop-grocery-run.png. Please measure it again."*
- *"I don't always use a title. Only when the diagram stands on its own."*

---

## Part C — The three wiki habits

Your wiki is only useful if it stays up to date, and it stays up to date only if that's easy. Each habit is one short instruction to Claude. You set them up in Step 1, so now you just use them.

### Step 5 — Add: feed it something new

**What this does:** shows what happens when new material arrives. You don't have to tell Claude which file is new: it compares `raw/` with `log.md` and finds anything it hasn't added yet. It doesn't just file it: it updates every page the new material affects, and tells you what changed.

**Do this:** copy one new file into the right `raw/` folder: a new piece of feedback, your latest piece of work, or a new idea list. For the course build, copy `later/dan-feedback-latest.txt` from the sample pack into `raw/feedback/`. It's a new email from Dan that flags something the wiki doesn't know yet.

**Send this to Claude** (works for any job as it is):

```text
add
```

(To add one particular file, name it: `add raw/feedback/dan-feedback-latest.txt`.)

**What you should see:** a short report, for example *"Dan flags an over-promising headline for the second time, so I moved that check near the top of review-checklist.md. He also asks you to stop using 'agentic' (added to voice.md under words you never use) and to add alt text to every diagram (added to visual-style.md). I updated people/dan.md and logged it."*

If the new material disagrees with something you said earlier, Claude doesn't pick a side. It keeps what the wiki says, writes the question on `judgment-notes.md` with its suggested answer, and asks you. With the sample pack, for example, Dan wants the headline check moved to the top of the checklist, but the writer said she edits the headline last. Claude may suggest a middle way: keep writing the headline last, but make "headline matches body" the first check. Answer now (*"Yes, do that"*) or later: the question waits on `judgment-notes.md` until you do.

**Check it worked:** open `wiki/log.md`. There's a new dated line for this add, naming the file and the pages that changed. Send `add` again: Claude should say there's nothing new in `raw/`.

> **Why this matters:** your wiki should never be a chore to keep up. From now on, all you do is drop files into `raw/`. You don't need to remember what's new, and you don't have to answer questions on the spot. In Lesson 5, this add runs by itself every week, and the questions come to you by email.

### Step 6 — Ask: put your wiki to work

**What this does:** questions answered from *your* wiki, not from the internet's average opinion. A good answer can be saved as a new page, so your wiki gets smarter every time you use it.

**Send this to Claude** (works for any job as it is; try one or two):

```text
ask What are the three mistakes I make most often in first drafts of my work, and how do I fix them?
```

```text
ask Rewrite the opening of baseline/before.md the way I would. Then tell me which
wiki rules you followed.
```

**What you should see:** answers that name the pages they came from (*"From editing.md and review-checklist.md…"*), with real examples from your own drafts. The rewritten opening follows your rules and lists which ones it used.

Expect **gaps in square brackets**, like *"[What you tried instead, for how long, and what you counted]"*. That's Claude obeying your wiki: it won't invent a moment or a number from your life, so it leaves a slot for you to fill. At the end, Claude may offer to save the answer as a wiki page, or the opening as a draft. Say no for now.

**Check it worked:** does the rewritten opening follow your rules (for example, a real moment from your week, no question, no banned phrases), with brackets instead of made-up facts? This is a first taste of the before-and-after comparison you'll do properly in Lesson 5.

**If it's not right:** this is where you find gaps in the wiki. Say what's off, and ask Claude to fix the *page*, not just the answer: *"That still opens too slowly. Update voice.md so this doesn't happen again, then try again."*

### Step 7 — Tidy: keep it healthy

**What this does:** Claude checks the whole wiki the way an editor checks a manuscript: contradictions between pages, claims that are out of date, pages nothing links to, and important topics with no page. It reports first and only fixes what you agree to.

**Send this to Claude** (works for any job as it is):

```text
tidy
```

**What you should see:** a report grouped into **out of date**, **disagreements** and **gaps**, then a lettered list of suggested fixes, for example:
- *"Out of date: visuals.md still says your colour meanings are unsettled, but you fixed a colour key in Step 4."*
- *"Disagreement: the review checklist fails a piece with no number in the first 4 paragraphs, but standards.md only asks for one number anywhere. The checklist is stricter than your rule."*
- *"Gap: seven questions on judgment-notes.md are still open."*

Reply with the fixes you want, e.g. *"Go ahead with A to F. Skip G for now."*

**Check it worked:** ask *"tidy"* again. The report should be shorter, with only the things waiting on you.

> **How often?** Tidy once a week, or after a big add. In Lesson 5 you'll set it to run every week by itself.

### Step 8 — Give corrections a proper home

**What this does:** in Lesson 1 Claude noted your corrections in `CHANGELOG.md` for now. Now that you have a wiki, every correction should change the page it belongs to, so the lesson is learned for good.

**Send this to Claude** (works for any job as it is):

```text
Update the rule about corrections in CLAUDE.md: from now on, when I correct you, (1) fix
the wiki page the correction belongs to (e.g. voice.md for a writing correction), quoting
my words, (2) add a dated line to wiki/log.md starting with "correction", and (3) tell me in
one sentence which page you changed. If no page fits, make one.
Then move any corrections already in CHANGELOG.md into the wiki the same way.
```

**What you should see:** Claude updates `CLAUDE.md` and moves any corrections it finds in `CHANGELOG.md` onto the right wiki pages. It may also add *your corrections* to the wiki's list of allowed sources in `CLAUDE.md`, so the two rules don't clash. That's expected.

**Check it worked:** correct Claude about something small, e.g. *"By the way, I never use the word 'hack'."* Claude should reply with one sentence like *"Added to voice.md under 'words I never use'."* Open `voice.md` to check.

---

## What you have now

- ✅ **A wiki** in `wiki/`, with `index.md` (contents) and `log.md` (diary)
- ✅ **Fact pages:** about you, who your work is for, what you work on, the people you work with, your process, one page per piece of past work
- ✅ **Judgment pages:** `voice.md`, `standards.md`, `editing.md`, `review-checklist.md` and `visual-style.md`
- ✅ **The three habits:** `add`, `ask` and `tidy`
- ✅ **Corrections that stick:** every correction now updates the right page

Start a new chat in `my-work-brain` and ask *"What do you know about how I write?"* Claude now answers from your wiki. Compare that with Lesson 1, when it knew nothing.

## Other jobs

Every prompt in this lesson works for any job as it is: Claude builds the pages from *your* material and *your* work map. What changes is what ends up in the wiki. You'll see pages like these:

| If you're a… | `voice.md` and `standards.md` cover | `visual-style.md` covers |
|---|---|---|
| Product manager | how you write specs and updates, what a good problem statement and scope look like, what engineers always ask | user flows, wireframes |
| Social media manager | brand voice per platform, hooks, hashtags, posting rules, what gets engagement | post graphics, carousel layouts, brand colours |
| Business owner | how you talk to customers, how you price and say no, what a good offer looks like | flyers, price lists, simple charts |
| Marketer | brand voice, what makes an email or ad convert for you | campaign charts, ad designs |
| Consultant | how you structure a proposal, how you size a problem, what clients push back on | framework diagrams, slide style |

## Common problems

| What you see | What to tell Claude |
|---|---|
| Claude says it can't read some files | *"Which files couldn't you read, and what should I do with them?"* (Usually re-saving as PDF fixes it.) |
| A page is full of vague words ("engaging", "clear") | *"Make every rule in this page specific enough to check in a draft."* |
| Claude answers an `ask` from general knowledge | *"Answer only from my wiki, and tell me which pages you used. If the wiki doesn't say, tell me that instead."* |
| Claude edited something in `raw/` | *"You changed a file in raw/. Please undo that and re-read the rules in CLAUDE.md."* |
| The wiki has dozens of tiny pages | *"tidy, and suggest pages to merge."* |
| `add` misses a file you put in `raw/`, or adds one twice | *"Check log.md against raw/. Which files are missing or listed twice? Fix the log, then add what's missing."* |
| You hit your usage limit during the first add | Wait for it to reset, then in the same chat say: *"Carry on with the add where you left off. Check log.md to see what's done."* |
