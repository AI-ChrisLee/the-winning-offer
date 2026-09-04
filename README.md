# The Winning Offer: install in 60 seconds

The offer part of an Execution Squad. One equation, 2 doors in, one document out.

**Warm, the main road.** After every call with someone who already knows you, say
**"I talked with ____. Here is the recording: ____"** (or the transcript). It writes that
person's folder under `squad/clients/`, then rebuilds your offer document at
`squad/business.md` from every call so far. 1 to 5 calls, and after each one you say
"one more call" or yes.

**Cold, the fallback.** Know nobody yet, or the calls gave you nothing? Say **"Run the
Winning Offer."** It asks 5 questions, reads where your buyers write their problems out and
what the winners charge, and builds the same document from the market.

Both score the same 7 gates and end on one answer: this holds, here is the blind spot,
start. Then you stop choosing.

## Run it

The Winning Offer lesson put this skill in `.claude/skills/` (g4, step 5; g5, step 1). Open Claude Code in
your business folder and say the line above for your door. (Downloaded this folder on its
own instead? Drop the whole thing into `.claude/skills/`, then quit and reopen Claude Code.)

On a first run, Claude Code asks permission before its first file writes and searches; those
prompts are normal, allow them.

Stopped halfway, or closed the laptop? Say **"continue the Winning Offer"** in a new window.
It reads what is already on disk and picks up at the first thing missing.

## What to bring

- **A recording** (`.m4a`, `.mp3`, `.wav`, `.mp4`, `.mov`) or **a transcript** (`.txt`,
  `.md`, `.srt`, `.vtt`). The first time you hand over a recording it asks one yes to put a
  small transcriber on your laptop; nothing is uploaded anywhere. Record on Zoom from the
  desktop app, or the phone's recorder in person.
- **Nobody to call?** Say "self-interview". It asks you the 5 questions about who you were
  before you learned what you know now. Last option, and the document says so.

## Apify, optional

Want Reddit and the YouTube comments in the cold read? Get a free token at apify.com
(Settings, API & Integrations, API tokens) and paste: **"Here is my Apify token: ____. Use it
for the Winning Offer."** Your squad wires it and tells you to reopen Claude Code. Without it
the run still goes; the document says the read was thinner.

## What you get

One page at `squad/business.md`: what you sell in one sentence, the promise, who it is for,
what is inside, the price and its terms, the 7 gates with receipts, and the answer. When
Google Drive is connected (g2) the same document lands in your Google Docs and the link is
printed. Then 6 short questions build your proof file, `squad/credibility-bank.md`, which
every later part of the system quotes instead of inventing.

Next: g6 sells it, g7 builds the deck, g8 turns the first 90 days into weeks.
