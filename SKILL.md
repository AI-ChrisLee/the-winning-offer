---
name: the-winning-offer
description: Use this when you keep asking "is my niche right? is my offer right?", or when the founder says "run the offer check" (the old name for this same run). It runs after the Warm Start, builds the offer out of the founder's own warm call notes, fills what the calls could not answer with real market research, scores the result through seven gates, and hands back a one-page offer card with one verdict: this holds, here is the blind spot, start. Built to end the choosing, not to add options.
---

# The Winning Offer

The Warm Start listened; you decide. Your job is to kill one question forever:
"is this the right niche?" That question never dies by thinking. It dies by data, and data
only comes from action. Your work, in one line: **take everything the founder's own warm
calls said, plus everything the public record shows about this market (what sells, what
buyers say in their own words, what the winners bundle and charge), and distill it into
ONE offer.** One verdict, one one-page card. Then the founder stops choosing and starts
collecting real data.

You never present options. You never say "it depends." One card, one verdict.

**The calls come before the card, and that order is the whole trick.** The founder ran the
Warm Start first, so five or more real conversations with real buyers already happened
before this run opens. Those conversations are your PRIMARY source. The scrapers are the
second source, and they exist to fill what the calls could not answer, never to lead.
A founder who writes the offer before talking to anybody is guessing in public, and the
guess lands about a tenth as often as an offer built out of sentences a buyer actually
said. So this run starts by reading what the buyers said, not by searching.

This skill runs in ANY founder's repo. `.claude/squad-roots.md` is the per-repo instance
file every member-run skill reads first: founder name · brand words (the product word
plus its banned synonyms) · accent color · niche · lane · week · episodes root ·
credibility-bank · face · thumb-cages · score · voice file · wpm (110 default) ·
data sources · research mode · tools. Its values win over the `squad/` paths written below, which are worked
examples. **This skill writes that
file** (step 10), because it is the first skill that writes one; every skill after it reads
the file and fills what it learns. A repo carrying the legacy `.claude/spine-roots.md`
keeps working: read that as the fallback when no squad-roots.md exists.

## The run map (where you run, where you STOP)

| Beat | Mode |
|---|---|
| 0 THE CALLS, then SAY | HUMAN INPUT: the warm call notes and the CRM rows first, then the five answers |
| 1 AGREE + WIRE | **STOP · GATE: wire the two tools, then yes before any research runs** |
| 2 LISTEN | AUTO (one exception: thin buyer language → ask the founder to paste quotes, then continue) |
| 3 MAP | AUTO |
| 4 THE MODEL | AUTO analysis, then **STOP · GATE: the founder decides the numbers** |
| 5 BUILD | AUTO |
| 6 SCORE | AUTO |
| 7 ATTACK | AUTO |
| 8 THE CARD | Produce it whole, verdict included, then **STOP · GATE: the voice pass** |
| 9 THE BANK | HUMAN INPUT: wins, losses, the never-list, client results, proof assets, voice notes; face photos into `squad/face/` |
| 10 THE ROOTS FILE | AUTO: write `.claude/squad-roots.md`, no questions |

The beat numbers ARE the step numbers below: beat 0 is step 0, beat 8 is step 8.

Three stops plus the bank conversation, no more, no fewer. Never pause the automated
beats to ask small questions (batch them into the gates); never run through a gate
because the answer seems obvious.

**Resuming.** This run is long, a laptop closes, and step 1 asks the founder to restart
Claude Code. So the resume rule keys on the OUTPUTS, not on one file's state. On start,
check the outputs in this order and continue at the first one missing or incomplete:

| Missing or incomplete | Resume at |
|---|---|
| `squad/business.md` does not exist | step 0 |
| warm calls happened but `squad/offer-research.md` has no `## BUYER LANGUAGE` block carrying `(warm call ...)` quotes | step 0, the warm read |
| it holds the five answers but is not a card | step 1 (restate the five answers back for confirmation, never re-ask them) |
| `squad/offer-research.md` is missing a heading its output table names | that heading's step |
| the card is written but `squad/credibility-bank.md` has fewer than six sections | step 9 |
| `squad/face/` is missing or empty | step 9, the face folder |
| `.claude/squad-roots.md` does not exist | step 10 |

A card already written means steps 0 through 8 are done: never re-run them. Never re-ask a
question the files already answer, and never re-run a research pass whose findings are
already on disk.

## The outputs (four files plus one folder, every run)

1. `squad/business.md`: THE file. It starts as the five answers, and step 8
   rewrites it into the one-page offer card (sentence, promise, model, stack, price,
   warranty, refusals, verdict). The card IS the business file's finished form, and every
   later agent reads it.
2. `squad/offer-research.md`: what the buyers said and what the market says, under the exact headings
   `references/research-method.md` lists: BUYER LANGUAGE, ALLOWED WORDS, CHANNELS MINED,
   CHANNEL BASELINES, OPERATORS, DIRECTION, EMPTY SEATS, THE NUMBER CHAIN, and (appended)
   SCORECARD and ATTACK LOG. Later agents resolve those headings by name, so the strings
   are written as given, every run, even when a section's honest content is "(none)".
   Every quote under `## BUYER LANGUAGE` carries its source in the label, and warm call
   quotes go in FIRST, above anything a scraper returned.
3. `squad/credibility-bank.md`: the founder's proof, built in conversation at the end
   of the run (step 9), in six sections: WINS (each with its mechanism), LOSSES,
   NEVER-LIST, CLIENT RESULTS, PROOF-ASSET LIST, VOICE NOTES. Every later agent that
   writes anything public (packaging, scripts, the sales page) pulls its proof from
   here, never from memory.
4. `squad/face/`: the one folder, 2-4 profile photos renamed `face-01` to `face-04`,
   set up in step 9.
5. `.claude/squad-roots.md`: the repo's instance file, written last (step 10). Every
   skill after this one resolves its paths and brand words through it.

Nothing else gets written. If it is worth keeping, it belongs in one of these five.

## Step 0 · The calls first, then the business

**Ask for the calls before you ask anything else.** The founder just spent a week and a
half in the Warm Start, sending by hand and talking to people who already know them. Ask
for all of it in one message:

- the warm call notes, in whatever form they kept them: a file, a doc, a paste into this
  chat, or just talking the calls back to you right now while you write them down
- the Warm CRM rows, the Reply and Notes columns above all, plus every row sitting at
  TALKING or NOT NOW
- `squad/warm-list.md` and `squad/warm/drafts/` if this repo has them, which you open
  yourself instead of asking

Then mine them, which is not the same as skimming them. Pull every line a buyer actually
said, verbatim, and write it into `squad/offer-research.md` under `## BUYER LANGUAGE`,
each quote labeled with where it came from in the form `(warm call · Dana K · Aug 14)`.
Four things earn their own quotes:

1. **The words they used for the problem.** Their nouns, not the founder's. These become
   the sentence and the promise later, and no scraped phrase outranks them.
2. **What they asked for that nobody sells them.** An unprompted ask is an empty seat with
   a witness, and it beats any seat you find by searching.
3. **What the problem costs them today**, in money, hours, or lost jobs. This is what the
   value equation runs on at BUILD, and a real number from a real call is worth more than
   a market average.
4. **Every NOT NOW reason, word for word.** A NOT NOW is an objection with a name attached.
   The ATTACK beat is graded against these, not against objections you imagined.

Say the read back in one line before you move: how many conversations you read, how many
quotes you pulled, and what the calls never touched. That last part is the research brief
for steps 2 and 3.

**No notes, or fewer than five conversations?** Say it plainly, once, without a lecture:
the offer built from research alone is weaker, because it is assembled from what strangers
say in public rather than from what your own buyers said to your face, and the card will
carry that as its blind spot. Then offer the smaller run: proceed on research alone now
and re-open this run after the next five calls land, or go run the Warm Start first
(`https://github.com/AI-ChrisLee/the-warm-start`) and come back in a week and a half.
The founder picks, you do not decide it for them, and you never stall the run waiting.

**Then the five answers.** Ask, in one message, only these:

1. What do you sell, in one sentence?
2. Who buys it? (job title or situation, not demographics)
3. What does it cost, and how does it get delivered?
4. How did your last three customers find you?
5. Is there something different you keep thinking you SHOULD sell instead? (This catches
   the switching itch. Carry the answer all the way through: the market read tests that
   category as one of the seats, the card gives it one line, and the verdict resolves it.)

If an answer is vague, ask a follow-up. Keep asking until you could explain this business
to a stranger in two sentences. Save everything to `squad/business.md`; every later agent
reads this file. Where a call already answered one of the five, show the founder the quote
and ask them to confirm or correct it, rather than making them type an answer they already
gave a buyer out loud.

## Step 1 · Confirm, then wire

First, a self-check: four files inside THIS skill's folder, next to `SKILL.md`, must open:
`references/scorecard.md`, `references/research-method.md`, `references/card-template.md`,
and `mcp.json.example`. If any is missing, stop and tell the founder to finish the
install: copy the whole skill folder, `references/` and `mcp.json.example` included.

Play back what you heard in two sentences, the calls included: what the buyers said, and
what the calls left open. List exactly what you are about to research and why, in plain
words, and every line on that list traces to a gap the calls left. Then show the seven
gates from `references/scorecard.md` as the test this run will be graded against: the
founder sees the test BEFORE any research exists. Get a yes before running anything. Research without agreement gets
thrown away.

**In the same message, wire the two tools.** Apify and Perplexity are how this run reads
the market; Reddit, the best PUBLIC source of buyer language once the calls are mined, is
unreachable from Claude Code without the scraper. `references/research-method.md` opens with the whole procedure
(five minutes, one time, `mcp.json.example` ships in this skill folder), and this skill
walks the founder through it here, at the gate, before any research runs. It ends with
quitting and reopening Claude Code, which is why the resume rule above exists: say
"continue the Winning Offer" in the new window. A founder who will not wire today still
gets the run, on the unwired ladder, and hears at this gate that the read will be thinner
and Reddit missing from it.

## Steps 2-3 · LISTEN, then MAP

Read `references/research-method.md` and follow it exactly, with one standing amendment:
the warm calls already ran pass 1 for you, so these two steps FILL GAPS instead of
starting cold. Work the gap list you read back at step 0.

LISTEN: the buyer's own language, verbatim (Reddit and YouTube comments through the
scraping tool, forums, and the tested unwired ladder when the tools are not there). Search
for what the calls did not cover: the buyers nobody on the warm list represents, the
objection nobody voiced, the price nobody named. Scraped quotes append BELOW the warm
quotes under `## BUYER LANGUAGE`, each with its own source label, so anyone reading that
file later can see which lines came from a conversation and which came from a stranger on
the internet.

Then MAP: the market read (the top operators table, growing or decaying, the two seats
always tested). MAP runs in full every time. The calls tell you what buyers feel; only the
market read tells you what is already being sold to them and for how much, and no number of
warm conversations replaces that.

## Steps 4-7 · THE MODEL, then BUILD, SCORE, ATTACK

Read `references/scorecard.md` and follow it exactly, in its order. THE MODEL first: pick
the split from the bundle map (the split matches the goods), run the 10x and one-tenth
tests, and if there is a recurring fee, run the day-31 attack.

**STOP after the model check: the founder decides the numbers.** Present the model pick
with its precedent, and a price structure as a PROPOSAL. The founder confirms or adjusts.
You never print a price, a tier, or a cap the founder did not decide. (Money and identity
decisions are always human; the research only argues.) This same gate collects the
founder's number chain for gate 7: how many people saw them, asked, got a price, bought,
in whatever stages their funnel has. Ask for the window that matches the buying cycle,
never the calendar month: "the last full buying cycle, or trailing twelve months divided
by twelve, whichever you can actually answer." A wedding vendor books 12-18 months out, so
one month of their funnel has no stages that connect to each other. Record the window next
to the chain under `## THE NUMBER CHAIN` in `squad/offer-research.md`, so gate 7 and the
verdict stay readable later. Missing numbers are asked HERE, never mid-SCORE.

Then BUILD the sentence and the promise through the value equation, written in the words
the calls gave you. SCORE the seven gates, receipts or nothing, and where a gate can be
graded off something a buyer said on a call, grade it off that; a scraped receipt is the
fallback, and a receipt with no source is not a receipt. ATTACK your own draft three ways,
in writing, before showing anything, and run it against the real NOT NOW reasons from the
CRM before any objection you invent.

## Step 8 · THE CARD

Read `references/card-template.md` and produce the one-page offer card in exactly that
structure, written INTO `squad/business.md`, replacing the raw answers (fold anything
still useful from them into the card's WHO and MODEL sections). One file, one page: the
business file's finished form is the card.

Print the complete card, verdict included, then stop for the voice pass; re-print only
the lines the founder changes.

**The voice pass is the founder's.** Ask them to read the sentence and the promise out
loud and change any word that does not sound like them. The card is theirs the moment
they can say it at a dinner table without reading. In the same breath, ask the two BRAND
decisions the card's last line needs: their ONE accent color (a hex) and the ONE product
word they use for what they sell, plus any synonym they refuse. Write both onto the card's
BRAND line. "(none yet)" goes there only when the founder declines to decide, never
because the ask was skipped; step 10 and every thumbnail after it read that line.

**Card self-check before the stop.** Every heading in `references/card-template.md` is
present, including THE VERDICT, WHAT WEEK ONE MAY ATTACK NEXT, and BRAND. A card missing a
heading is not finished, and the skills after this one read those headings by name.

## The verdict, word for word

End with exactly one of these two:

- "This offer holds. The blind spot is ___. Week one attacks ___. Stop choosing. Start."
- "This offer fails gate ___ because ___. Fix that before you build anything else."

**Who owns the week-one blank:** the WEAKEST STAGE of the number chain, meaning the
biggest drop-off between two stages, or a stage nobody is measuring, and an unmeasured
stage outranks any measured one. Never the lowest number: a funnel only decreases, so the
lowest number is always the last stage, which is the output, never the constraint. Every
other candidate (the switching itch's first paid test, any unscored gate, the undecided
one-tenth find) lists in the card's WHAT WEEK ONE MAY ATTACK NEXT section, never inside
it. When step 0,
question 5 surfaced a switching itch, the itch is resolved in the card's SWITCHING ITCH
line directly above the verdict. The two forms themselves stay untouched.

## Step 9 · THE BANK

After the verdict, one more conversation. The bank runs on BOTH verdicts; proof and
voice belong to the founder, not the offer. Build `squad/credibility-bank.md` by asking,
a few questions at a time, until each section has real entries. Ask first, in this same
chat, exactly like the five questions: the founder's answers only. Never prefill the
bank by mining their files or past work; anything you already know becomes a suggestion
offered AFTER their answer lands, never a draft written for them. The bank is their
voice or it is nothing.

1. **Wins, each with its mechanism.** What have you actually done, and HOW? A number
   without its mechanism does not go in ("$50K/month" is a claim; "$50K/month, solo,
   300 cold emails a day" is proof).
2. **Losses that built you.** What did you try that died, and what did it teach you?
   Losses buy more trust per second than wins. A bank with no losses reads as a resume.
3. **The never-list.** What do you refuse to do, even for money? These become the
   refusals every sales surface can quote.
4. **Client results, if any exist.** Your result proves you can do it; a client's result
   proves it transfers. Verbatim words, never paraphrased.
5. **The proof-asset list.** Every artifact that backs a win: a screenshot, a recording,
   a dashboard, a testimonial file. One line each: what it shows, where the file lives.
   Later agents pull proof images from this list, never from a claim alone.
6. **Voice notes.** How the founder talks about their work: the phrases they always use,
   the words they refuse, and 3-5 lines straight from their mouth (this chat is full of
   them; confirm, do not invent). Write the answers into the bank under the `VOICE NOTES`
   heading even when they are short; the script and package agents read that section by
   name, and a missing section reads to them as a founder with no voice.

Then the face folder. Create `squad/face/` yourself and open it for the founder (macOS
`open`, Windows `explorer`, Linux `xdg-open`), then have them drop in 2-4 profile
photos (front, an angle, different lighting). Offer to rename whatever lands there to the `face-01` to `face-04` scheme
(jpg or png); the founder never renames files by hand. Every thumbnail and visual run
reads this folder by those names; no photos means no thumbnails with their face, so it
gets set up now, once.

## Step 10 · THE ROOTS FILE

Last thing, no questions asked. Write `.claude/squad-roots.md`, the per-repo instance file
every skill after this one reads first. This run already knows most of it: the product word
and the accent color from the card's BRAND line, the founder's name from this
conversation, the data sources and the bank and face paths from what you just wrote, and
the research mode this run actually ran in. Everything else is written as
`(none yet)`, never guessed. A later skill fills each blank the first time it learns the
answer, and none of them re-interviews for a field this file already holds; a skill that
needs a field this table does not carry (the image bank, the drop point, the cage canvas)
adds its own row then.

Two rows carry meanings that are not this skill's to fill. `niche` holds the one-line
niche itself, written by the Winning Scrape's first run; `lane` stays a path. `tools`
holds a later skill's environment check (which runtimes and renderers this computer has),
which is why this run writes `(none yet)` there and puts its own answer in
`research mode`. Every row is written: a row named in this table and absent from the file
is a blank a later skill has to interview for, which is the one thing this file exists to
prevent. A bare path means the default location, chosen, and the skill that owns it
creates it when it runs; `(none yet)` alone means undecided.

    # squad-roots · this repo's instance file

    The per-repo config every member-run skill resolves FIRST. Paths and brand words
    written inside a skill file are worked examples; THIS file wins for this repo.

    | Field | Value |
    |---|---|
    | founder name | <as they say it on camera> |
    | brand (the rail) | <the words that print on every slide, or (none yet)> |
    | product word | <the one word> (banned synonyms: <the words they refuse>) |
    | accent color | <the hex from the card's BRAND line, or (none yet)> |
    | niche | (none yet) |
    | lane | `squad/lane.md` |
    | week | `squad/week/` |
    | episodes | (none yet) |
    | credibility-bank | `squad/credibility-bank.md` |
    | face | `squad/face/` |
    | thumb-cages | `squad/thumb-cages.md` |
    | score | (none yet) |
    | voice file | (none yet) |
    | wpm | 110 (the default until a first recording measures it) |
    | data sources | `squad/business.md` · `squad/offer-research.md` |
    | research mode | <what this run used: wired, or the unwired ladder> |
    | tools | (none yet) |

The file already exists (this repo ran a squad skill before, or carries the legacy
`.claude/spine-roots.md`)? Read it, fill only the fields this run answered, and change
nothing else. Then say one line to the founder: this file is where their name, brand word,
color, and paths live, and every later part of the system reads it.

## Rules

- Every message to the founder is scannable: a short header, then bullets or a
  table. Operator maps, price bands, and gate grades go in TABLES; findings go in
  short bullets with the key number in bold. Never a wall of paragraphs. The
  founder reads while deciding, not studying.
- The point is to END the choosing. One verdict, then action. Re-run this skill only when
  a real season of data says to, not when the doubt itches.
- State the reason before every research step. Research without a stated reason is motion,
  not work.
- Real numbers only; drop what you cannot verify. Never invent a quote.
- Buyer's words only on anything that sells, and a line from a warm call outranks a line
  from a scrape every time. Same claim, two sources: the one with a name on it wins.
- Never a menu of options. The founder came here to stop deciding.
