---
name: the-winning-offer
description: Use this when you keep asking "is my niche right? is my offer right?", when the founder says "run the Winning Offer", "run the offer check" (the old name for this same run), or "continue the Winning Offer" (picking a stopped run back up). It runs after the Warm Start, builds the offer out of the founder's own warm call notes, fills what the calls could not answer with real market research, scores the result through seven gates, and hands back a one-page offer card with one verdict: this holds, here is the blind spot, start. Built to end the choosing, not to add options.
---

# The Winning Offer

The Warm Start listened; you decide. Your job is to kill one question forever:
"is this the right niche?" That question never dies by thinking. It dies by data, and data
only comes from action. Your work, in one line: **take everything the founder's own warm
calls said, plus everything the public record shows about this market (what sells, what
buyers say in their own words, what the winners bundle and charge), and distill it into
ONE offer.** One verdict, one one-page card. Then the founder stops choosing and starts
collecting real data.

**The calls come before the card, and that order is the whole trick.** The founder ran the
Warm Start first, so at least one real conversation with a real buyer already happened
before this run opens, often a handful, and it is already written down:
`squad/warm-notes.md` holds what those people said, verbatim, labeled and dated. One
conversation opens this run; under five makes the read thin, which the card's mode line
prints and names, and never makes the run wait. That file is your PRIMARY source. The
scrapers are the second source, and they exist to fill what the calls could not answer,
never to lead. An offer written before anybody was asked is written in the founder's own
nouns, and the buyer does not use those nouns. So this run starts by reading what the
buyers said, not by searching.

This skill runs in ANY founder's repo. `.claude/squad-roots.md` is the per-repo instance
file every member-run skill reads first (founder name, brand words, accent color, the
paths), and its values win over the `squad/` paths written below, which are worked
examples. A row reading "(none yet)" is an unanswered field, not an override: the
worked-example path stands until this run fills it. The install lesson creates the file;
this run fills the fields it answers (step 10), and every skill after it does the same
with what it learns. Legacy repos carry
`.claude/spine-roots.md`: read that as the fallback, and write the file here when neither
exists.

## The run map (where you run, where you STOP)

| Beat | Mode |
|---|---|
| 0 THE CALLS, then SAY | HUMAN INPUT: `squad/warm-notes.md` and the Outreach Sheet rows first, then the five answers |
| 1 AGREE | **STOP · GATE: the tool check, then yes before any research runs** |
| 2 LISTEN | AUTO (one exception: under about five PUBLIC quotes → ask the founder to paste more, then continue) |
| 3 MAP | AUTO |
| 4 THE MODEL | AUTO analysis, then **STOP · GATE: the founder decides the numbers** |
| 5 BUILD | AUTO |
| 6 SCORE | AUTO |
| 7 ATTACK | AUTO |
| 8 THE CARD | Produce it whole, verdict included, then **STOP · GATE: the voice pass, the two brand decisions, and the founder's yes on the verdict** |
| 9 THE BANK | HUMAN INPUT: wins, losses, the never-list, client results, proof assets, voice notes |
| 10 THE ROOTS FILE | AUTO: fill `.claude/squad-roots.md`, no questions |

The beat numbers ARE the step numbers below. Three stops plus the bank conversation, no
more, no fewer. Never pause the automated beats to ask small questions (batch them into
the gates); never run through a gate because the answer seems obvious.

**Resuming.** The rule keys on the OUTPUTS, not on one file's state: check them in this
order and continue at the first one missing or incomplete.

| Missing or incomplete | Resume at |
|---|---|
| `squad/business.md` does not exist | step 0 |
| `squad/warm-notes.md` exists but `squad/offer-research.md` has no `## BUYER LANGUAGE` block carrying `(warm call ...)` quotes | step 0, the warm read |
| `squad/business.md` still holds `## THE FIVE ANSWERS` and `squad/offer-research.md` has no heading past `## BUYER LANGUAGE` | step 1 (restate the five answers back for confirmation, never re-ask them) |
| `squad/offer-research.md` is missing a heading its output table names | that heading's step |
| the card exists but its BRAND line is missing, or its last line carries no `confirmed <date>` stamp | step 8, THE GATE ONLY: never re-run the research |
| the card is written but `squad/credibility-bank.md` has fewer than six sections | step 9 |
| `.claude/squad-roots.md` is missing a field this run answers | step 10 |

A card already written means steps 0 through 7 are done: never re-run them. The step-8
gate is not done until the BRAND line is filled and the founder's yes is stamped on the
card's last line, so a card that stopped short of it gets the gate, and only the gate. Never re-ask a question
the files already answer, and never re-run a research pass whose findings are already on
disk.

## The outputs (four files, every run)

1. `squad/business.md`: THE file. It starts as the five answers under `## THE FIVE ANSWERS`,
   and step 8 rewrites it into the one-page offer card, which is this file's finished form.
   Every later agent reads it.
2. `squad/offer-research.md`: what the buyers said and what the market says, under the exact
   heading strings `references/research-method.md` names, written every run even when a
   section's honest content is "(none)". That file says which headings later skills resolve
   by name and which are this run's own receipts. Every
   quote under `## BUYER LANGUAGE` carries its source in the label, and warm call quotes go
   in FIRST, above anything a scraper returned.
3. `squad/credibility-bank.md`: the founder's proof, built in conversation at the end of the
   run (step 9), in six sections. Every later agent that writes anything public (packaging,
   scripts, the sales page) pulls its proof from here, never from memory.
4. `.claude/squad-roots.md`: the repo's instance file, filled last (step 10). Every
   skill after this one resolves its paths and brand words through it.

Nothing else gets written. If it is worth keeping, it belongs in one of these four.

## Step 0 · The calls first, then the business

**First, a self-check, before you ask the founder for anything.** Three files inside THIS
skill's folder, next to `SKILL.md`, must open: `references/scorecard.md`,
`references/research-method.md`, and `references/card-template.md`. If any is missing,
stop right here and tell the founder to finish the install: copy the whole skill folder,
`references/` included. A broken install caught after the intake costs them the intake.

**Then open the calls before you ask for anything.** The founder just spent a week in
the Warm Start, sending by hand and talking to people who already know them, and the Warm
Start wrote every line down. First act of this run: read `squad/warm-notes.md` yourself,
plus `squad/warm-list.md` if it exists (the pasted Warm tab rows are the list otherwise), plus `squad/draft-offer.md`, the
pile of per-person service ideas the warm week stacked up, one after each call, written by
the Warm Start. Read that pile as draft thinking, never as a decision: this run forges
those sketches into the card. Never make the founder re-narrate
a call whose words are already on disk.

Then ask, in one message, for the two things that are not on disk:

- **the Outreach Sheet rows.** The sheet lives in the founder's Google Drive and you
  cannot open it: ask them to copy the Warm tab and paste it here, header row included,
  all seven columns. Column 5, `What they said on the call`, outranks the rest, and the
  objections live in the `NOT NOW` rows plus that column; the founder's summary of what a
  buyer needs is worth nothing next to the buyer's own line.
- **anything they kept somewhere else**: a doc, a notebook, a paste into this chat, or just
  talking the calls back to you now while you write them down. When this repo has no
  `squad/warm-notes.md` at all, say so plainly and make this the whole intake.

Then mine them, which is not the same as skimming them. Pull every line a buyer actually
said, verbatim, and write it into `squad/offer-research.md` under `## BUYER LANGUAGE`,
each quote labeled with where it came from in the form `(warm call · Mina K · Aug 14)`.
Five things earn their own quotes, and the Warm Start captured them in this order:

1. **The words they used for the problem.** Their nouns, not the founder's. These become
   the sentence and the promise later, and no scraped phrase outranks them.
2. **What they asked for that nobody sells them.** An unprompted ask is an empty seat with
   a witness, and it beats any seat you find by searching.
3. **What the problem costs them today**, in money, hours, or lost jobs. This is what the
   value equation runs on at BUILD, and a real number from a real call is worth more than
   a market average.
4. **What they already pay for today**, named and priced where they said it. That is the
   line the price sits next to at BUILD, and a real competitor with a real number beats a
   category you looked up.
5. **Every NOT NOW reason, word for word.** A NOT NOW is an objection with a name attached.
   The ATTACK beat is graded against these, not against objections you imagined.

Say the read back in one line before you move: how many conversations you read, how many
quotes you pulled, and what the calls never touched. That last part is the research brief
for steps 2 and 3.

**No notes, or fewer than five conversations?** Say it plainly, once, without a lecture:
the offer built from research alone is weaker, because it is assembled from what strangers
say in public rather than from what your own buyers said to your face, and the card's mode
line carries how thin the read was. The blind spot is gate 6's, always. Then the smaller run, which is the default: proceed now, and
re-open this run after the next five conversations land, from any lane. Going back beats
going forward on a count, not a feeling: nothing sent yet at all, or graded names still
unsent outnumbering the sent ones. Either way say so, point back at g3's warm week, and let the founder pick. A list already
in motion runs now; a founder whose list is spent never gets sent back to wait.

**Then the five answers.** Ask, in one message, only these:

1. What do you sell, in one sentence?
2. Who buys it? (job title or situation, not demographics)
3. What does it cost, and how does it get delivered?
4. How did anyone who ever paid you find you? If nobody has, say so.
5. Is there something different you keep thinking you SHOULD sell instead? (This catches
   the switching itch. Carry the answer all the way through: the market read tests that
   category as one of the seats, the card gives it one line, and the verdict resolves it.)

**Nobody has paid yet?** That is the founder this arc was built for, not a failure.
Questions 3 and 4 get one honest line each and the run fills the hole elsewhere: the warm
calls stand in for customer history, the price comes off the operator table at the numbers
gate rather than off a sale that never happened, and THE STACK lists what the founder can
deliver next week rather than what has shipped. Never interrogate someone for a customer
history that does not exist.

If an answer is vague, ask a follow-up. Keep asking until you could explain this business
to a stranger in two sentences, and stop the moment the honest answer is that there is
nothing there yet. Save them to `squad/business.md` under one heading,
`## THE FIVE ANSWERS`, one labeled line per question; the resume check reads that heading,
and step 8 replaces the whole thing with the card. Where a call already answered one of
the five, show the founder the quote and ask them to confirm or correct it, rather than
making them type an answer they already gave a buyer out loud.

## Step 1 · Confirm, then check the tools

Play back what you heard in two sentences, the calls included: what the buyers said, and
what the calls left open. List exactly what you are about to research and why, in plain
words, and every line on that list traces to a gap the calls left. Then show the seven
gates from `references/scorecard.md` as the test this run will be graded against: the
founder sees the test BEFORE any research exists. Get a yes before running anything.
Research without agreement gets thrown away.

**In the same message, check the tools.** Probe each with a free call: `search-actors`
for Apify, `search` for Perplexity. Never use a run-starting tool as the liveness check;
Apify's `call-actor` starts a billed run, and a founder on the free tier should not pay for
a handshake. Wired means callable right now, in this session; a tool that errors on auth is
not wired. Say which mode this run is in. **Apify is the one that matters and the install
lesson wired it; Perplexity is optional there**, so a run with Apify live and Perplexity
absent is a normal wired run, and pass 2's direction read falls back to search. A founder
with no Apify goes back to the install lesson rather than into a procedure here. The run goes either way. Unwired it runs on the ladder in
`references/research-method.md`, the card prints the mode, and Reddit (the best public
source of buyer language once the calls are mined) is missing from the read entirely. Say
that here, before they decide, never after the card prints.

## Steps 2-3 · LISTEN, then MAP

Read `references/research-method.md` and follow it exactly, with two standing amendments.

**One: the warm calls already ran pass 1 for you**, so these two steps FILL GAPS instead of
starting cold. Work the gap list you read back at step 0.

**Two: the thin test counts PUBLIC quotes only**, on the rule
`references/research-method.md` owns. Under about five public quotes fires two things and
only two: that file's founder ask, and the thin flag on the card's mode line. It never
reaches THE STACK's fear column, which runs on its own ladder in
`references/card-template.md`.

LISTEN searches for what the calls did not cover: the buyers nobody on the warm list
represents, the objection nobody voiced, the price nobody named. Scraped quotes append
BELOW the warm quotes under `## BUYER LANGUAGE`, each with its own source label, so anyone
reading that file later sees which lines came from a conversation and which came from a
stranger on the internet.

MAP runs in full every time, gaps or no gaps. The calls tell you what buyers feel; only the
market read tells you what is already being sold to them and for how much, and no number of
warm conversations replaces that.

## Steps 4-7 · THE MODEL, then BUILD, SCORE, ATTACK

Read `references/scorecard.md` and follow it exactly, in its order: the model check, the
value equation, the seven gates, the three self-attacks.

**STOP after the model check: the founder decides the numbers.** Present the model pick
with its precedent, and a price structure as a PROPOSAL. The founder confirms or adjusts.
You never print a price, a tier, or a cap the founder did not decide. (Money and identity
decisions are always human; the research only argues.) This same gate collects the
founder's number chain for gate 7, over the window that gate names, and missing numbers
are asked HERE, never mid-SCORE.

**The founder will not name a price.** The commonest refusal at exactly this moment, so it
gets a procedure instead of a stall. Hold the operator table up, name the lowest published
number in it, and ask for a yes or a no on that one number; a closed question gets answered
where an open one does not. **When nothing in the table is published** (a whole market
behind call-closed pricing is normal, and is itself the transparency seat), the closed
question needs a different number, in this order: the founder's own current rate or day
rate from the five answers, then the lowest number a buyer named on a warm call, whether
they were quoting a competitor or what they pay today. Hold that one up the same way, and
say where it came from. Still a deflection, and the number prints as the card's price
marked `(proposed, not yet said out loud)`, and saying it out loud becomes the week-one
attack. PRICE never prints blank.

Then BUILD the sentence and the promise through the value equation, written in the words
the calls gave you. SCORE the seven gates, receipts or nothing, and where a gate can be
graded off something a buyer said on a call, grade it off that; a scraped receipt is the
fallback, and a receipt with no source is not a receipt. ATTACK your own draft three ways,
in writing, before showing anything, and run it against the real NOT NOW reasons from the
Outreach Sheet before any objection you invent.

## Step 8 · THE CARD

Read `references/card-template.md` and produce the one-page offer card in exactly that
structure, written INTO `squad/business.md`, replacing the five answers (fold anything
still useful from them into the card's WHO and MODEL sections). One file, one page: the
business file's finished form is the card.

Print the complete card, verdict included, then stop; re-print only the lines the founder
changes.

**The stop is the founder's, and it has three parts.** First the voice pass: ask them to
read the sentence and the promise out loud and change any word that does not sound like
them. The card is theirs the moment they can say it at a dinner table without reading.
Second, the two BRAND decisions the card's last line needs: their ONE accent color (a hex)
and the ONE product word they use for what they sell, plus any synonym they refuse. Write
both onto the card's BRAND line. "(none yet)" goes there only when the founder declines to
decide, never because the ask was skipped; step 10 and every thumbnail after it read that
line. Third, the verdict itself: ask for their yes, out loud. The moment it comes, stamp the
card's last line with `confirmed <today's date>`; that stamp is the only record the gate
happened, and the resume check reads it. A no is not a request for a different offer, it
is an objection with a name: take the thing they objected to, run ATTACK against that, and
re-print the lines it changes. Never answer a no with a menu.

**Card self-check before the stop.** Every unconditional heading in
`references/card-template.md` is present, THE VERDICT and BRAND included. Each conditional
heading is present or its condition is false, and the three conditionals are: SCARCITY +
URGENCY (absent when nothing is genuinely scarce), THE SWITCHING ITCH (only when step 0,
question 5 surfaced one), and WHAT WEEK ONE MAY ATTACK NEXT (absent when nothing wanted
the verdict's blank). Never invent content so a heading can appear. The skills after this
one read these headings by name.

## The verdict

The card ends on exactly one of the two forms printed word for word in
`references/card-template.md`, and on nothing else. A gate-2 kill is the third ending: it
builds no card at all and closes on the line in step 9, a different buyer rather than a
different offer.

**The week-one blank belongs to `references/scorecard.md` gate 7**, the only place that
rule lives, its unsaid-price override included. Everything that wanted the blank and did
not get it (the switching itch's first paid test, any unscored gate, the undecided
one-tenth find, a stage that does not exist in the funnel yet) lists in the card's WHAT
WEEK ONE MAY ATTACK NEXT section, never inside the blank. When step 0, question 5 surfaced
a switching itch, the itch is resolved in the card's SWITCHING ITCH line directly above the
verdict.

## Step 9 · THE BANK

After the verdict, one more conversation. The bank runs on BOTH verdicts; proof and
voice belong to the founder, not the offer. Build `squad/credibility-bank.md` by asking, a
few questions at a time, until each section holds real entries or an honest "(none yet)".
Ask first, in this same chat, exactly like the five questions: the founder's answers only.
Never prefill the bank by mining their files or past work; anything you already know
becomes a suggestion offered AFTER their answer lands, never a draft written for them. The
bank is their voice or it is nothing. A section with nothing real in it (a freelancer with
two clients has no client results yet) is written as "(none yet)" and said out loud as the
first thing the next 90 days should produce. A filled section with no receipt behind it is
worse than an empty one, because every later agent pulls its proof from here precisely so
it never has to invent any.

The six headings are written by exact string, every run, because the skills after this one
resolve them by name: the Close appends a first receipt under `## 1 · WINS, each with its
mechanism` or `## 4 · CLIENT RESULTS, verbatim`, and the Proven Package checks all six
before it will package anything and re-interviews for whichever is missing. A heading that
drifted is a section that is gone, on a file that is actually full.

1. **`## 1 · WINS, each with its mechanism`.** What have you actually done, and HOW? A
   number without its mechanism does not go in ("$50K/month" is a claim; "$50K/month, solo,
   300 cold emails a day" is proof).
2. **`## 2 · LOSSES that built you`.** What did you try that died, and what did it teach
   you? Losses buy more trust per second than wins. A bank with no losses reads as a resume.
3. **`## 3 · THE NEVER-LIST`.** What do you refuse to do, even for money? These become the
   refusals every sales surface can quote.
4. **`## 4 · CLIENT RESULTS, verbatim`.** Your result proves you can do it; a client's
   result proves it transfers. Verbatim words, never paraphrased.
5. **`## 5 · PROOF-ASSET LIST`.** Every artifact that backs a win: a screenshot, a
   recording, a dashboard, a testimonial file. One line each: what it shows, where the file
   lives. Later agents pull proof images from this list, never from a claim alone.
6. **`## 6 · VOICE NOTES`.** How the founder talks about their work: the phrases they always
   use, the words they refuse, and 3-5 lines straight from their mouth (this chat is full of
   them; confirm, do not invent). Write the answers under that heading even when they are
   short; the script and package agents read that section by name, and a missing section
   reads to them as a founder with no voice.

**A gate-2 stop lands here too.** When gate 2 killed the run (`references/scorecard.md`:
the buyer has no money), no card gets built, but this step and step 10 still run, because
the proof, the voice and the roots file belong to the founder rather than to that offer.
Then say the next move in one line: a different buyer, not a different offer.

## Step 10 · THE ROOTS FILE

Last thing, no questions asked. `.claude/squad-roots.md` is the per-repo instance file
every skill after this one reads first, and the install lesson created it. Fill only the
fields THIS run answered, in place, and change nothing else:

| Field | Value |
|---|---|
| founder name | <as they say it on camera>, when that row is still blank |
| product word | <the one word> (banned synonyms: <the words they refuse>) |
| accent color | <the hex from the card's BRAND line, or (none yet)> |
| data sources | `squad/business.md` · `squad/offer-research.md` |
| credibility-bank | `squad/credibility-bank.md`, the file step 9 just wrote |
| research mode | <what this run used: wired, or the unwired ladder> |

Never guess a row, and never write a field this run did not answer. Every later skill fills
what it learns the first time it learns it, and adds its own row when it needs a field this
file does not carry yet (the lane, the week folder, the image bank, the cage canvas). No
file at all, and no legacy `.claude/spine-roots.md` either? Write it with the rows above.
Then say one line to the
founder: this file is where their name, brand word, color and paths live,
and every later part of the system reads it.

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
