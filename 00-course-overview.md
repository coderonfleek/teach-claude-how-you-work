# Course Overview — Teaching Claude Code How You Work

## Who this course is for

**Anyone who already uses Claude and is tired of explaining themselves every time.** If you've ever thought *"Claude is clever, but it doesn't know me, so everything it writes sounds generic"*, this course fixes that.

You don't need to be technical. If you can use a computer, you can do this course. You'll **click buttons in the Claude app, copy prompts into Claude**, look at what it makes, and tell it what to change in plain words. Claude does all the technical work.

If you *are* technical, everything still applies. Look out for the **For the technical** notes, which explain what's happening underneath.

## What we're building

A Claude that works **the way you work**. It has three layers, and each one builds on the one before it:

1. **A second brain.** A wiki about you and your work: your voice, your standards, your clients or readers, how you make decisions, how your visuals look, what "good" looks like to you. You drop in your material (past work, notes, feedback you've received) and **Claude writes and maintains the wiki**. You never have to keep it tidy yourself. That's why this one won't die like the Notion setups you've abandoned before.
2. **Connections to your apps.** Claude can read (and, when you allow it, write to) the apps where your work lives: Notion, Gmail, Google Drive, and Medium through the browser.
3. **Skills built from 1 and 2.** Claude looks at your wiki and your apps, works out what you do again and again, and turns each of those into a **skill**: a saved workflow you run with a slash command. For our writer, that's `/ideate`, `/draft`, `/diagram`, `/review` and `/publish-medium`. Every time you correct a skill, it gets better.

Then we put parts of it **on autopilot**, so some of the work happens without you asking.

**Diagrams in your style.** Writers who explain ideas often draw them. You'll give Claude pictures (PNG or JPG) of diagrams from your past articles. Claude studies them, writes down your diagram style in the wiki (shapes, colours, lettering, arrows, layout, how much text), and the `/diagram` skill draws new diagrams in that same style for each article, as images ready for Medium. Not a writer? The same steps work for any visuals you make: user flows, post graphics, flyers or charts.

**Each lesson ends with something that works.** In Lesson 1 you'll give Claude a writing task with no context and save the result. In Lesson 5 you'll give it the same task again and compare. That difference is what this course is about.

## How every lesson works

There are **five lessons, one for each stage**, and each lesson is **one video**. Follow along with the video and the written lesson side by side: they cover exactly the same steps.

A lesson is split into **parts** (for example, Lesson 2 has *Setting up the wiki*, *Teaching Claude your judgment* and *The add, ask and tidy habits*). Take a break between parts if you like: each part ends at a point where everything works.

Each lesson has the same structure:

- **Lesson goal**: what you'll have at the end
- **Before you start**: anything to set up first, with step-by-step instructions
- **Parts**, each made of **steps**, and each step has:
  - **What this does**: in plain words
  - **Send this to Claude**: a prompt to copy and paste, or **Do this**: something you click or do yourself
  - **What you should see**
  - **Check it worked**: how to tell it went right
  - **If it's not right**: what to say to Claude
- **Other jobs**: what changes if you're not a writer
- **What you have now**

### Prompts work for any job

The course follows a writer, but **every prompt is written so you can reuse it for your own job**: product manager, social media manager, business owner, consultant, anyone. There are two kinds of prompt:

- **Works for any job as it is.** Most prompts. They're marked *(works for any job as it is)*: copy and send them unchanged, whatever you do.
- **Two versions.** Where a prompt needs details about *your* work, it comes twice:
  - **Course build (writer):** filled in for our writer. This is the one used in the video. Use it if you're following along with the sample pack.
  - **Your own work:** the same prompt with **[PLACEHOLDERS IN CAPITALS AND BRACKETS]** where your details go. A fill-in box above it shows what to write, with examples for other jobs:

> **Fill in:** `[YOUR TASK]` → PM: *a one-page spec for adding dark mode to our app* · Social media manager: *five LinkedIn posts announcing our spring sale* · Business owner: *a monthly update email to our customers*

Replace the whole placeholder, brackets included, then send the prompt. If you leave one in by mistake, Claude will ask you about it.

> **The golden rule:** if anything goes wrong (an error, a strange result, something you don't understand), **tell Claude what you see in your own words**. "It says the connector isn't working" or "this doesn't sound like me" is all Claude needs. You never have to work out the fix yourself.

## The big ideas (why this works)

- **Claude only knows what's written down.** It doesn't remember last week's chat the way a colleague would. The wiki is where everything it should know about you lives, so every new chat starts informed.
- **Your material stays as it is, and the wiki is Claude's job.** You drop things into a `raw/` folder and never have to organise them. Claude reads them and writes the wiki. Your originals are never changed.
- **Judgment beats facts.** "I write for busy founders" helps a little. "I always cut the first paragraph because it's throat-clearing" helps a lot. The course spends real time getting your *judgment* into the wiki, because that's what makes skills good.
- **Connect to read first, write later.** Claude starts by reading your apps. You decide, one app at a time, whether it may also create or change things.
- **Skills come from your work, not from imagination.** We don't invent skills. Claude finds them in what you already do.
- **Every correction is useful.** When you tell Claude "not like that", the course shows you how to save that correction so you never have to say it twice.

## Before Lesson 1: get comfortable with the app

### Install the Claude desktop app

1. Download the Claude app from **https://claude.ai/download** (Mac or Windows) and install it like any other app.
2. Sign in. You need a paid Claude plan (Pro, Max, Team or Enterprise).
3. Open the **Code** tab. This is Claude Code: Claude can work with files on your computer, use your connected apps and do tasks for you.
4. When it asks for a folder, choose the folder you're working in (we create it in Lesson 1).

### A quick tour of what you'll use

- **The chat box**: where you paste prompts and talk to Claude.
- **Allow / Deny**: when Claude wants to do something (create a file, use a connected app, open a web page), it **asks first**. Read the short description and click **Allow**. If you're unsure, ask: *"What does this do, in simple terms?"*
- **The file pane**: click a file Claude mentions to open it beside the chat. This is how you'll read your wiki.
- **The browser pane**: a small web browser inside the app. Claude uses it in Lessons 3 and 4 for Medium.
- **Settings → Connectors**: where you connect apps like Notion and Gmail (Lesson 3).
- **Slash commands**: type `/` in the chat box to see your skills. From Lesson 4 onwards, your own skills show up here.

> **Prefer the terminal?** Claude Code also runs in a terminal window. Every prompt in this course works the same there, but the clicks described in the lessons will be different.

### Windows only: install Git

Claude Code on Windows uses a program called Git behind the scenes, so it needs to be installed. You won't use it yourself.
1. Go to **https://git-scm.com/download/win** and download the installer.
2. Run it and click **Next** through every screen. The default options are fine.
3. Restart the Claude app.

## Words you'll hear (plain-English glossary)

| Word | What it means |
|------|---------------|
| **Second brain** | A collection of notes about you and your work that you can rely on instead of your memory. Here, Claude writes it for you |
| **LLM Wiki** | Andrej Karpathy's method for a second brain that an AI maintains: you add material, the AI writes and organises linked pages |
| **Raw material** (`raw/`) | Your original files: past work, notes, feedback, briefs. Claude reads them but never changes them |
| **Wiki** (`wiki/`) | The pages Claude writes from your raw material, linked to each other, like a small Wikipedia about you |
| **Index** | The wiki's contents page, so Claude can find the right page quickly |
| **Log** | A diary of everything that was added to or changed in the wiki, and when |
| **Add / ask / tidy** | The three wiki habits: *add* new material, *ask* the wiki a question, *tidy* it (find contradictions, out-of-date pages and gaps) |
| **Check apps** | The fourth habit, from Lesson 3: Claude looks in your connected apps for anything new since the last *add* |
| **Browser pane** | The web browser built into the Claude app. Claude uses it for sites with no connector, like Medium, while you watch |
| **Hidden instruction** | Text inside an email, document or web page that tries to tell an AI what to do. Your rules tell Claude to point it out and never follow it |
| **CLAUDE.md** | A file of standing instructions Claude reads at the start of every chat in your folder. It holds the rules for your wiki |
| **Work map** | The plan you make in Lesson 1: your tasks, your tools, and what "good" means for each |
| **Connector** | A link between Claude and one of your apps (Notion, Gmail…), set up with a few clicks |
| **MCP** | The technical standard connectors are built on. You'll see the word, but you don't need to know how it works |
| **Read / write access** | *Read*: Claude can look at things in the app. *Write*: Claude can also create or change things there |
| **Skill** | A saved workflow with your standards built in, which you run with a slash command like `/review` |
| **Slash command** | Typing `/` and a skill's name in the chat box to run it |
| **Skill test** | A small set of examples Claude uses to check a skill is actually better than a plain prompt |
| **Scheduled task** | A job Claude runs by itself at set times, like every Monday at 9am |
| **Baseline** | The "before" result from Lesson 1, used to measure how much better Claude has become |

## Lessons

| # | Lesson (one video) | Parts | What you'll have at the end |
|---|--------------------|-------|-----------------------------|
| 1 | [Map How You Work](01-map-how-you-work.md) | **A.** Your project folder · **B.** The "before" test · **C.** The work-map interview | A work map, and a baseline article from Claude with no context |
| 2 | [Your Second Brain](02-your-second-brain.md) | **A.** Setting up the wiki: `raw/` and `wiki/` folders, wiki rules in CLAUDE.md, first pages from your past work · **B.** Teaching Claude your judgment: voice, standards, review checklist, and your **visual style** from pictures of your past work (for our writer, her diagrams) · **C.** The add, ask and tidy habits | A wiki that knows *how* you write and draw, not just *what* you've done |
| 3 | [Connecting Your Apps](03-connecting-your-apps.md) | **A.** Notion, Gmail and Google Drive connectors, each tested: Claude creates your content calendar in Notion, emails you and reads it back · **B.** Safety basics: what Claude can do in each app, app rules in CLAUDE.md (Claude may email only you), and a hidden-instruction test · **C.** Feeding the wiki from your apps, and a fourth habit, *check apps* · **D.** Medium in the browser: sign in, a test draft, and bringing in your published work | Connected apps, each tested, and a wiki updated from them |
| 4 | [Skills From How You Work](04-skills-from-how-you-work.md) | **A.** How a skill works, finding your skills in your wiki, and the rules every skill follows · **B.** `/ideate`, which adds ideas to your Notion calendar · **C.** `/draft`, `/diagram` and `/review`: `/review` saves its notes and emails them to you; reply from your phone, and `/draft` redrafts from the email thread first (your replies win), falling back to the saved notes · **D.** `/publish-medium`, plus a copy-and-paste fallback · **E.** Testing a skill against your past work, and corrections that land in the right place | An article with your diagrams, saved as a Medium draft ready for you to publish |
| 5 | [On Autopilot](05-on-autopilot.md) | **A.** Rules for autopilot, then a weekly wiki check and a Monday ideas brief, emailed to you · **B.** `/wrap-up`: saving what Claude learns at the end of each chat · **C.** The "after" test, scored against your own checklist | A system that keeps improving by itself, and your before-and-after comparison |

## Your folder at the end of the course

You don't need to understand every file. Claude creates and looks after almost all of them. The folders **you** put things in are marked ✋.

```
my-work-brain/
├── CLAUDE.md          Claude's standing instructions, including the rules for your wiki
├── CHANGELOG.md       A diary of every change to your skills, and why
├── work-map.md        Your tasks, tools and standards (from Lesson 1)
├── raw/             ✋ Your original material. Claude reads it but never changes it
│   ├── past-work/   ✋ Articles you've written
│   ├── visuals/     ✋ Pictures of diagrams or designs you've made (PNG or JPG)
│   ├── feedback/    ✋ Notes from editors, clients or readers
│   └── notes/       ✋ Ideas, voice memos, anything else
├── wiki/              Your second brain, written and kept tidy by Claude
│   ├── index.md       The contents page
│   ├── log.md         What changed and when
│   └── …              Pages like voice.md, readers.md, visual-style.md, review-checklist.md
├── drafts/            Articles in progress, one folder per article (the text and its diagram images)
├── baseline/          The "before" and "after" tests
├── practice/          Practice files from the sample pack (Lessons 3 and 4)
├── reports/           Reports from your scheduled jobs (Lesson 5)
└── .claude/skills/    Your skills: /ideate, /draft, /diagram, /review, /publish-medium, /wrap-up (a hidden folder)
```

> **File names may differ slightly.** Claude decides the exact names of wiki pages based on your material. If you can't find something, ask Claude: *"Which wiki page covers my voice?"*

## Sample pack

The course comes with a **sample pack** for a fictional freelance writer who publishes on Medium about productivity and working with AI:
- a writer profile (`writer-profile.md`) and example answers (`sample-answers.md`), so you can answer Lesson 1's interviews as the writer
- 10 past articles
- pictures (PNG/JPG) of the diagrams from those articles, all in one consistent style
- a folder of editor feedback and before-and-after edits
- notes and a few voice-memo transcripts
- a `practice/` folder: a content calendar Claude puts into your Notion for you and a pretend newsletter for a safety test (Lesson 3), and the writer's notes for the article you write with your skills (Lesson 4)
- a `later/` folder with one new piece of feedback, held back for practising the *add* habit in Lesson 2

Follow along with it first. Once it works, run the same lessons with your own work. Claude checks what you give it and offers to organise it for you.

> **About your apps:** there's nothing to set up in your apps ahead of time. In Lesson 3, Claude creates the writer's content calendar in your Notion and sends a test email to you, so it has something real to work with.

## What gets set up along the way

You don't need to install anything ahead of time. Each lesson tells you what to set up when you need it.

| What | What it's for | Lesson |
|------|---------------|--------|
| Claude desktop app | Where you work with Claude | Before Lesson 1 |
| Git (Windows only) | Needed by Claude Code itself on Windows | Before Lesson 1 |
| Notion connector | Your content calendar and notes | 3 |
| Gmail connector | Feedback from editors and clients | 3 |
| Google Drive connector | Notes and documents | 3 |
| The app's browser (or Claude in Chrome) | Reading and drafting on Medium, which has no connector | 3, 4 |
| Skill creator (built in) | Building and testing your skills | 4 |
| Obsidian (optional) | A nicer way to browse your wiki as linked pages | 2 |
