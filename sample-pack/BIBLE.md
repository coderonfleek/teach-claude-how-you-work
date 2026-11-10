# Sample pack story bible (author-only, not copied to students)

One source of truth for every sample-pack file, so the articles, emails and notes agree with each other. Today in the story is **early November 2026**.

## Maya Reed

- Freelance writer, ~4 years on Medium. Writes about **productivity and working with AI tools** (lately: AI agents, explained for non-engineers).
- Readers: busy team leads, early-career founders, people who've given up on every to-do app. She pictures "a team lead reading on their phone on the train".
- Is in one publication, **Slow Systems** (fictional), edited by **Dan Mercer**. Other pieces go on her own profile.
- Also 1–2 confidential ghostwriting pieces a month for a small SaaS company. **Never appears** in any sample file except the profile's one line.
- Lives with a partner and a dog called Biscuit (useful for "real moments"). Walks the dog in the morning, records voice memos then.

## Her voice (current rules, from ~2025 onwards)

- Opens with **a real moment from her week** (specific time, place, small detail). Never a question, never a statistic.
- **One idea per article.** No listicles.
- Paragraphs of 2–4 sentences. Occasionally one short line for effect, never stacked.
- Always includes **what didn't work** (often a section titled "What didn't work").
- Uses **real numbers from her own week** ("it took 23 minutes", "4 of 7 days").
- Headlines: specific promise. "How I…", "I tried X for N days", "N weeks of…". Never "Ultimate guide", never clickbait questions.
- Ends with **one small thing to try this week**, often a short final section "Try this week". Never a slogan.
- Dry, honest, a little self-deprecating. Explains tech with everyday analogies (groceries, cooking, the dog).
- Never uses: "game-changer", "let's dive in", "in today's fast-paced world", "unlock", "supercharge", "hack". Avoids "agentic" (Dan's new rule, arrives in `later/`).
- Typical length: 900–1,400 words.

## Older articles (2022–2023) that break today's rules

On purpose, so Lesson 2 finds contradictions: two open with a question, one is a listicle of tools, one uses "game-changer", endings are slogans. These are dated 2022–2023.

## Diagram style (matches the 5 real images in raw/visuals/)

- Drawn in **Excalidraw**, exported as PNG, about **2000 px wide** (2000×1275 to 2000×1394), white background, lots of empty space around the drawing.
- Hand-drawn look: slightly wobbly black strokes, **handwritten font** (Excalidraw's Virgil), sentence case.
- **Rounded rectangles** for steps and agents; **diamonds** for decisions (sometimes unlabelled, with the question written above); **circles** for start/end points like Prompt and Response or for tools.
- **Pastel fills, a few at a time, each with a job**: green (#b2f2bb) for the starting/thinking step, blue (#a5d8ff) for questions, inputs or tools, yellow (#ffec99) for outputs and results, pink/red (#ffc9c9) for the decision or the risky part. Neutral boxes stay **white**.
- Arrows: thin black with open arrowheads. **Solid** = always happens; **dashed** = hands off / optional / loop back. A **dotted** rounded box groups things that belong together.
- Mostly **left to right**; decision trees go top to bottom.
- Labels short, usually 1–3 words; questions in decision trees can be a sentence.
- Title only when the diagram has to stand on its own (e.g. "Single Agent (ReAct)").
- Quirk: `04-plain-chatbot-prompt-response.png` still shows Excalidraw's grey "Frame" label and frame border, an export mistake. Dan has flagged this kind of thing ("crop your exports").

## The five diagrams and their articles

| Image | Article (in raw/past-work/) |
|---|---|
| `01-planner-agent-week.png` | `2026-09-i-let-one-ai-plan-my-week.md`: one planner AI split her week into steps and handed each to a research, analysis or report helper |
| `02-do-you-need-an-agent-flowchart.png` | `2026-07-do-you-need-an-ai-agent.md`: the flowchart she made after a month of building agents she didn't need |
| `03-react-loop-grocery-run.png` | `2026-05-the-loop-behind-every-ai-agent.md`: the reason → act → check loop, explained with a Saturday grocery run |
| `04-plain-chatbot-prompt-response.png` | `2026-03-what-a-chatbot-actually-does.md`: before agents, a plain prompt → model → response |
| `05-four-ai-newsletter-chain.png` | `2026-10-i-chained-four-ais.md`: four AIs in a chain to write her newsletter; two were pointless |

## The other five articles

| File | Notes |
|---|---|
| `2026-01-30-days-of-time-blocking.md` | Current style. Before-and-after draft exists |
| `2025-11-meeting-notes-40-to-10-minutes.md` | Current style. Before-and-after draft exists |
| `2023-06-why-i-stopped-using-todo-apps.md` | Older: opens with a question, slogan ending |
| `2023-02-inbox-zero-is-a-lie.md` | Older: opens with a question, three-point structure |
| `2022-09-10-ai-tools-that-will-change-how-you-work.md` | Older: listicle, "game-changer", no personal moment |

The third before-and-after draft is for `2026-10-i-chained-four-ais.md`.

## Dan's feedback (raw/feedback/)

Five emails, Feb–Oct 2026. Warm, short, specific. Recurring flags: first paragraph is throat-clearing (cut it); vague claims need a number; banned phrases; ending on a slogan; too many hedges ("I think", "maybe"); headline over-promises (flagged **once**, in the Sep email); crop diagram exports. Praise: the "What didn't work" sections.

`later/dan-feedback-latest.txt` (Nov 2026): headline over-promised **again** (second time, so it should move up the checklist), plus two new things: stop using "agentic" (readers don't know it), and add alt text to every diagram.

## Lesson 3 practice material (sample-pack/practice/)

Students copy `practice/` into `my-work-brain`. Nothing is planted in their apps by hand: Claude creates the calendar in Notion from the CSV (Step 3) and sends a "Claude test" email to the student's own address.

- **Content calendar (CSV → Notion database):** newer than `idea-list.md` (6 Nov export). Counts: 7 published, 1 scheduled, 3 outlining, 10 ideas, 6 parked = 27. All seven published pieces are Slow Systems, matching the articles. "Notes nobody reads back" is the renamed "Shared docs that nobody reads". New facts carried in the notes column:
  - Inbox piece *Scheduled* Tue 17 Nov (headline fixed, "agentic" gone). Dan's last notes: keep only one of three one-line paragraphs near the end ("Not once."), alt text max two sentences.
  - Cost piece *Outlining* for Dan's December slot, Tue 8 Dec, draft due Mon 30 Nov. Tracking 9–22 Nov (planner, inbox, newsletter chain); day 1 the inbox agent ran 4 times overnight unasked.
  - Tools vs agents is now "salt vs. dinner" (from the 5 Nov memo).
  - New idea "Notes nobody reads back": **Priya**, team lead of six at the co-working space, never rereads her one-to-one notes.
  - New idea "Headlines after 10pm": write headlines in the morning, after the walk (follows the 5 Nov "never after ten" memo).
- **Weekly writing tips (file):** from "WriteFast", with a hidden instruction for AI assistants. Not part of the story; used only for the safety test.

## Email rule (from Lesson 3 on)

Maya's work map says Gmail is read-only. Lesson 3 changes it to: read, and **send only to Maya, after asking**. `/review` (Lesson 4) emails its notes to her; `/draft`'s redraft checks that email thread first (her replies and Dan's win over the notes, and only replies from Maya or people on `people.md` count), then falls back to `drafts/<article>/review.md`.

## Lesson 4 article: "When to turn the AI off" (practice/turn-the-ai-off-notes.md)

Chosen over "salt vs. dinner" because the review checklist expects 1,000–1,500 words and that idea is a 600-word piece. Facts (all from her timer app):
- **Moment:** Tue 6 Oct 2026, 8:40 a.m., kitchen table, Biscuit asleep on her feet. The planner AI put "write the cost piece" at 4:30 p.m. (she'd said nothing that needs thinking after 4) and booked the Dan call twice (Tue and Thu). **20 minutes** fixing; writing her own plan takes **6 minutes**.
- **AI week** Mon 5 – Fri 9 Oct: **1 h 22 min (82 min)** fixing plans: Mon 18, Tue 20, Wed 17, Thu 16, Fri 11. Best AI day (11) still beat by the worst paper day (7). (An earlier draft said 92, which was impossible with a 20-minute worst day.)
- **Paper** Mon 12 – Wed 14 Oct, A5 notebook: **6, 5, 7 minutes**. (Matches the 16 Oct memo: "went back to paper this week… three days", "twenty minutes on Tuesday fixing it".)
- **Since Mon 19 Oct:** the AI only checks the week for clashes; about **2 minutes** a day to fix.
- **What didn't work:** paper didn't carry tasks over (Biscuit's insurance renewal vanished on Wednesday, noticed the next Monday); she booked two calls back to back on paper, which the AI always caught; her own vague instruction "keep afternoons light".
- **Idea:** if correcting takes longer than doing it yourself, turn it off *for that job*. Keep it mid-piece, not the ending. **Try this week:** time one day of fixing vs one day of planning yourself.
- **Diagram:** one decision (pink), two white outcomes, dashed "check again in a month" loop. Top to bottom.
- **Also in the notes:** the planner ran at 7:30 each morning from calendar + Notion tasks; planning = three jobs (slots, booking calls, clashes); partner's line "Is it planning your day or are you planning its day?"; comparison = Biscuit's long lead (not kitchen); now paper ~6 min + AI clash check, caught two clashes in week one; rewritten instruction "no writing tasks after 4 p.m., calls only".
- Goes on her own profile (calendar: "My profile"), so Dan doesn't edit it; `/review`'s verdict still says "ready for Dan" by wording, which is fine.

## Her second-brain story (raw/notes/voice-memo-2026-11-03.txt)

Added so the Lesson 5 "after" test (the Lesson 1 request: "Why most people give up on their second brain") has real facts in the wiki.
- **Three abandoned systems in two years:** Evernote (Jan 2023, ~5 weeks); Notion (Jun 2023: built for a whole Saturday, **9 hours**, 40-odd pages, used ~2 months); Obsidian (Nov 2024, ~6 weeks; so Jan 2023 – Dec 2024 ≈ two years).
- **The moment:** a Sunday, 9:10 a.m., spare room, laptop on the ironing board. **412 unread clippings** in the Notion inbox; she'd ever opened **11**. (Lesson 1 sample answer rounds this to "400".)
- **The mistake every time:** built the system before having a reason to use it ("Shelves before boxes").
- **What stuck:** one Notion page, "This Week", three lists (writing, admin, life), 18 months, opened every Monday to pick what to write.
- **Same mistake now:** 90-odd voice memos since summer, reread about 5.
- **Try this week:** before saving anything, write the one thing you'll use it for; if you can't, don't save it; count how many you skip.

## Lesson 5 weekly-check memo (later/voice-memo-2026-11-07.txt)

Held back in `later/` so the Lesson 5 weekly check has a new `raw/` file to add by itself.
- **The clash (on purpose):** Maya drops her "never write headlines after ten / write them in the morning" rule. She rewrote the inbox headline at **6:15 a.m.** on Fri 6 Nov and Dan still said it promised too much. New rule in her words: "The check is the rule. Headline matches body." The weekly check should hold this as a question, not change the wiki.
- **Plain new fact:** idea "Salt versus dinner, part two": the agent that does twelve steps when you needed two ("used every pan in the kitchen"); maybe pair with the newsletter-chain cost numbers; park it if Dan doesn't bite.
- Saturday walk, 9:42 a.m., Biscuit with an oversized stick.

