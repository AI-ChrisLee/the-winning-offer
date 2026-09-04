# The Winning Offer: install in 60 seconds

The offer part of an Execution Squad. One equation, 2 doors in, one document out.

**Warm, the main road.** Record each call with someone who already knows you. Drop the
recording or the transcript in `squad/interviews/`, named after the person (`daniel.m4a`,
`daniel.txt`). Then say **"/the-winning-offer I put my interview with Daniel in
squad/interviews. Build the offer from it."** It reads every file in that folder it has not
read yet, writes one folder per person under `squad/clients/`, rebuilds your offer document
at `squad/business.md` from every call so far, and puts it in your Google Docs. 1 to 5 calls,
and after each one you say "one more call" or yes.

**Cold, the fallback.** Know nobody yet, or the calls gave you nothing? Say **"Run the
Winning Offer."** It asks 5 questions, reads where your buyers write their problems out and
what the winners charge, and builds the same document from the market.

Both score the same 7 gates and end on one answer: this holds, here is the blind spot,
start. Then you stop choosing.

## Run it

The Winning Offer lesson put this skill in `.claude/skills/` (g4, step 5; g5, step 1). Open
Claude Code in your business folder and say the line above for your door. (Downloaded this
folder on its own instead? Drop the whole thing into `.claude/skills/`, then quit and reopen
Claude Code.)

On a first run, Claude Code asks permission before its first file writes and searches; those
prompts are normal, allow them.

Stopped halfway, or closed the laptop? Say **"continue the Winning Offer"** in a new window.
It reads what is already on disk and picks up at the first thing missing.

## What to bring

- **One file per call in `squad/interviews/`, named after the person.** A recording (`.m4a`,
  `.mp3`, `.wav`, `.mp4`, `.mov`) or a transcript (`.txt`, `.md`, `.srt`, `.vtt`). The first
  time it meets a recording it asks one yes to put a small transcriber on your laptop;
  nothing is uploaded anywhere. Record on Zoom from the desktop app, or the phone's recorder
  in person.
- **Nobody to call?** Say "self-interview". It asks you the 5 questions about who you were
  before you learned what you know now. Last option, and the document says so.

## Apify, optional

Want Reddit and the YouTube comments in the cold read? Get a free token at apify.com
(Settings, API & Integrations, API tokens) and paste: **"Here is my Apify token: ____. Use it
for the Winning Offer."** Your squad wires it and tells you to reopen Claude Code. Without it
the run still goes; the document says the read was thinner.

## What you get

One page at `squad/business.md`: what you sell in one sentence, the promise, who it is for,
what is inside as a table, the price and its terms, the numbers, and the answer in bold. When
Google Drive is connected (g2) the same page lands in your Google Docs as "Offer document ·
<your name>", headings and tables intact, and the link is printed.

Next: g6 sells it, g7 builds the deck, g8 writes your 4-week plan.
