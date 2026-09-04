---
name: the-winning-offer
description: Use this when the founder is building their offer, from people they already know or from the market. They say "/the-winning-offer I put my interview with <name> in squad/interviews. Build the offer from it." (the warm entry; the old "I talked with <name>. Here is the recording: <path>" and a pasted transcript still work), "/the-winning-offer warm", "self-interview" (nobody to call), "/the-winning-offer", "run the Winning Offer", "/the-winning-offer cold", "run the offer check" or "write my offer card" (the old names for the same run), "Here is my Apify token: ____. Use it for the Winning Offer." (the optional wiring), or "continue the Winning Offer" (picking a stopped run back up). 2 entries, one equation, one document. Warm: every interview dropped in squad/interviews/ becomes a folder under squad/clients/ and squad/business.md is rebuilt from every call so far. Cold: 5 questions, then the market read. Both score the same 7 gates and end on one answer: this holds, here is the blind spot, start. On the yes the document goes to Google Docs when Drive is connected. It never sends, never prices past the number the founder said, and never invents a quote.
---

# The Winning Offer

One equation, 2 sources. **Your work, in one line: turn what buyers said, on a call or in
public, into ONE offer document at `squad/business.md`, scored through 7 gates, closed on one
answer, and put in the founder's Google Docs.** The founder's part: the calls, one file per
call in `squad/interviews/`, the yes on the words, and one number.

Warm outranks cold. An offer built from 1 to 5 calls with people who already know the founder
is written in the buyers' own nouns. An offer read off the market is written from what
strangers say in public. So the warm entry is the main road, and the cold entry is the
fallback for the founder who honestly knows nobody, or whose calls gave nothing. Both end in
the same file, the same gates and the same 2 closing sentences. A gate the calls never touched
prints `unscored: no call touched it`, and that blank is what the cold run, or week one,
attacks. Client folders, when they exist, are read first on every run, and a line from a call
outranks a line from a scrape every time.

This skill runs in ANY founder's repo. `.claude/squad-roots.md` is the per-repo instance file
every member-run skill reads first (founder name, voice sample, and the rows this skill
fills), and its values win over the `squad/` paths below, which are worked examples. A row
reading "(none yet)" is an unanswered field, not an override. Legacy repos carry
`.claude/spine-roots.md`: read that as the fallback, and write the roots file when neither
exists.

## The 2 entries, and how they are called

| Entry | The founder says | Beats |
|---|---|---|
| warm | "/the-winning-offer I put my interview with <name> in squad/interviews. Build the offer from it." (the old "I talked with <name>. Here is the recording: <path>", or a pasted transcript, still work); `/the-winning-offer warm`; "self-interview" | W0 and W1 once per unprocessed file, then W2 and W3 once. Then the close |
| cold | `/the-winning-offer`, "run the Winning Offer", `/the-winning-offer cold`, or no interview offered | C0 to C7. Then the close |
| wiring | "Here is my Apify token: ____. Use it for the Winning Offer." | the one paragraph in C1, then stop |

A bare "continue the Winning Offer" reads the outputs, picks the beat off the resume table, and
says in one line which entry it entered and why.

## The run map (where you run, where you STOP)

| Beat | Mode |
|---|---|
| W0 THE INTERVIEWS | HUMAN INPUT: the recording or the transcript dropped in `squad/interviews/`, named after the person. AUTO: every file in that folder the run has not processed is read; audio and video are transcribed on the laptop, after one yes, once. One question only when nothing says who the person is |
| W1 THE FOLDER | AUTO: `transcript.md` (its first line naming the source file), `notes.md`, the `clients` and `interviews` roots rows once |
| W2 THE DOCUMENT | AUTO: `squad/business.md` rebuilt from every folder so far. HUMAN INPUT, at most 2 questions, only for what no call answered: the sentence, the price |
| W3 THE YES | **STOP · GATE: the document whole. "One more call" ends the run for tonight; the yes stamps it** |
| C0 THE FIVE | HUMAN INPUT: the 5 answers, pre-filled from a warm document when one exists |
| C1 THE PLAN | AUTO: the tool check, the gap list, the 7 gates shown. Then **STOP · GATE: the yes before any research runs** |
| C2 LISTEN | AUTO. One exception: under about 5 public quotes, ask the founder to paste more, then continue |
| C3 MAP | AUTO |
| C4 THE NUMBERS | AUTO: the model check. Then **STOP · GATE: the founder decides the price, one number** |
| C5 BUILD · SCORE · ATTACK | AUTO |
| C6 THE DOCUMENT | AUTO: written whole into `squad/business.md` |
| C7 THE YES | **STOP · GATE: the same gate as W3** |
| THE DOC | AUTO: the Google Doc when a Drive connector answers; one line when it does not |
| THE ROOTS | AUTO: the rows this run answered |

The close (THE DOC, THE ROOTS) runs after either yes. Never pause an automated beat to ask a
small question (batch it into the next gate); never run through a gate because the answer
seems obvious.

**Resuming.** The rule keys on the OUTPUTS, never on a session's memory. Check them in this
order and continue at the first one missing or incomplete.

| Missing or incomplete | Resume at |
|---|---|
| `squad/interviews/` holds a transcript or recording file whose name no `squad/clients/*/transcript.md` carries on its first line | W0 for that file, then W1, then the rebuild |
| nothing exists under `squad/` yet | no run has started: say so in one line and ask which entry, since a file in `squad/interviews/` starts the warm run and "cold" starts the cold run |
| `squad/offer-research.md`'s `## SCORECARD` records gate 2 failing, and `squad/business.md` holds no offer document (it is absent, or holds only `## THE FIVE ANSWERS`) | the run is over. Say gate 2 killed it, name the receipt, and turn the conversation to which buyer has money. Never re-enter research and never build the document |
| a `squad/clients/*/` folder holds `transcript.md` and no `notes.md` | W1 for that folder |
| a `notes.md` is newer than `squad/business.md`, or its quotes are not under `## BUYER LANGUAGE` in `squad/offer-research.md` | W2, the rebuild |
| `squad/business.md` holds `## THE FIVE ANSWERS`, and `squad/offer-research.md` either has no `## ALLOWED WORDS` or its `## ALLOWED WORDS` still carries the warm placeholder | C1: restate the 5 answers for a confirm, never re-ask them. A `confirmed` stamp does not block this row: a warm document is the normal road into the cold entry |
| `squad/offer-research.md` exists, already holds `## BUYER LANGUAGE`, and is missing a later heading `references/research-method.md` names, on a cold run (a heading still carrying the warm placeholder counts as missing) | that heading's beat |
| the document exists and its last line carries no `confirmed <date>` stamp, or its BRAND line is blank | THE YES only: never re-run the research, never re-read the calls |
| the document is stamped, the roots file carries no `offer doc` row, and a Drive connector answers | THE DOC |
| `.claude/squad-roots.md` is missing a row this run answers | THE ROOTS |

A stamped document plus a new interview file is a rebuild: W0 and W1 run on the new file, W2
runs, the stamp comes off, and W3 asks the yes again on the lines that changed. Never re-ask a
question the files already answer; never re-run a research pass whose findings are on disk;
never parse a file a folder already holds twice.

## The outputs

1. `squad/business.md`: THE file. Its finished form is the one-page offer document, and every
   later skill reads it. On a cold run it first holds `## THE FIVE ANSWERS`; C6 replaces the
   whole file.
2. `squad/offer-research.md`: the receipts, under the exact heading strings
   `references/research-method.md` names, written every run. `## BUYER LANGUAGE` is compiled
   from `squad/clients/*/notes.md` first, on every run, and nobody else writes that heading. On
   a warm run the market headings hold "(not read: warm run; the cold entry fills it)" where no
   cold run has filled them; a filled heading is never overwritten.
3. `squad/clients/<first-last>/transcript.md` and `notes.md` (warm), one folder per person,
   `self/` for the self-interview. The first line of `transcript.md` is
   `source: <file name> · <date>` (`source: pasted · <date>` for a paste, `source:
   self-interview · <date>` for the self-interview); that line is the only record a file was
   processed.
4. `.claude/squad-roots.md`, given the `founder name` (only when blank), `clients`,
   `interviews`, `product word`, `accent color`, `data sources`, `research mode` and `offer
   doc` rows. Nothing else in it touched.
5. `.mcp.json` in the company folder, on the wiring paste only.
6. `~/.squad/whisper` (Mac and Linux) or `%USERPROFILE%\.squad\whisper` (Windows): the local
   transcriber, on a recording only, on the founder's one yes. That folder existing IS the
   record that the yes was given; a later recording goes straight to the transcription and the
   yes is never re-asked.

`squad/interviews/` is the founder's folder. This skill reads it, creates it empty when it is
missing, and never writes, renames or deletes a file in it.

Off disk, one thing gets created, on the yes only: the Google Doc "Offer document · <founder
name>", in the founder's own Drive. Nothing else gets written.

## The equation (both entries run through this)

**The install check, before you spend any of the founder's input.** 4 files inside THIS
skill's folder, next to `SKILL.md`, must open: `references/recording.md`,
`references/card-template.md`, `references/scorecard.md`, `references/research-method.md`.
Any missing: stop and say the folder was downloaded without its `references/`, and to copy
the whole skill folder in again.

**The document** is `references/card-template.md`, in that order, under its law (a heading
per section, one-line paragraphs, a table wherever there are 3 or more columns of facts, THE
SENTENCE and THE ANSWER in bold, no paragraph over 40 words, no section past one screen),
written INTO `squad/business.md` as the whole file. Every unconditional heading present, THE
ANSWER and BRAND included; each conditional present or its condition false (SCARCITY +
URGENCY only when something is genuinely scarce, THE SWITCHING ITCH only when C0 question 5
surfaced one, WHAT WEEK ONE MAY ATTACK NEXT absent when nothing wanted the answer's blank).
Never invent content so a heading can appear; later skills read these headings by name. **The
mode line**, the document's last line, reads `warm · N calls`, `warm · self-interview only`,
`cold · market` or `cold · market + N calls`; a cold run adds the tool mode in parens
(`wired`, or `unwired ladder`) and `thin` when the public read came back under about 5
quotes; the yes adds `confirmed <date>`.

**The 7 gates** are `references/scorecard.md`, in its order: the model check, the value
equation, the gates, the 3 self-attacks. Receipts or nothing. Where a gate can be graded off
something a buyer said on a call, grade it off that; a scraped receipt is the fallback. A gate
with no receipt prints `unscored`, on a warm run `unscored: no call touched it`, and an
unscored gate never fails the offer. Gate 2 failing kills the run (no document; a different
buyer, not a different offer, and THE ROOTS still runs because the rows already answered
belong to the founder); gates 1, 3, 4 and 5 failing print the second closing sentence; 6 and 7
are diagnostic. The document ends on exactly one of the 2 forms in the template, word for
word: **"This offer holds. The blind spot is ___. Week one attacks ___. Stop choosing.
Start."** or **"This offer fails gate ___ because ___. Fix that before you build anything
else."**

**The numbers gate: the founder decides the price.** One number, never a range, and you never
print a price, a tier or a cap the founder did not decide. For a service the ladder is $997,
then $2,997, then $4,997; a first offer starts on the first rung unless a call or the operator
table argues higher, and the founder picks the number. A number a buyer said on a call (what
they pay now, what they were quoted) is a fact to hold up, never the price. Present the model
pick with its precedent, the price as a proposal and, when there is a recurring fee, the day-31
cancel line, together, then stop. **The founder will not name a price:** hold up one number
(the lowest published operator price; when none is published, the founder's own current rate,
then the lowest number a buyer named), ask for a yes or a no on that one number, and say where
it came from. Still a deflection, and it prints marked `(proposed, not yet said out loud)`, and
saying it out loud becomes the week-one attack. PRICE never prints blank.

**THE YES has 3 parts, and it is the founder's.** Print the complete document, answer
included, then stop. First the voice pass: read the sentence and the promise out loud, change
any word that does not sound like you. Second the 2 BRAND decisions: the one accent color (a
hex) and the one product word for what they sell, plus any synonym they refuse; both go on the
BRAND line, and "(none yet)" goes there only when the founder declines, never because the ask
was skipped. On a rebuild both decisions are already answered: print them as they stand for a
confirm, and ask the 2 questions only for a line still blank. Third the answer: the yes, out loud. The moment it comes, stamp the mode line
`confirmed <today's date>`; that stamp is the only record the gate happened. A no is an
objection with a name: run ATTACK against the thing they objected to and re-print the lines it
changes. Never answer a no with a menu, and never print the whole document twice.

**THE DOC, after the yes.** Look for a Google Drive connector by shape, never by name: a tool
whose name ends in `create_file` on a server whose prefix is a UUID. Found: render the
document to HTML the way the "The Google Doc" section of `references/card-template.md` says
(an `<h1>` for the title, an `<h2>` per section by the same strings, a `<p>` per line,
`<table border="1" cellpadding="6">` for THE STACK, PRICE and THE NUMBERS tables, `<b>` on
THE SENTENCE and THE ANSWER), then call `create_file` with `title` "Offer document · <founder
name>", `contentMimeType` `text/html` and the HTML as `textContent`, reading the tool's own
schema in case a field name differs. It lands as a formatted Google Doc. Print the link it
returns and write it into the roots file as `offer doc`; a later yes after a rebuild makes a
new Doc with the same title, and the row takes the new link. Not found: one line, "connect
Google Drive (g2) and I put it in Docs next time", and carry on. Never stop for it, never ask
the founder to install anything here.

**THE ROOTS, last, no questions.** Fill only the rows THIS run answered, in place, and change
nothing else. Never guess a row.

| Row | Value |
|---|---|
| founder name | as they say it on camera, only when the row is still blank |
| clients | `squad/clients/` (warm, written once) |
| interviews | `squad/interviews/` (warm, written once) |
| product word | the one word (banned synonyms: the words they refuse) |
| accent color | the hex from the BRAND line, or (none yet) |
| data sources | `squad/business.md` · `squad/offer-research.md` |
| research mode | the tool mode off the mode line on a cold run; `warm only` when no cold run has happened |
| offer doc | the Google Doc link, when one was created |

Then one line to the founder: this file is where their name, brand word, color and paths live,
and every later part of the system reads it.

## The warm entry

### W0 · THE INTERVIEWS

Reads: `squad/interviews/` (the `interviews` roots row wins when it names another path). One
file per call, named after the person: `daniel.m4a`, `daniel-kim.txt`, `priya.vtt`.
Transcripts are `.txt`, `.md`, `.srt` or `.vtt`; recordings are `.m4a`, `.mp3`, `.wav`,
`.mp4` or `.mov`. Any other file in the folder is named in one line and skipped.

A file is processed when a `squad/clients/*/transcript.md` names it on its first line. Every
other file is this run's work, oldest first. The founder's line may name one person ("my
interview with Daniel"): still read every unprocessed file, and say which ones you found. The
founder never has to type a file name.

**No `squad/interviews/` folder, or nothing in it this run has not already processed:**
create the folder when it is missing, then one line, "drop the recording or the transcript in
`squad/interviews/`, named after the person", and wait. A transcript pasted into the chat, or
a path in the founder's own message, is read where it sits, so this never fires on those.

The person's name is the file name (`daniel-kim.txt` is Daniel Kim). The call's date comes
from the text, from the founder's line, or from the file's own date, in that order. One
question, only when the file name says nothing (`call-1.m4a`): "Who was this with?"

The old line still works. "I talked with <name>. Here is the recording: <path>" reads that
one file where it sits; a transcript pasted into the chat is read from the chat. The first
line of `transcript.md` then says `source: <path>` or `source: pasted`.

**A recording** gets transcribed here, on the laptop, the way `references/recording.md` says.
When the transcriber folder is not there yet (`~/.squad/whisper`, or
`%USERPROFILE%\.squad\whisper` on Windows), ask one yes: install a local transcriber
(faster-whisper through pip in its own folder). Say in the same line that the model weights
download once and the recording never leaves the laptop. That folder existing is the record
the yes was given, so a later recording goes straight to the transcription and the yes is
never re-asked. On the yes, run the install, then the transcription with the smallest model
that runs cleanly (that file names the order), and the text lands as this person's
`transcript.md`. A 20-minute call takes a few minutes; say so and wait. An install that fails
gets one line naming MacWhisper on a Mac or Buzz on Windows, "export .txt, drop it in
squad/interviews/", and then waits. Never a paid service, nothing uploaded.

- The founder's own account from memory is the floor. Take it as it comes, in any order, and
  label every quote `(founder's recollection · Name · date)`.
- Language is read, never asked. Quotes stay in the language they were said in; the notes and
  the document are written in the language of the roots file's voice sample.
- Never ask the founder to organise anything past one file per call in the folder. Messy is
  the format.

### W1 · THE FOLDER

Writes `squad/clients/<first-last>/`: the name as the file names it, lowercased and
hyphenated (a first name alone is the folder name; `self` for the self-interview).
`transcript.md` opens with `source: <file name> · <date>`, written by the transcriber itself
for a recording and by this beat for a transcript or a paste, and then holds the text as it
arrived; that first line is the record the file was processed, and it is never rewritten. A
`transcript.md` that came back without it gets the line added here, before anything else.
`notes.md` opens with `# Name · what they do · date` and holds these 7 headings, by exact
string, in this order, in one pass:

| Heading | Holds |
|---|---|
| `## QUOTES` | every line the person said that carries a problem, a cost, a spend, an ask or a next step, verbatim, each labeled `(warm call · Name · date)`; a one-line gloss under a quote in another language. A paraphrase is never saved as a quote |
| `## THE PROBLEM` | one line per problem, 3 at most, each pointing at the quote that carries it |
| `## THE COST` | a number the text supports (money or hours, and how often), or the question that would get it |
| `## WHAT THEY PAY NOW` | a fact line ("$400 a month on a VA"), or "unknown". Never a price |
| `## THE IDEA` | one line: what the founder would deliver to this person for this problem |
| `## THE MODEL` | one line: agency, consulting or software, and why in 6 words |
| `## THE NEXT STEP` | the date they agreed to, or "none" |

Then add the `clients` and `interviews` rows to `.claude/squad-roots.md` when they are not
there yet. Say: **Saved: `squad/clients/<first-last>/notes.md`**, then the 7 sections as
written. Another unprocessed file: back to W0 for it. None left: straight into W2.

### W2 · THE DOCUMENT

Read every `squad/clients/*/notes.md` on disk, this run's included, and rebuild
`squad/business.md` whole through the equation: the template, the gates, the closing sentence.
Every call-sourced line is rebuilt from the folders, never carried over from the last document,
so the third call can move what the first call set. `self/` is evidence about a buyer, never a
buyer.

- `## BUYER LANGUAGE` in `squad/offer-research.md` is compiled fresh from the folders: every
  quote, verbatim, with its label. `## SCORECARD` and `## ATTACK LOG` are appended under it;
  the market headings are written with "(not read: warm run; the cold entry fills it)" ONLY
  where the heading is absent or already carries that placeholder, so the later skills read an
  intentional gap. A market heading a cold run filled is left exactly as it stands; a warm
  rebuild never overwrites a market receipt.
- **When `squad/offer-research.md` already carries a cold run's market headings,** the rebuild
  keeps those receipts in the document (the operator table, the seats, the direction, and every
  gate the market scored) and only the call-sourced sections are rewritten from the folders.
  The mode line then reads `cold · market + N calls`. `warm · N calls` prints only in a repo
  where no cold run has happened.
- The receipts are the calls. THE DREAM OUTCOME, THE SENTENCE, THE PROMISE and the fear column
  of THE STACK are built from `## QUOTES`, in the buyers' words. THE MODEL is the model the
  folders agree on; when they split, the one the strongest quotes back, and say so. WHO refuses
  whoever the calls showed has no money or no urgency. With no cold run on disk, the WHAT THEY
  PAY NOW lines are the only operator table this run has; the shelf attack runs against those,
  and says so.
- Gate 7's chain is not asked here. A gate no folder gives a receipt for, and no cold run
  scored, prints `unscored: no call touched it`. The week-one blank goes to an unsaid price
  first, then to the earliest unscored gate.
- **What no call and no `squad/business.md` on disk answered gets asked, 2 questions at most,
  in one message, before the document prints:** what you sell in one sentence (only when no
  folder carries a named ask the founder will stand behind), and the price (one number, held
  against the ladder; the numbers gate's refusal procedure applies). A buyer's own number
  stays a fact on the WHAT THEY PAY NOW line.
- **The lines only the founder can decide carry forward.** THE SENTENCE, PRICE and the 2
  BRAND decisions come off the document already on disk and the roots rows `product word`
  and `accent color`. Print each as it stands for a confirm or a correction; never ask the
  question again on a rebuild.

The mode line reads `warm · N calls`, N being the folders that are not `self/`, and
`cold · market + N calls` when a cold run's market headings are already on disk.

### W3 · THE YES

THE YES from the equation, with one extra exit. Say it back in 3 lines first: the files
processed, by name; the document rebuilt from N calls; the closing sentence. Then the document
whole. **"One more call"** ends the run for tonight, the document stays unstamped, and the
next file in `squad/interviews/` rebuilds it. The yes stamps it, then the close runs: the
Google Doc, then the roots.

### Self-interview

Nobody to call is the trigger, and it is the last option: say so once. Ask the 5 questions one
at a time, in the past tense, about who the founder was before they learned what they know
now, and wait for each answer:

1. "What was the hardest part about your work back then?"
2. "Tell me about the last time that happened."
3. "Why was that hard?"
4. "What, if anything, did you do to try to solve it?"
5. "What didn't you love about what you tried?"

Then the exit question: **"Who is standing where you stood today that you could reach?"** The
chat is the transcript, the folder is `squad/clients/self/` (its `transcript.md` opens with
`source: self-interview · <date>`), every quote is labeled `(self-interview · Name · date)`,
and a name from the exit question gets its own folder when the real call lands in
`squad/interviews/`, not before. W2 runs on it; the mode line reads `warm · self-interview
only`, and under the closing sentence one more line: call one real person before you sell this.

## The cold entry

### C0 · THE FIVE

**Client folders first.** Read every `squad/clients/*/notes.md` on disk, compile
`## BUYER LANGUAGE` from them the way W2 does, and say the read back in one line: how many
calls, how many quotes, what the calls never touched. That last part is the research brief.
The Outreach Sheet's NOT NOW rows, when the founder has them, get pasted here too, header row
included; column 5 is the objection stage gate 7 reads. No folders: say once that the market
read is the thinner source, and go.

**Then the 5 answers, in one message.** A warm document at `squad/business.md` already
answers the first 3 (THE SENTENCE is 1, WHO is 2, PRICE and THE MODEL are 3): restate each and
ask for a confirm or a correction, never the question again. Otherwise ask only these:

1. What do you sell, in one sentence?
2. Who buys it? (job title or situation, not demographics)
3. What does it cost, and how does it get delivered?
4. How did anyone who ever paid you find you? If nobody has, say so.
5. Is there something different you keep thinking you SHOULD sell instead? (The switching
   itch. Carry it through: the market read tests that category as one of the seats, and the
   document gives it one line.)

Nobody has paid yet is the founder this arc was built for: questions 3 and 4 get one honest
line each, and the run fills the hole at the numbers gate. If an answer is vague, ask a
follow-up until you could explain the business to a stranger in 2 sentences, and stop the
moment the honest answer is that there is nothing there yet. Write them to `squad/business.md`
under `## THE FIVE ANSWERS`, one labeled line per question; a warm document stays as it is, and
`## THE FIVE ANSWERS` is written directly above its mode line so the `confirmed` stamp stays
the file's last line, until C6 rewrites the file.

### C1 · THE PLAN, then the yes

Play back what you heard in 2 sentences. List exactly what you are about to research and why,
each line tracing to a gap the calls left. Show the 7 gates from `references/scorecard.md` as
the test this run is graded against. **In the same message, check the tools:** probe Apify
with `search-actors` and Perplexity with `search`, free calls only (never `call-actor`, which
starts a billed run). Wired means callable right now, in this session; an auth error is not
wired. Apify is the one that matters and Perplexity is optional, so Apify alone is a normal
wired run. Say which mode this run is in and what unwired costs, in one line: Reddit and the
YouTube comments are missing from the read, so it walks the thinner ladder in
`references/research-method.md`, and the mode line says so. Then get the yes. Research without
agreement gets thrown away.

**The wiring, when the founder pastes "Here is my Apify token: ____. Use it for the Winning
Offer."** Write `.mcp.json` in the company folder yourself, from this skill's
`mcp.json.example`: the `apify` block with the token in place of the placeholder, the
`perplexity` block only when a key was pasted too, and an existing `.mcp.json` gets the block
merged in with nothing else in it touched. Never print the token back, never ask the founder
to open or edit a file. Then one line: quit and reopen Claude Code in this folder, and say
"run the Winning Offer" again. Nothing else runs in that turn.

### C2 · LISTEN, then C3 · MAP

Read `references/research-method.md` and follow it exactly, with 2 standing amendments.
**One:** the calls already ran pass 1, so LISTEN fills the gap list from C0 (the buyers no
folder represents, the objection nobody voiced, the price nobody named) instead of starting
cold, and scraped quotes go BELOW the warm quotes under `## BUYER LANGUAGE`, each with its own
source label. **Two:** the thin test counts PUBLIC quotes only; under about 5 fires that
file's founder ask and the `thin` flag on the mode line, nothing else. MAP runs in full every
time: only the market read says what is already sold to this buyer and for how much. State the
reason before each pass; write pass 1 to the file before pass 2 starts.

### C4 · THE NUMBERS

The model check from `references/scorecard.md`, then the numbers gate from the equation. A
warm document's price line is the proposal held up first, ahead of the operator table. This
gate also collects gate 7's number chain (sent, replies, calls, money, plus views and clicks
where a content lane exists), over the window that gate names, in one batch, never mid-SCORE.

### C5 · BUILD, SCORE, ATTACK

`references/scorecard.md`, in its order. BUILD the sentence and the promise through the value
equation, in the words the calls and the rooms gave you. SCORE the 7 gates with the receipt
next to each, under `## SCORECARD`. ATTACK the draft 3 ways in writing under `## ATTACK LOG`,
against the real NOT NOW reasons before any objection you imagine, and re-read THE PROMISE
against gate 6's weakest dial before anything prints.

### C6 · THE DOCUMENT, then C7 · THE YES

Produce the document into `squad/business.md`, replacing the whole file (`## THE FIVE
ANSWERS` and any warm document fold into WHO and THE MODEL). The mode line reads
`cold · market`, or `cold · market + N calls` when folders were read, with the tool mode and
the thin flag. Then THE YES from the equation, and the close.

## Rules

- Every message to the founder is scannable: a short header, then bullets or a table. Operator
  maps, price bands and gate grades go in tables. They are deciding, not studying.
- Never send anything, never post, never book.
- Never price past the founder's own number. One number, decided by them at the gate; a
  buyer's number is a fact, never the price.
- Never invent a quote, a number, a name or a need. A cost the text does not support is a
  question; a need nobody said stays out.
- Never paraphrase a quote, and never save a paraphrase as one. Verbatim, labeled, dated. A
  line from a call outranks a line from a scrape; same claim, 2 sources, the one with a name
  on it wins.
- Never a menu of options. The founder came here to stop deciding. Re-run this skill when a
  real season of data says to, not when the doubt itches.
- Never ask the founder to edit a file or organise their notes. The one thing they do by hand
  is drop one file per call in `squad/interviews/`, named after the person. The one install
  this skill makes is the transcriber, on one yes; only when that install fails does the
  founder install anything themselves, and then it is the one line in W0 and nothing more.
- Never make the founder re-narrate a call whose words are already on disk.
