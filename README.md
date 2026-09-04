# The Winning Offer: install in 60 seconds

The offer agent of an Execution Squad, and the second part of the run: Warm Extract
listened, this one decides. It exists to kill one question: "is my niche even right?" It
reads your own warm call notes first, fills what the calls could not answer with real
market research, and hands you a one-page offer document with one answer. Then you stop
choosing and start.

## What to bring

Your calls. Warm Extract wrote each one into its own folder, `squad/clients/<name>/notes.md`,
and the draft offer into `squad/business.md` when a call handed one over; this run opens
them itself, and it asks you to paste the NOT NOW rows of your Outreach Sheet's Warm tab next
to them. Notes kept somewhere
else are fine: a doc, a notebook, or just talking the calls back while it writes them
down. No calls yet and the run still goes; the document carries that as its blind spot.

## Run it

Step 1 of the Winning Offer lesson put this skill in `.claude/skills/` and wired Apify.
Open Claude Code in your business folder and say: **"Run the Winning Offer on my
business."** (Downloaded this folder on its own instead? Drop the whole thing into
`.claude/skills/`, then quit and reopen Claude Code.)

It reads your calls, asks five questions, confirms what it is about to research, and comes
back with your one-page offer document: what your offer is in one sentence, the promise, who it
is for, what is inside, the price and its terms, and the answer. On a first run, Claude
Code asks permission before its first searches and file writes; those prompts are normal,
allow them.

Stopped halfway, or closed the laptop? Say **"continue the Winning Offer"** in a new
window. It reads what is already on disk and picks up at the first thing missing.

## The two tools

Apify is the one that matters, and Step 1 of the Winning Offer lesson wires it (five
minutes, once). Perplexity is optional and no lesson wires it, so Apify alone is a normal wired run.
This run only checks them at its first stop, and tells you which mode it is in. Reddit is
where your buyers write their problems out in full sentences and Claude Code cannot open it
alone, so unwired the read is thinner, Reddit and the YouTube comments are missing from it
entirely, and the document says so. Skipped Step 1? Go back and do it there; the
`mcp.json.example` in this folder is the config that paste uses. The run goes either way.

## What you get

One page and one answer. Either "this holds, here is the blind spot, start," or "this
fails at gate X, fix that first." No option menus, no "it depends."

Three parts come next: the one that runs the sales call (one general script, one personal
question before every call, the debrief after it), the one that builds the shell you put on the
screen in the sales hour, and the one that turns your first 90 days into weekly tasks sized to
your hours. They arrive one episode at a time. Subscribe (the link under every episode) and each
new part lands in your inbox the day its episode goes live.
