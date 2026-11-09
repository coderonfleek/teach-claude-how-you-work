# Lesson 4 — Skills From How You Work

## Lesson goal

By the end of this lesson you'll have:
- **five skills**, found in your own work rather than invented: for our writer, `/ideate`, `/draft`, `/diagram`, `/review` and `/publish-medium`
- **a real article made with them**: an idea picked from your calendar, drafted in your voice, with a diagram in your style, reviewed, redrafted from your reply to the review email, and saved as a **Medium draft** ready for you to publish
- a way to **test** a skill, and a rule that turns every correction into a better skill or a better wiki

**Why this lesson matters:** a skill is a job you do again and again, written down once with your standards built in. You run it by typing `/` and its name. Because every skill reads your wiki instead of keeping its own copy of your rules, improving the wiki improves every skill at once.

⏱ About **2 hours**. Claude works for about 25 minutes of that: a minute or two to build each skill, then 1–4 minutes for each run. Most of your time goes on reading what the skills make and answering their questions.

> **Usage note:** heavy, close to Lesson 2. Drafting and reviewing a full article reads several wiki pages each time. If you hit your limit, carry on in the same chat when it resets.

> **Click Allow when Claude saves a skill.** Skills live in a protected folder (`.claude`, in your home folder), so Claude asks every time it saves or changes one, even if you've already let it edit other files. If you click Deny by mistake, say *"Save the skill again, I'll allow it."*

### The five parts of this lesson

| Part | What you do | What you get |
|---|---|---|
| **A** | Find your skills, and set the rules every skill follows | A ranked list of skills, a "My skills" section in `CLAUDE.md`, and access to your second brain from any project |
| **B** | Build and run `/ideate` | New ideas added to your Notion calendar |
| **C** | Build and run `/draft`, `/diagram` and `/review` | A drafted article with a diagram, reviewed, then redrafted from your email reply |
| **D** | Build and run `/publish-medium` | The article as a Medium draft, plus a copy-and-paste fallback |
| **E** | Test a skill and correct one | Proof that a skill does its job, and a correction that sticks |

---

## Before you start

- Lessons 1–3 are done: you have a wiki, connected apps, and the *check apps* habit.
- **Using the sample pack?** Copy `practice/turn-the-ai-off-notes.md` into `raw/notes/`. It's the writer's outline notes for the article you'll write in this lesson. Then send Claude: `add raw/notes/turn-the-ai-off-notes.md`
- **Using your own work?** Pick one real piece of work you need to do this week. Put any notes you have for it into `raw/notes/` and *add* them.

Open a **new chat** in `my-work-brain` for this lesson.

---

## Part A — Finding your skills

### Step 1 — How a skill works

**What this does:** shows you where skills live before you make any. Nothing to send yet.

A skill is a **folder with one instruction file in it**, `SKILL.md`, saved in your **personal skills folder**: a hidden `.claude/skills/` folder in your home folder (on a Mac `~/.claude/skills/`, on Windows `C:\Users\<you>\.claude\skills\`). It's not inside `my-work-brain`, so **your skills work in any project you open on this computer**, not just this one. The file says:
- **what the skill is for**, in one or two sentences, so Claude knows when to use it
- **the steps**, in order
- **where your second brain is**, by its full path, and **which wiki pages to read** for the standards, e.g. `voice.md` and `review-checklist.md`
- **what it may do in your apps**, following your "My apps" rules

You run a skill by typing **`/`** in the chat box and picking it from the list, e.g. `/review`. You can add details after the name: `/review drafts/turn-the-ai-off/draft.md`.

**Do this:** type `/` in the chat box now. You'll see the commands that come with the app. After this lesson, your own five skills are in that list too.

> **Why the full path?** A chat in another project doesn't read `my-work-brain/CLAUDE.md` or your wiki on its own. So every skill starts by reading them from their full path, and saves its work in `my-work-brain/drafts/`, wherever you run it from. In Step 3 you also give every project permission to open `my-work-brain`. If you ever move or rename `my-work-brain`, tell Claude: *"I moved my second brain to [new place]. Update my skills."*

> **For the technical:** skills are Claude Code Agent Skills. Personal skills live in `~/.claude/skills/<name>/SKILL.md` and load in every project; project skills in `<project>/.claude/skills/` load only there. Each has YAML front matter (`name`, `description`) and Markdown instructions. Claude loads only the description until the skill is used, so having many skills costs almost nothing.

### Step 2 — Let Claude find your skills

**What this does:** instead of you guessing which skills to build, Claude looks at your work map, your wiki and your corrections, and finds the jobs you actually repeat. It ranks them by the time they'd save you.

**Send this to Claude** (works for any job as it is):

```text
Find the skills I should build. Read work-map.md, wiki/process.md, the judgment pages
(standards, editing, review checklist, visual style), wiki/feedback-history.md (or the
page with feedback I've had) and any corrections in wiki/log.md.
List the jobs I do again and again. For each one:
- a short skill name (one word, lower case, e.g. "review")
- what it does, in one sentence
- what it starts from and what it produces
- which wiki pages it should read
- which apps it uses, and what it may do there (from "My apps" in CLAUDE.md)
- how I'd know it did a good job
Rank them by how much time they'd save me each week, and say which you'd build first.
Don't build anything yet.
```

**What you should see:** a ranked table of 5–7 skills, each with an estimate of the time it saves and the numbers behind it. Claude's names and groupings won't match this lesson exactly. In the dry run it suggested `ideas`, `edit`, `diagram`, `review`, `memos`, `prepublish` and `dan`, and folded memo sorting into the ideas skill. The jobs are the same; the names are yours to choose.

Then tell Claude which ones you want. Building comes next, one skill at a time.

**Send this to Claude** (two versions, pick one):

**Course build (writer):**

```text
Let's build five: ideate (fold the memo sorting into it), draft (a first draft from my
notes, so I start by editing instead of staring at a blank page, plus a redraft mode),
diagram, review, and publish-medium. Keep the others for later.
Don't build them yet: we'll build them one at a time.
```

**Your own work:**

> **Fill in:** the 4–6 skills from Claude's list that you want first, by name, plus anything you'd like merged or renamed.

```text
Let's build these: [SKILL NAMES]. Keep the others for later.
Don't build them yet: we'll build them one at a time.
```

These are the five the course builds:

| Skill | What it does |
|---|---|
| `/ideate` | Suggests what to write next from the calendar, voice memos and reader comments, scored against the writer's test for a good idea, and adds the chosen ones to Notion |
| `/draft` | Turns an idea and notes into an outline, then a first draft in the writer's voice. Also **redrafts** after a review |
| `/diagram` | Makes a diagram image in the writer's style, with alt text |
| `/review` | Checks a draft against the review checklist, saves the notes and emails them to the writer |
| `/publish-medium` | Puts the finished article into Medium as a draft. Never publishes |

A digest of Dan's feedback is a good one to keep for Lesson 5.

**Check it worked:** is each job one you really do? Is the top one the job that wastes most of your week? (For the writer, it's picking ideas on Monday.)

**If it's not right:** *"You missed [a job]. I do it every week."* or *"Merge draft and redraft into one skill."*

### Step 3 — Rules every skill follows

**What this does:** writes the house rules for skills into `CLAUDE.md`, once, so you don't repeat them in every skill. The most important one is the last: when you correct a skill's work, Claude decides where the fix belongs, and makes it there. A rule about *your work* goes in the wiki, so every skill learns it. A rule about *how the skill works* goes in that skill.

**Send this to Claude** (works for any job as it is):

```text
Add a "My skills" section to CLAUDE.md, in plain words:
1. Skills live in my personal skills folder, ~/.claude/skills/<name>/SKILL.md, not in
   this folder, so I can use them in any project on this computer. Each one says what
   it's for, its steps, which wiki pages it reads, and what it may do in my apps.
2. Because a skill may run from another project, every skill starts by reading this
   folder's CLAUDE.md by its full path, and uses full paths for the wiki, raw/ and
   drafts/. Its work always goes in this folder, wherever I run it from.
3. Skills read my wiki pages for my standards. They never copy rules out of the wiki,
   so when the wiki improves, every skill improves.
4. Skills follow the "My apps" rules, and ask before anything that creates or sends.
5. Skills never make up facts about my life or work: no invented moments, numbers,
   names or quotes. If something's missing, leave a gap in [square brackets] and tell me.
6. Work in progress goes in drafts/<short-name>/, one folder per piece of work. Never
   overwrite an earlier version: save the next one alongside it (draft-2.md, draft-3.md…).
7. Every skill ends with a short list: which wiki pages and rules it followed, and
   anything it wasn't sure about.
8. When I correct a skill's output, decide where the fix belongs: a rule about my work
   goes on the right wiki page, and a change to the steps goes in the skill. Make the
   fix, add a line to CHANGELOG.md, and tell me in one sentence where it went.
Add a line to CHANGELOG.md too.
```

**What you should see:** Claude adds the section and confirms in a few bullets, including the folder's full path it wrote into rule 2.

**Check it worked:** open `CLAUDE.md`. There's a **My skills** section with all eight rules.

**Then let your other projects reach this folder.** Out of the box, a chat in one project can only open that project's files. In the dry run, `/review` run from a client project stopped at its first step because it wasn't allowed to read `my-work-brain`. This one-time setting fixes that for every project on your computer.

**Send this to Claude** (works for any job as it is):

```text
So my skills can reach this folder from any project, add this folder's full path and my
personal skills folder (~/.claude/skills) to "additionalDirectories" in my user settings
(~/.claude/settings.json). Keep everything else in that file as it is. Before you change
it, tell me in one sentence what this does.
```

**What you should see:** a one-sentence explanation, something like *"Every chat on this computer will be able to open files in my-work-brain and your skills folder, wherever it starts."* Then Claude asks to change your settings file: click **Allow**.

> **Only do this for your second brain.** It lets every project read the folder, which is the point. Don't add folders with things other projects shouldn't see.

---

## Part B — `/ideate`

### Step 4 — Build `/ideate`

**What this does:** builds the skill for the job the writer said costs her most: picking what to write on Monday ("64 minutes to pick two ideas").

**Send this to Claude** (two versions, pick one):

**Course build (writer):**

```text
Build a skill called "ideate". When I run /ideate, it should:
1. Read my Notion "Content calendar", my voice memos in raw/notes/, reader comments in
   raw/feedback/, and wiki/ideas.md.
2. Suggest 3–5 ideas to write next. Include ideas already on the calendar (status Idea
   or Outlining) and up to 2 new ones it found in my notes or comments.
3. Score each one against my test for a good idea in wiki/standards.md, in a small table
   with a one-line reason per idea. Flag anything too close to a piece I've already
   written.
4. Ask me which new ideas to add to the calendar. Add only the ones I pick, as new rows
   with status Idea and a one-line note. Never change rows that are already there.
5. End with the list of pages and rules it followed.
Then show me the skill in plain words, not the file.
```

**Your own work:**

> **Fill in:**
> `[WHAT I PLAN]` → PM: *which features to spec next* · Social media manager: *next week's posts* · Business owner: *this month's offers*
> `[WHERE MY LIST LIVES]` → *my Notion roadmap* · *the content calendar in Google Drive* · *my Notion "Offers" page*
> `[OTHER SOURCES]` → *customer feedback in raw/feedback/* · *comments on last week's posts* · *emails from customers*

```text
Build a skill called "ideate". When I run /ideate, it should:
1. Read [WHERE MY LIST LIVES], [OTHER SOURCES], and the wiki page about my ideas or
   plans.
2. Suggest 3–5 options for [WHAT I PLAN]. Include ones already on my list and up to 2
   new ones it found in my notes or feedback.
3. Score each one against my standards in the wiki, in a small table with a one-line
   reason per option. Flag anything too close to something I've already done.
4. Ask me which new ones to add to [WHERE MY LIST LIVES]. Add only the ones I pick, as
   new items with a one-line note. Never change items that are already there.
5. End with the list of pages and rules it followed.
Then show me the skill in plain words, not the file.
```

**What you should see:** Claude asks to save `~/.claude/skills/ideate/SKILL.md` (click **Allow**) and explains the skill back step by step. Expect it to have thought of details you didn't ask for, e.g. *"New ideas must come from one memo or comment. It never merges two into one."*

**Check it worked:** type `/` in the chat box. **ideate** is in the list. (If it isn't, open a new chat and try again.)

### Step 5 — Run `/ideate`

**Send this to Claude** (works for any job as it is):

```text
/ideate
```

**What you should see:** Claude reads your calendar (click **Allow**), then shows a table like this:

| Idea | From | Score | Too close? | Why |
|---|---|---|---|---|
| What an AI agent costs per week | Outlining | 8/8 | No | Tracking until 22 Nov, draft due to Dan 30 Nov |
| When to turn the AI off | Outlining | 8/8 | Near the Sep planner piece, but a new angle | Real moment, timed numbers, outline done |
| Notes nobody reads back | Idea | 7/8 | No | You planned to ask two more people first |
| *New:* How much does the check step really help? | Daniel's comment | 5/8 | **Yes:** the May loop piece | A fair challenge, but no moment or number yet |
| *New:* What I draw my diagrams in | Grace's comment | 6/8 | No | Readers ask, but would a team lead care? |

It also says why it left the other ideas off ("Need two weeks of data first"), and saves the shortlist in `drafts/`. Then it asks which new ideas to add. Pick one, e.g. *"Add the first new one."* Claude asks to create a row in Notion: click **Allow**.

**Check it worked:**
1. In Notion, the new idea is a new row with status **Idea**. No other rows changed.
2. Did it flag the idea that's too close to something you've written?

**If it's not right:**
- *"Two of these are listicles. My standards say I don't write those. Why did they get through?"* (Claude should fix the skill or the wiki, and tell you which.)
- *"Show the scores as ticks, not numbers out of 10."*

For the rest of this lesson, pick an idea you have notes for. With the sample pack, that's **When to turn the AI off**: the writer's notes for it are the file you added before the lesson.

---

## Part C — `/draft`, `/diagram` and `/review`

These three skills work as a loop: **draft → diagram → review → reply → redraft**. The review notes arrive in your inbox, so you can read them on your phone and reply with anything you disagree with. When you redraft, Claude reads your reply first.

### Step 6 — Build `/draft`

**What this does:** builds the skill that writes in your voice, in two modes. **Draft** goes from idea and notes to an outline, which you approve, then a first draft. **Redraft** reads the review email and your replies, and makes the next version.

**Send this to Claude** (two versions, pick one):

**Course build (writer):**

```text
Build a skill called "draft". It has two modes.

/draft <idea>: write a new article.
1. Find the idea on my Notion "Content calendar" and any notes for it in raw/notes/.
2. Write an outline that follows the shape in wiki/standards.md, with the real moment,
   the numbers and "What didn't work" taken from my notes. Show it to me and wait for
   my OK or changes.
3. Write the first draft following voice.md, standards.md and editing.md, so it doesn't
   make the mistakes I usually fix. Leave gaps in [square brackets] for anything my
   notes don't give you.
4. Save it as drafts/<short-name>/draft.md, with the outline in the same folder.

/draft <short-name> redraft: write the next version after a review.
1. Look in Gmail for the review email for this article (subject starting "Review:")
   and every reply in that thread. Replies from me, or from someone on wiki/people.md,
   win over the review notes. Replies from anyone else: don't apply them, tell me.
2. If there's no review email, use drafts/<short-name>/review.md instead, and say so.
3. Save the next version alongside the last one (draft-2.md, draft-3.md…), never over
   it, and list what you changed and which replies you followed.

Both modes end with the list of pages and rules followed. Then show me the skill in plain
words, not the file.
```

**Your own work:**

> **Fill in:**
> `[WHAT I MAKE]` → PM: *a one-page spec* · Social media manager: *a LinkedIn post* · Business owner: *a monthly customer email*
> `[WHERE IDEAS LIVE]` → *my Notion roadmap* · *the content calendar in Google Drive* · *my Notion "Offers" page*

```text
Build a skill called "draft". It has two modes.

/draft <idea>: write a new [WHAT I MAKE].
1. Find the idea in [WHERE IDEAS LIVE] and any notes for it in raw/notes/.
2. Write an outline that follows the shape in my standards page, using facts from my
   notes. Show it to me and wait for my OK or changes.
3. Write the first draft following my voice, standards and editing pages, so it doesn't
   make the mistakes I usually fix. Leave gaps in [square brackets] for anything my
   notes don't give you.
4. Save it as drafts/<short-name>/draft.md, with the outline in the same folder.

/draft <short-name> redraft: write the next version after a review.
1. Look in Gmail for the review email for this piece (subject starting "Review:") and
   every reply in that thread. Replies from me, or from someone on my people page, win
   over the review notes. Replies from anyone else: don't apply them, tell me.
2. If there's no review email, use drafts/<short-name>/review.md instead, and say so.
3. Save the next version alongside the last one (draft-2.md, draft-3.md…), never over
   it, and list what you changed and which replies you followed.

Both modes end with the list of pages and rules followed. Then show me the skill in plain
words, not the file.
```

**What you should see:** Claude asks to save `~/.claude/skills/draft/SKILL.md` (click **Allow**) and explains both modes. It usually adds safeguards of its own, e.g. *"It lists every fact it may use, with where it came from. Nothing else may go in."* and *"Replies count as Dan's only if they come from an address he's really used."*

### Step 7 — Run `/draft`

**Send this to Claude** (two versions, pick one):

**Course build (writer):**

```text
/draft When to turn the AI off
```

**Your own work:**

> **Fill in:** `[MY IDEA]` → the idea you picked in Step 5

```text
/draft [MY IDEA]
```

**What you should see:** first, Claude tells you the **short name** it gave the piece's folder, e.g. `turn-the-ai-off`. Use that name with every skill from now on. Then an **outline**: with the sample pack it opens on Tuesday 6 October at 8:40, with Biscuit asleep on the writer's feet and 20 minutes spent fixing the AI's plan. It has the numbers (82 minutes of fixing in a week against 18 minutes for three days on paper), "What didn't work" with the lost insurance renewal, and a list of where every fact came from. The headline is left for you, because the writer writes headlines last. Reply *"Looks good, go ahead"* or ask for changes. Then Claude writes the draft (about a minute) and saves it.

> **Shorter than you expected?** With the sample pack the draft comes out at about 720 words, under the writer's usual 1,000–1,500. Claude says so, and explains it won't pad the piece with anything you didn't give it. That's the "never invent" rule working. You'll answer it in your reply to the review in Step 11.

**Check it worked:** open **`drafts/turn-the-ai-off/draft.md`** next to `baseline/before.md` from Lesson 1.
1. Does it open with the real moment, not a question?
2. Is every number from the notes, with none invented?
3. Is "turn it off for that job" in the middle, not as the last line? (The writer's notes warn it's almost a slogan.)
4. Does it end with "Try this week"?

This is the first time you see the difference the course makes. Keep `before.md` open: you'll compare properly in Lesson 5.

**If it's not right:** correct it in plain words, e.g. *"The opening is too long. I'd start at 'Twenty minutes.'"* Claude fixes the draft *and*, following your skill rules, says where the lesson went: *"Added to editing.md: start the opening at the number."*

### Step 8 — Build and run `/diagram`

**What this does:** makes a picture in your visual style for the piece you're working on, ready to put in Medium. Claude plans the diagram in words first and waits for your OK, because changing a plan is quicker than changing a picture.

**Send this to Claude** (two versions, pick one):

**Course build (writer):**

```text
Build a skill called "diagram". When I run /diagram <short-name>, it should:
1. Read the draft in drafts/<short-name>/ and wiki/visual-style.md.
2. Pick the one idea in the piece that a diagram explains best, and plan the diagram in
   words: each shape, its label, its colour and why, and the arrows. Show me the plan and
   wait for my OK.
3. Make it as a PNG image that follows visual-style.md as closely as possible (size,
   white background, hand-drawn look, handwritten lettering, colour key, arrows). Use
   whatever works on this computer, ask me before installing anything, and write down in
   the skill how you did it so it's the same next time.
4. Save it as drafts/<short-name>/diagram-1.png (diagram-2.png for a second one), and
   write its alt text in drafts/<short-name>/diagrams.md: at most two sentences saying
   what goes where and what the arrows mean.
5. Show me the image, then list the style rules it followed and any it couldn't.
Then run it for turn-the-ai-off.
```

**Your own work:**

> **Fill in:** `[MY VISUAL]` → PM: *a user flow* · Social media manager: *a post graphic* · Business owner: *a simple flyer* · Consultant: *a framework diagram*
> `[WHERE IT GOES]` → *in my spec* · *on LinkedIn* · *in my shop window* · *in my proposal*

```text
Build a skill called "visual". When I run /visual <short-name>, it should:
1. Read the work in drafts/<short-name>/ and wiki/visual-style.md.
2. Decide what [MY VISUAL] for this piece should show, and plan it in words: each
   element, its text, its colour and why. Show me the plan and wait for my OK.
3. Make it as a PNG image that follows visual-style.md as closely as possible, ready to
   use [WHERE IT GOES]. Use whatever works on this computer, ask me before installing
   anything, and write down in the skill how you did it so it's the same next time.
4. Save it as drafts/<short-name>/visual-1.png, and write its alt text in
   drafts/<short-name>/visuals.md: at most two sentences describing it.
5. Show me the image, then list the style rules it followed and any it couldn't.
Then run it for <short-name of the piece I'm working on>.
```

**What you should see:** Claude works out how to make images on your computer (it may ask to run a few commands: click **Allow**), creates the skill, and then shows a plan as a small table: *"A pink diamond, label above it: 'Fixing Takes Longer?'. Yes → a white rounded box: 'Turn It Off'. No → a white rounded box: 'Keep It'. Dashed lines from both back up to the diamond: 'In a Month'."* It also lists where the plan bends one of your rules and asks you to choose, e.g. *"Your question is 7 words but your labels are 1–3 words. Shorten it to 'Fixing Takes Longer?'"* Reply *"OK to all four"* or choose differently. Then it draws the PNG (about 1–2 minutes) and checks it against one of your old diagrams.

> **How Claude makes the image:** in the dry run on a Mac, it wrote a small drawing script using Python and the Mac's built-in **Chalkboard SE** handwriting font, and saved the script inside the skill's folder so every diagram is made the same way. On another computer it may need to install something first (for example Python's image library): it asks before it does. A skill's folder can hold helper files like this alongside `SKILL.md`.

**Check it worked:** open the new image next to one of your old ones from `raw/visuals/`.
1. Same feel: white background, hand-drawn look, handwritten lettering?
2. Colours used the way your colour key says?
3. Short labels? Alt text in `diagrams.md`, two sentences at most?

It won't be pixel-identical to a hand-made Excalidraw drawing. In the dry run, the shapes, colours, wobbly lines and arrowheads matched closely, and the lettering was the main difference: neater than Excalidraw's. It should look like it belongs in the same article. Next to the image, Claude also saves the plan (`diagram-1.json`), so the diagram can be redrawn exactly after a correction.

> **Want closer lettering?** Ask Claude: *"Can you use Excalidraw's own handwriting font? It's free. Tell me where you'd download it from before you do."*

**If it's not right:** say what's off, e.g. *"The lines are too neat. Mine wobble a little."* or *"Too much text in the boxes: three words max."* A rule about your style goes into `visual-style.md`, and a fix to how the image is made goes into the skill. Claude tells you which.

### Step 9 — Build `/review`

**What this does:** reviews a draft the way you (or your editor) would, using your checklist in order. The notes are saved in the article's folder **and** emailed to you, so you can read them away from your desk and reply.

**Send this to Claude** (two versions, pick one):

**Course build (writer):**

```text
Build a skill called "review". When I run /review <short-name>, it should:
1. Read the newest draft in drafts/<short-name>/, its diagrams and alt text, and
   wiki/review-checklist.md, voice.md, standards.md and visual-style.md.
2. Go through the checklist in order. Report only what fails or is borderline, as
   numbered notes, most important first. Each note quotes the draft, says which rule
   it breaks, and suggests a fix. Never rewrite the draft itself.
3. Finish with a one-line verdict: ready for Dan, one more pass, or needs work.
4. Save the notes as drafts/<short-name>/review.md.
5. Ask me, then email the notes to my own address only, with the subject
   "Review: <article title>", so I can reply from my phone.
6. End with the list of pages and rules it followed.
Then show me the skill in plain words, not the file.
```

**Your own work:**

> **Fill in:** `[REVIEWER]` → whoever reviews your work: *my manager* · *the client* · *my business partner* · *me*

```text
Build a skill called "review". When I run /review <short-name>, it should:
1. Read the newest version in drafts/<short-name>/, any visuals and alt text, and my
   review checklist, voice, standards and visual style pages.
2. Go through the checklist in order. Report only what fails or is borderline, as
   numbered notes, most important first. Each note quotes the work, says which rule
   it breaks, and suggests a fix. Never rewrite the work itself.
3. Finish with a one-line verdict: ready for [REVIEWER], one more pass, or needs work.
4. Save the notes as drafts/<short-name>/review.md.
5. Ask me, then email the notes to my own address only, with the subject
   "Review: <title>", so I can reply from my phone.
6. End with the list of pages and rules it followed.
Then show me the skill in plain words, not the file.
```

**What you should see:** Claude asks to save `~/.claude/skills/review/SKILL.md` (click **Allow**) and explains it back.

### Step 10 — Run `/review`

**Send this to Claude** (works for any job as it is; use your own short name):

```text
/review turn-the-ai-off
```

**What you should see:** a numbered list of notes, most important first, each with a quote, the rule and a fix, for example *"2. 'it still got Tuesday wrong, but less often.' Check 7, fail: 'less often' has no number. Give the count from your records, or cut 'but less often'."* With the sample pack, expect about 9 notes, including the length and the missing headline, and *"23 of 33 checks passed. Verdict: one more pass."* Then Claude asks before emailing, and names the address it will send to. Check it's yours, reply *"Yes, send it"* and click **Allow**.

**Check it worked:**
1. `drafts/turn-the-ai-off/review.md` exists.
2. The "Review: …" email is in your Gmail inbox.
3. The draft itself hasn't changed.

**If it's not right:** *"Note 4 is wrong: 'Biscuit asleep on my feet' is a real detail, not decoration. Update the checklist so it stops flagging real details."*

### Step 11 — Reply, then redraft

**What this does:** the full loop. You answer the review the way you'd answer an editor, and `/draft` picks up your answer.

**Do this:** open the "Review: …" email in Gmail, on your phone if you like, and **reply** to it. Agree with most notes, but **disagree with at least one**, so you can check that Claude follows you and not the note. For example:

> *Keep "This isn't an anti-AI piece", it's my line and it stays. Skip the length note: this is a short own-profile piece, 700-ish words is fine for my profile. For note 2, cut "but less often". Headline: I Went Back to Paper for Three Days. Even My AI Planner's Best Day Lost. Subtitle: Fixing its plans took 82 minutes in a week. Planning on paper took 18 minutes for three days. Everything else: yes.*

(This is the reply from the dry run, in the sample pack's `sample-answers.md`. Change the note numbers to fit the notes you actually got.)

**Send this to Claude** (works for any job as it is; use your own short name):

```text
/draft turn-the-ai-off redraft
```

**What you should see:** *"Both messages in the thread came from your own address: my review and your reply at 17:31. Saved as draft-2.md."* Then a list of what changed, each marked with where it came from (*"your reply"* or *"note 3"*), and a list of what was **kept on purpose** because your reply said so, e.g. *"'This isn't an anti-AI piece.' You said it's my line and it stays."*

Claude may also spot that something in your reply is a **rule**, not a one-off, and offer to save it. In the dry run: *"'700-ish words is fine for my profile' sounds like a rule about your work. Shall I update the length rule on standards.md and review-checklist.md?"* Say yes. Claude saves your reply into `raw/feedback/` first, then updates the wiki, so the next review won't flag it.

**Check it worked:**
1. `draft-2.md` exists, and `draft.md` is unchanged.
2. The note you disagreed with was **not** applied.

> **What if the email isn't there?** Claude says *"No review email found, so I used review.md"* and carries on. The loop never depends on your inbox.

> **Want a second opinion?** Run `/review` again on draft 2. A shorter list of notes means the redraft worked.

---

## Part D — `/publish-medium`

### Step 12 — Build `/publish-medium`

**What this does:** puts the finished article into Medium as a **draft**, using the browser pane you signed in to in Lesson 3. It does a final check first, and it **never presses Publish**: you read the draft in Medium and publish it yourself. If the browser route doesn't work, it falls back to a page you copy and paste.

**Send this to Claude** (two versions, pick one):

**Course build (writer):**

```text
Build a skill called "publish-medium". When I run /publish-medium <short-name>, it should:
1. Take the newest draft in drafts/<short-name>/ and run a final check: no [square
   brackets] left, headline matches the body, every diagram has alt text. If anything
   fails, stop and tell me.
2. Make drafts/<short-name>/medium-ready.html: the article formatted for Medium (title,
   subtitle, headings, bold, links), with a clear line like "[IMAGE: diagram-1.png]"
   where each diagram goes.
3. In the browser pane, open a new story on Medium and put in the title, subtitle and
   article with its formatting. Try opening medium-ready.html in the pane, copying it
   all and pasting it into the story; if that doesn't work, type it in.
4. Leave each [IMAGE] line where it is, and tell me which file to drag in at each one.
   After I've added them, add each image's alt text from diagrams.md.
5. Never press Publish. Stop with the story saved as a draft, and tell me where to find
   it.
6. If Medium isn't working in the browser pane (signed out, blocked, or the editor
   misbehaves), stop and give me the fallback instead: open medium-ready.html, select
   all, copy, paste into a new Medium story, and drag in the images.
Then show me the skill in plain words, not the file.
```

**Your own work:**

> **Fill in:** `[WHERE I PUBLISH]` → PM: *Confluence* · Social media manager: *LinkedIn* · Business owner: *my Mailchimp newsletter* · Consultant: *Google Docs, to send to the client*
> `[SKILL NAME]` → e.g. *publish-linkedin*, *publish-newsletter*

```text
Build a skill called "[SKILL NAME]". When I run /[SKILL NAME] <short-name>, it should:
1. Take the newest version in drafts/<short-name>/ and run a final check: no [square
   brackets] left, and every visual has alt text. If anything fails, stop and tell me.
2. Make drafts/<short-name>/ready.html: the work formatted for [WHERE I PUBLISH], with
   a clear line like "[IMAGE: visual-1.png]" where each visual goes.
3. Put it into [WHERE I PUBLISH] as a draft: with a connected app if I have one, or in
   the browser pane if not. Never publish, post, schedule or send it.
4. Tell me which file to add at each [IMAGE] line, and add the alt text after I have.
5. Stop with it saved as a draft, and tell me where to find it.
6. If that doesn't work, stop and give me the fallback: open ready.html, select all,
   copy and paste it into [WHERE I PUBLISH] myself.
Then show me the skill in plain words, not the file.
```

**What you should see:** Claude asks to save `~/.claude/skills/publish-medium/SKILL.md` (click **Allow**) and explains it back, including the fallback.

### Step 13 — Run `/publish-medium`

**Do this first:** make sure you're still signed in to Medium in the browser pane (ask Claude *"Open medium.com in the browser pane"*). If not, sign in yourself, as in Lesson 3.

**Send this to Claude** (works for any job as it is; use your own skill and short name):

```text
/publish-medium turn-the-ai-off
```

**What you should see:** the final check, with its working shown, e.g. *"'Best Day Lost' = 11 minutes against 7. '82 minutes' = the body's 1 hour 22 minutes."*, and `medium-ready.html` saved. Claude asks before it opens Medium: say *"Yes, go ahead."* Then you watch Claude open a new story and put the article in. It stops at each `[IMAGE]` line and tells you which file to drag in from `drafts/turn-the-ai-off/`. When you say *"Images are in"*, Claude adds the alt text and ends with *"Saved as a draft. Nothing was published."*

**Check it worked:**
1. In Medium, the story is under **Drafts**, not **Published**.
2. Headings, bold and links look right.
3. Click the diagram: its alt text is there.

**Using the sample pack?** Don't publish it: it's the sample writer's article, not yours. Delete the draft in Medium yourself (**⋯** → **Delete story**).

> **If you got the fallback instead:** open `medium-ready.html` from the file pane, select all (**Cmd+A** on Mac, **Ctrl+A** on Windows), copy, and paste into a new Medium story. Formatting comes with it. Drag the images in where the `[IMAGE]` lines are.

---

## Part E — Testing and improving your skills

### Step 14 — Test a skill

**What this does:** checks that a skill does its job on work where you already know the right answer. For `/review`, that's your past work: the old pieces that break your current rules should fail, and your best recent piece should mostly pass. Where your editor's real feedback exists, the skill should catch what they caught.

**Send this to Claude** (two versions, pick one):

**Course build (writer):**

```text
Test the review skill without sending any emails or saving review files.
Run its checks on these three pieces from raw/past-work/:
- 2022-09-ai-tools-that-will-change-how-you-work.md (should fail badly: it's a listicle)
- 2023-02-inbox-zero-is-a-lie.md (should fail: question opening, slogan ending)
- 2026-09-i-let-one-ai-plan-my-week.md (should mostly pass)
For the third one, compare its notes with what Dan actually said about it in
raw/feedback/. Give me a short table: piece, verdict, top 3 notes, and whether it caught
what Dan caught. Then tell me what you'd change in the skill or the checklist, and
don't change anything until I say.
```

**Your own work:**

> **Fill in:** `[OLD PIECE]` → something you'd do differently now · `[GOOD PIECE]` → one of your best recent pieces · `[FEEDBACK]` → the feedback file about one of them, if you have one

```text
Test the review skill without sending any emails or saving review files.
Run its checks on these pieces:
- raw/past-work/[OLD PIECE] (should fail)
- raw/past-work/[GOOD PIECE] (should mostly pass)
Compare its notes with what was actually said in raw/feedback/[FEEDBACK].
Give me a short table: piece, verdict, top 3 notes, and whether it caught what the real
feedback caught. Then tell me what you'd change in the skill or the checklist, and
don't change anything until I say.
```

**What you should see:** a table where the old pieces fail for the right reasons (*"not one idea: 10 numbered tools"*, *"opens with a question"*, *"ends on a bold slogan"*) and the good piece gets *"one more pass"* with small notes. For the planner piece, Claude puts Dan's original problems back in to test them, and catches both: the headline promising "10 hours" when the body adds up to about 2.5, and the slogan ending.

Then it suggests improvements, numbered, e.g. *"Always re-add any total in the headline. Catching Dan's '10 hours' depended on me adding up the four Mondays."* and *"List fails before borderline notes."* Approve the ones you agree with: *"Do 1, 2 and 3."*

> **Testing other skills:** the same idea works for each one. Give `/ideate` your parked ideas: it should score them low, for the reasons you parked them. Give `/diagram` an article you already drew a diagram for: does its plan look like yours?

### Step 15 — Correct a skill, and watch where the fix goes

**What this does:** shows rule 8 from Step 3 at work. Corrections are how skills get better, and each one lands in the right place.

**Send this to Claude** (works for any job as it is; send one or both):

```text
From now on, when /ideate shows its table, put the idea I should write first in bold.
```

```text
The diagram's labels are too small to read on a phone. Make them bigger in every
diagram from now on.
```

**What you should see:** one sentence for each, saying where the fix went:
- *"That's about how the skill works, so I added it to the ideate skill."*
- *"That's a rule about your diagrams, so I added it to visual-style.md. The diagram skill reads that page every time, so it needed no change."*

Claude also checks the work it already made against the new rule, and tells you if anything needs redoing.

**Check it worked:** open `CHANGELOG.md`. There's a dated line for each correction.

---

## What you have now

- ✅ **Five skills** in your personal skills folder, found in your work, all reading the same wiki, and ready in any project
- ✅ **An idea added to your Notion calendar** by `/ideate`
- ✅ **A drafted, reviewed and redrafted article**, with a diagram in your style and alt text, in `drafts/`
- ✅ **A review that reached your inbox**, and a redraft that followed your reply
- ✅ **A Medium draft**, put there by Claude and published (or deleted) by you
- ✅ **A tested skill**, and corrections that land in the right place

Type `/` in a new chat. Your five skills are there, **in any folder**: try it in a chat started somewhere else. In the dry run, `/review turn-the-ai-off` run from a client's newsletter project still read the wiki, saved its notes in `my-work-brain/drafts/` and left the client's folder alone. In Lesson 5 some of your skills start running by themselves.

## Other jobs

Every role ends up with a similar set: something to choose the work, something to make it, something to check it, and something to get it out. Ask Claude for its own suggestions in Step 2: they'll fit your work better than these.

| If you're a… | Choose | Make | Check | Get it out |
|---|---|---|---|---|
| Product manager | `/prioritise`: ranks requests from feedback | `/spec`, `/flow` (user flow image) | `/review`: against your spec checklist | `/publish-confluence`, or Notion |
| Social media manager | `/ideate`: next week's posts | `/post`, `/graphic` | `/review`: brand voice, platform rules | `/publish-linkedin`: a draft or scheduled post, never live |
| Business owner | `/offers`: what to promote this month | `/email`, `/flyer` | `/review`: tone, prices, promises | `/publish-newsletter`: draft in your email tool |
| Marketer | `/ideate`: campaign angles | `/ad-copy`, `/chart` | `/review`: claims, brand, legal checks | Draft in your ad tool or email tool |
| Consultant | `/scope`: which problem to tackle first | `/proposal`, `/framework` | `/review`: against your proposal checklist | Google Docs draft for the client |

## Common problems

| What you see | What to tell Claude, or do |
|---|---|
| Claude says it couldn't save the skill | You probably clicked **Deny**, or missed the prompt. *"Save the skill again, I'll allow it."* |
| Your skill isn't in the `/` list | Open a new chat. If it's still missing: *"Check that the review skill is saved in my personal skills folder, ~/.claude/skills/review/SKILL.md."* |
| A skill run from another project says it can't read your second brain | The setting at the end of Step 3 is missing. *"Add my second brain's full path and ~/.claude/skills to additionalDirectories in my user settings."* Then open a new chat |
| A skill run from another project can't find your wiki, or saves its work in the wrong place | *"Make every skill read my second brain's CLAUDE.md by its full path, and save its work in my second brain's drafts/."* |
| A skill copied rules from the wiki into itself | *"Don't copy rules into the skill. Point it at the wiki page instead."* |
| The draft has facts you never gave it | *"Where did that come from? My skill rules say never invent facts. Fix the draft and tell me why it happened."* |
| `/draft` left lots of [square brackets] | That's the rule working: your notes didn't have those facts. Fill them in, or add more notes to `raw/notes/` and *add* them |
| `/diagram` can't make an image | *"What would you need to make a PNG on this computer? Explain it simply before installing anything."* On Windows this may mean installing Python, which Claude can walk you through |
| A skill says it can't find your folder | Skills use the short folder name Claude gave the piece in Step 7, e.g. `turn-the-ai-off`. *"Which folders are in drafts/?"* |
| The diagram doesn't look like yours | Compare them side by side and say what's different, one thing at a time: lines, lettering, colours, spacing |
| `/review` flags things you're happy with | *"Note 3 is wrong for me because [reason]. Update the checklist."* |
| The review email didn't arrive | Check **Spam**. Then: *"Did you send it? If sending failed, make it a draft to me instead."* |
| `/draft redraft` ignored your reply | *"Search Gmail for the thread starting 'Review:' for this article, including replies, and try again."* |
| `/publish-medium` got stuck in the editor | Take over in the browser pane, or ask for the fallback: *"Give me the copy-and-paste version instead."* |
