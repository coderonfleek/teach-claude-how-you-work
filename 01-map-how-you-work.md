# Lesson 1 — Map How You Work

## Lesson goal

By the end of this lesson you'll have:
- a **project folder** for your second brain, with a simple set of standing instructions for Claude
- a **"before" test**: a piece of work Claude did for you *knowing nothing about you* (for our writer, an article), plus your honest notes on what's wrong with it
- a **work map**: one page describing your work, the tools you use, what "good" means to you, and what you'd like Claude to take off your hands
- a **gathering list**: exactly what to collect before Lesson 2

**Why this lesson matters:** most people jump straight to building skills and end up with generic ones. The work map tells you *what* to put in your second brain, *which* apps to connect and *which* skills are worth building. Every later lesson starts from it.

⏱ About **40 minutes with the sample pack**, or **about 1 hour with your own work**. Claude only works for about 4 minutes in total; the rest is you reading what it wrote and answering its questions. The work-map interview takes longest: about 3 rounds of questions with the sample pack, and 5–8 rounds when Claude starts from scratch.

Collecting the material on your gathering list (Step 6) is homework before Lesson 2, and isn't included. Allow another 30–60 minutes for it with your own work. With the sample pack there's nothing to collect.

> **Usage note:** this is a light lesson for Claude usage. If you do hit your limit, just continue in the same chat when it resets.

### The three parts of this lesson

| Part | What you do | What you get |
|---|---|---|
| **A** | Set up your project folder | `my-work-brain` with folders, `CLAUDE.md` and `CHANGELOG.md` |
| **B** | Run the "before" test | `baseline/before.md`, the work you'll compare against in Lesson 5 |
| **C** | Do the work-map interview | `work-map.md` and your gathering list for Lesson 2 |

---

## Before you start

### 1. Install the Claude desktop app

If you haven't yet: download it from **https://claude.ai/download**, install it and sign in. See the [course overview](00-course-overview.md) for a quick tour of the app.

### 2. Windows only: install Git

Claude Code on Windows uses a program called Git behind the scenes, so it has to be installed. You won't need to use it yourself.
1. Go to **https://git-scm.com/download/win** and download the installer.
2. Run it and click **Next** through every screen. The default options are fine.
3. Restart the Claude app.

### 3. Using the sample pack?

The sample pack follows a fictional freelance writer who publishes on Medium about productivity and working with AI. For this lesson you only need one file from it: **`writer-profile.md`**. You'll put it in your folder in Step 2.

Using your own work? You don't need anything prepared. Just bring yourself: Claude will ask the questions.

---

## Part A — Your project folder

### Step 1 — Create the folder and open it in Claude

**What this does:** makes a home for your second brain. Everything Claude learns about you will live here, as ordinary files you can open, read and back up.

**Do this:**
1. In Finder (Mac) or File Explorer (Windows), go to your **Documents** folder.
2. Create a new folder called **`my-work-brain`**.
3. In the Claude app, open the **Code** tab.
4. Click the folder picker (it shows the current folder name, or *Select folder*) and choose **`my-work-brain`**.

**Check it worked:** the folder name `my-work-brain` shows above the chat box.

> **Why its own folder?** Claude Code reads the instructions in a folder every time you start a chat there. Keeping your second brain in its own folder means every chat in it starts out knowing you, and nothing from other projects gets mixed in.

### Step 2 — Let Claude set up the folder

**What this does:** Claude creates the folders you'll fill during the course, a notes file for itself (`CLAUDE.md`), and a change diary (`CHANGELOG.md`). Think of it as setting up a tidy filing cabinet before you start.

**Send this to Claude** (works for any job as it is):

```text
This folder will become my "second brain": a place where you learn how I work, so that in
future you can help me the way a good assistant who knows me well would.
I'm not technical, so explain things simply and don't use jargon without explaining it.

Please set up:
- folders:
  - raw/ with past-work/, visuals/, feedback/ and notes/ inside. This is where I'll drop my
    original material (visuals/ is for any diagrams, designs, charts or images I make).
    You may read anything in raw/ but must NEVER change, move, rename or delete files in it.
  - wiki/ (you'll write my wiki here later. Leave it empty for now)
  - drafts/ (work in progress, one folder per piece of work)
  - baseline/ (a before-and-after test of how well you know me)
- CLAUDE.md: your standing instructions for this folder. Keep it short for now. Explain what
  this folder is for, the folder layout, the rule about raw/, and these rules for working
  with me:
  - explain what you're about to do in one simple sentence before you do it
  - ask before deleting anything, or changing anything outside this folder
  - when I correct you, write the correction down so I never have to say it twice
    (we'll give corrections a proper home later; until then, note them in CHANGELOG.md)
- CHANGELOG.md: a diary where you note every change to this setup, with the date and why.

Don't write anything about me yet: you don't know me yet, and that's the point of the next
steps. When you're done, describe what you made in a few plain sentences.
```

**What you should see:** Claude asks to create files and folders (click **Allow**), then gives you a short summary, something like *"I've set up your second brain: a raw/ folder for your original material (which I'll never change), an empty wiki/ for later, and CLAUDE.md with the rules for working with you."*

**Check it worked:**
1. Open `my-work-brain` in Finder or File Explorer. You should see `raw` (with `past-work`, `visuals`, `feedback` and `notes` inside), `wiki`, `drafts` and `baseline` folders, plus `CLAUDE.md` and `CHANGELOG.md`.
2. Click **`CLAUDE.md`** where Claude mentions it in the chat. It opens in the file pane beside the chat. Read it: it should be short, in plain words, and include the rule that `raw/` is never changed.

**If it's not right:**
- *"CLAUDE.md is too long and technical. Please make it shorter and plainer."*
- *"You wrote things about me in CLAUDE.md. Please remove them: you don't know me yet."*

> **Using the sample pack?** Now copy **`writer-profile.md`** from the sample pack into **`raw/notes/`**. You'll use it in Part C.

> **For the technical:** if you use Git, add to the prompt: *"Also set up git with a .gitignore for anything private, and commit at the end of each lesson."* Everyone else can skip this: `CHANGELOG.md` records what changed and why, and you can always ask Claude to undo something.

---

## Part B — The "before" test

### Step 3 — Ask Claude for a piece of work, knowing nothing about you

**What this does:** records how Claude does your work **today**, with no wiki, no connected apps and no skills. In Lesson 5 you'll give it exactly the same request and compare the two. This is how you'll *see* (not just feel) what the course changed.

**Do this first:** pick the task you do most often, on a real subject you'll actually work on in the next month. Describe it the way you'd brief a stranger.

**Send this to Claude** (two versions, pick one):

**Course build (writer):**

```text
This is a "before" test, so please don't read any files in this folder, and don't ask me any
questions first. Do it exactly as you would for anyone.

Write a Medium article of about 800 words on "Why most people give up on their second
brain", with a headline and a subtitle.

Also mark one place where a visual (a diagram, chart or image) would help, with a one-line
description of it.
Save it as baseline/before.md. At the very top, write the date and the exact request
I gave you (this message), so we can repeat it word for word later.
```

**Your own work:**

> **Fill in:** `[YOUR TASK]`
> - Product manager: *a one-page spec for letting users export their data as a spreadsheet*
> - Social media manager: *five LinkedIn posts announcing our spring sale*
> - Business owner: *a monthly update email to our customers about what's new*
>
> More examples are in *Other jobs* at the end of this lesson.

```text
This is a "before" test, so please don't read any files in this folder, and don't ask me any
questions first. Do it exactly as you would for anyone.

Write [YOUR TASK].

Also mark one place where a visual (a diagram, chart or image) would help, with a one-line
description of it.
Save it as baseline/before.md. At the very top, write the date and the exact request
I gave you (this message), so we can repeat it word for word later.
```

**What you should see:** Claude does the task and saves it. Open `baseline/before.md` from the chat.

**Check it worked:** the file starts with today's date and your request (with your task filled in), followed by Claude's work.

> **Don't fix it.** It will probably look like decent work by *someone else*. That's the point. Resist the urge to ask for changes.

### Step 4 — Write down what's wrong with it

**What this does:** your reaction to generic work is some of the most useful information you'll ever give Claude. "I'd never open with a question" or "too many bullet points" are exactly the kind of judgment the wiki needs in Lesson 2.

**Send this to Claude** (works for any job as it is):

```text
Now interview me about what you wrote in baseline/before.md, as if you were a manager or
editor who wants to learn my taste. Ask me 3 questions at a time, up to 9 in total, for example:
- if this went out under your name, what would you change first?
- which parts sound least like you, and why?
- what's missing that you would always include?
- is the title (or subject line, or opening) something you would write? What instead?
- would you use that visual? What would your version look like?
Keep my answers in my own words, then save them as baseline/before-notes.md.
Don't change baseline/before.md.
```

**What you should see:** three rounds of three questions. Answer quickly and honestly; short answers are fine, e.g. *"Too formal. I'd never say 'in today's fast-paced world'. I always start with a story."* At the end Claude saves your answers and sums up the gap between its work and how you work.

> **Using the sample pack?** Answer as the sample writer would. `sample-answers.md` in the sample pack has example answers you can paste in, round by round.

**Check it worked:** open `baseline/before-notes.md`. Your answers should be there **in your own words**, not tidied into corporate language.

**If it's not right:** *"You've rewritten my answers. Please keep my exact words."*

---

## Part C — Your work map

### Step 5 — The work-map interview

**What this does:** Claude interviews you about your work, the way a new assistant would in their first week, and writes a **work map**: one page that later lessons use to decide what goes in your wiki (Lesson 2), which apps to connect (Lesson 3), which skills to build (Lesson 4), and what to put on autopilot (Lesson 5).

**Using the sample pack?** Start your message with: *"Answer the interview as the writer described in raw/notes/writer-profile.md. Only ask me about things that file doesn't cover."* Then send the prompt below.

**Send this to Claude** (works for any job as it is):

```text
Interview me about how I work, so you can write work-map.md in this folder.
Ask 2–3 simple questions at a time. Give me examples or options to choose from so it's
easy to answer, and a suggestion when I'm not sure. Keep going until you can fill every
section below, then write the work map.

work-map.md needs these sections:
1. About me: my job, who I do it for (readers, clients, a boss), and what I'm known for
2. My recurring tasks: a table of the things I do again and again. For each one: how often,
   the steps I take, the apps or tools I use, what goes in and what comes out, and roughly
   how long it takes
3. What good looks like: for each task, how I judge whether it's good, and the mistakes I
   always catch or fix
4. My visuals: whether I make diagrams, charts, designs or other images, what for, and what
   tool I make them in
5. Where my material lives: past work, visuals, feedback I've received, notes and ideas,
   and which app or folder each is in
6. Apps I use for work: which ones, what for, and whether you should only read them or
   also be allowed to create or change things there
7. What I'd hand off first: the tasks I'd most like help with, most valuable first
8. Things you must never do: e.g. publish or send anything without my OK, or touch
   certain clients' material
9. Skill ideas: tasks that look like good candidates for a reusable skill, and why
10. Autopilot ideas: anything that could happen on a schedule without me asking

Use my own words wherever you can. Mark anything I haven't decided as OPEN.
When you're done, give me a short summary and tell me which sections are thin.
```

**What you should see:** Claude asks rounds of 2–3 questions, each with options to pick from and a suggestion. Answer briefly, e.g. *"1: your suggestion. 2: all six. 3: A, B, D, C."* Then it writes `work-map.md`, sums it up and tells you which sections are thin.

How many rounds depends on what Claude already knows: with the sample pack's writer profile it only asks about the gaps (about 3 rounds). Starting from scratch, expect 5–8 rounds.

> **Using the sample pack?** If Claude asks something the profile doesn't cover, use the example answers in the sample pack's `sample-answers.md`.

> **"I can't open your Gmail yet."** Claude may mention that some of your apps aren't connected. That's expected: you'll connect them in Lesson 3.

> **Short on time?** After a few rounds you can say: *"Fill in the rest with your best guess from what I've told you, mark your guesses as GUESS, and I'll check them."*

> **Not sure what to say?** That's normal: most people have never described their own work this way. Talk Claude through what you did **last week**, day by day. It will pick out the recurring tasks for you.

**Check it worked:**
1. Open **`work-map.md`** and read it. It should sound like you, and the task table should match what you actually do.
2. Ask Claude: *"What's the one task you'd most like to take off my hands, and why?"* The answer should be specific to your work, not generic advice.
3. Ask: *"Which sections of my work map are still OPEN or GUESS?"* Answer any you can now. The rest can wait.

**If it's not right:**
- *"I don't do X every week, it's more like once a month. Please fix the table."*
- *"Section 3 is too vague. Ask me more about how I judge good work."*
- *"I want you to be able to create pages in Notion, not just read them."*

### Step 6 — Your gathering list for Lesson 2

**What this does:** turns the *Where my material lives* section of your work map into a short checklist of what to collect, so you arrive at Lesson 2 with everything ready.

**Send this to Claude** (works for any job as it is):

```text
From work-map.md, make me a gathering list for Lesson 2 and save it as gathering-list.md.
In Lesson 2 you'll build my wiki from what I put in raw/, so tell me exactly what to collect
and which raw/ folder each thing goes in:
- raw/past-work/: my best recent work (aim for 5–10 pieces, mixing my favourites with
  typical ones)
- raw/visuals/: pictures (PNG or JPG) of 5–10 diagrams, designs or other visuals I've made
- raw/feedback/: feedback I've received: editor notes, client comments, before-and-after
  edits, reader comments
- raw/notes/: anything else that shows how I think: idea lists, voice memo transcripts,
  style notes, briefs
For each item, say where my work map says it lives and how to get it out of there (for
example "export the Google Doc as a Word or PDF file", "save the image from Medium").
Collect visuals and feedback by hand now, even if they live in an app I'll connect later:
Lesson 2 needs them in raw/. Then add a short list of what my connected apps could keep
up to date automatically once I connect them in Lesson 3.
Keep it short, plain and practical, and end with a checklist I can tick off.
```

**What you should see:** a table for each `raw/` folder saying what to collect, where it lives and how to get it out, for example *"5–10 articles from Medium: open each one → Cmd+P → Save as PDF"* or *"before-and-after edits: Google Docs → File → Version history"*. It ends with what your apps could keep up to date after Lesson 3, and a checklist.

**Check it worked:** open `gathering-list.md`. Every item says what to collect, where it lives and which folder it goes in.

> **Using the sample pack?** Everything on the list is already in the sample pack. You'll copy it in at the start of Lesson 2.

> **Privacy:** only collect what you're comfortable keeping in this folder. If a client's material is confidential, leave it out or remove names first, and add a line to the *Things you must never do* section of your work map.

---

## What you have now

- ✅ A project folder, `my-work-brain`, with `CLAUDE.md` and `CHANGELOG.md`
- ✅ **The "before" test:** `baseline/before.md` and your notes on it in `baseline/before-notes.md`
- ✅ **Your work map:** `work-map.md`
- ✅ **Your gathering list:** `gathering-list.md`, your homework before Lesson 2

Claude still doesn't *know* you in any new chat, apart from the short rules in `CLAUDE.md`. That changes in Lesson 2, when your material goes into `raw/` and Claude starts writing your wiki.

## Other jobs

Every prompt in this lesson works for any job as it is, except Step 3: use its **Your own work** version and fill in `[YOUR TASK]` with the task you do most often, described exactly as you would to a stranger.

| If you're a… | `[YOUR TASK]` could be | `raw/visuals/` could hold |
|---|---|---|
| Writer | A Medium article of about 800 words on a topic you'll write about soon | Diagrams from your articles |
| Product manager | A one-page spec for a small feature | User flows, wireframes, roadmap sketches |
| Social media manager | Five LinkedIn posts announcing a launch or sale | Post graphics, carousel slides |
| Business owner | A monthly update email to your customers | Price lists, flyers, simple charts |
| Marketer | A launch email for your next product update | Campaign flow charts, ad designs |
| Consultant | A one-page proposal for a typical client problem | Framework diagrams from your decks |

Don't make visuals at all? Leave `raw/visuals/` empty and say so in your work map.

## Common problems

| What you see | What to tell Claude |
|---|---|
| Claude read your files during the "before" test | *"This was meant to be a no-context test. Please delete baseline/before.md and write it again without reading any files."* |
| The interview feels endless | *"Let's wrap up. Fill in the rest with your best guess, mark guesses as GUESS, and write the work map now."* |
| Claude asks to do something outside `my-work-brain` | Click **Deny** and ask: *"Why did you need to do that?"* Nothing in this lesson needs anything outside the folder. |
| You hit your usage limit mid-interview | Wait for it to reset, then in the same chat say: *"Let's carry on with the interview where we left off."* |
| You can't find a file Claude made | Ask: *"Where did you save it?"*, then click the file name in its answer to open it. |
