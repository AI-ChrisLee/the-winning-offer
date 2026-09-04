# The offer document (the Winning Offer: THE DOCUMENT)

One page, read on a screen. These headings, this order, nothing else.

## The law

- A heading per section, by exact string, in the order below.
- One-line paragraphs. No paragraph over 40 words. No section past one screen.
- A table wherever there are 3 or more columns of facts: THE STACK always, PRICE when it has rungs or tiers, THE NUMBERS when a chain exists.
- Bold on the lines the founder says out loud: THE SENTENCE and THE ANSWER. Nothing else bold.
- Plain markdown in `squad/business.md`. The HTML below is made only for the Google Doc.

## THE DREAM OUTCOME
One line, in the buyers' words, quoted like they would say it, with its source label.

## THE MODEL
One word for the model, then what is mixed, in one line.
Example shape: "Hybrid: done-for-you plus one thing you do."
A pure 1-on-1 service is one word with no mix. Never force a hybrid.

## THE SENTENCE
The one sentence. Bold, alone.

## THE PROMISE
Three sentences at most, one per line.
The honesty line when a time claim exists: "X days to ready, not X days to results."

## WHO
Line 1: who it is for.
Line 2: who gets refused and why. A named refusal builds more trust than any claim.

## THE STACK (everything included)
A table, one row per part: `the part · the fear it kills · what they get`. Delivery details live in the row they belong to.
The fear cell is a quote in quotation marks with its label: `(warm call · Name · date)`, `(scraped · source)` or `(founder's own read, unsourced)`.
That is a ladder, and it climbs down only when a rung is empty. A document carrying warm quotes never prints the last form. Never blank, never unmarked, never a quote nobody said.
The stack lists what exists today. Anything new the research suggests goes in WHAT WEEK ONE MAY ATTACK NEXT, never silently into the stack.
Sparse and true beats padded. A service has fewer rows than a productized system.
Never force an owned-forever vs rented split on an offer with no one-time part. The stack mirrors the model.
An owned asset not yet a deliverable (an unmailed list, an unused review base) still gets a row, labeled as an asset.

## PRICE
Line 1: the number, one payment or the recurring fee, and how it is paid.
Rungs or tiers print as a table. `stage · trigger · price` for a price that rises on a ladder. `package · what's inside · price` for a market whose operators all sell named tiers.
One price with no rungs: one line, no table.
Never invent tiers the founder has not decided. A tier table the founder decided at the numbers gate is a price, not a menu.
Then the terms, one line each: what is included, what happens on cancel, why the price rises (a real reason, or no rise).
A recurring fee's cancel line names what stops. A cancel line that names nothing is not ready to print.
Short is the honest outcome, not under-delivery.

## THE WARRANTY
Only what the founder controls. Never outcomes.
One line per condition, and what happens when it is missed.

## SCARCITY + URGENCY
Only if real: one line, with the reason. Nothing scarce, and the section is absent.

## THE REFUSALS
One line each: no income promises, no invented numbers, no fake deadlines, then this market's own worst habits.

## THE NUMBERS
A table when a chain exists: `stage · count · note`. The stages carry the founder's own log names (sent, replies, calls, money, plus views and clicks where a content lane exists).
Under it one line: the window the counts cover, and the stage week one attacks.
A stage that does not exist yet is "not in play", never zero and never uncounted. Only a stage nobody counts can take the week-one blank.
The full chain lives in `squad/offer-research.md` under `## SCORECARD`, next to gate 7.

## THE SWITCHING ITCH (only when C0, question 5 surfaced one)
One line: the thing the founder keeps thinking about switching to, and what the research found.
The itch resolves here. Its first paid test goes in WHAT WEEK ONE MAY ATTACK NEXT, never in the answer's blank.

## THE ANSWER
The document's last judgment. Bold, exactly one of these 2 forms, word for word:

**"This offer holds. The blind spot is ___. Week one attacks ___. Stop choosing. Start."**

**"This offer fails gate ___ because ___. Fix that before you build anything else."**

The week-one blank goes to the weakest stage of the number chain, by the rule in `scorecard.md` gate 7.

## WHAT WEEK ONE MAY ATTACK NEXT
One line each, no ranking: the itch's first paid test, any unscored gate, the undecided one-tenth find.
Absent when there is nothing in it.

## BRAND (one line, the document's last section)
The founder's one accent color (a hex) and the product word, plus any synonym they refuse.
Asked at THE YES, in the same breath as the sentence. "(none yet)" only when the founder declines, never a color chosen for them.
The thumbnail work reads this line and the roots file copies it.

## The mode line
The document's last line, small: `warm · N calls`, `warm · self-interview only`, `cold · market` or `cold · market + N calls`.
A cold run adds the tool mode in parens (`wired`, or `unwired ladder`) and `thin` when the public read came back under about 5 quotes.
The yes adds `confirmed <date>`. That stamp is the only record the answer was approved, and a later session reads it to know whether the gate still owes a run.

## The Google Doc
Made on the yes, when a Drive connector answers (found by shape: a tool named `create_file` on a UUID-prefixed server).
The document is rendered to HTML: `<h1>` for the title, `<h2>` per section by the same strings, `<p>` per line, `<b>` on THE SENTENCE and THE ANSWER, `<i>` on the mode line.
Every table is `<table border="1" cellpadding="6">` with a `<tr><th>` header row: THE STACK, PRICE when it has rungs, THE NUMBERS when a chain exists.
No CSS, no `<div>`, no markdown left inside the HTML.
Created with `create_file`: `title` "Offer document · <founder name>", `contentMimeType` `text/html`, the HTML as `textContent`. It lands as a formatted Google Doc.
The link it returns is printed to the founder and written to the roots row `offer doc`.
A later yes after a rebuild makes a new Doc with the same title, and the row takes the new link.
