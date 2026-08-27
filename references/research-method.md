# Research method (the Winning Offer, step 2)

Two passes, in this order. State the reason for each before running it.

## Pass 1 · The buyer's own language

Reason to state: "Everything that sells must be written in your buyers' words, so first we
collect them."

Search where this buyer actually talks, in this order:

1. **Reddit first.** Find the 3-5 subreddits where this buyer asks questions (search
   "[their job/situation] reddit"). Reddit is where pain arrives as full sentences:
   people ASK there before they buy anywhere. Pull the top and recent question posts
   plus their comment threads. Reddit blocks ordinary web tools, so use the wired
   scraping tool when one is set up (the Squad wires Apify for this). **No scraping tool
   wired? The whole pass still runs on Claude Code's built-in web search**, with three
   honest rules: (a) search MAY surface thread titles and excerpts; when it only
   paraphrases, cite the thread title plus the paraphrase and never turn a paraphrase
   into a quote; (b) when a rung returns ZERO results (not blocked, just nothing), say
   so and move down the ladder; a niche with no Reddit trace is a note on the card, and
   fabricating Reddit-flavored quotes to fill the section is the worst failure this
   skill can commit; (c) a page that redirects to a bot-toll or paywall (HTTP 402) is
   its own failure, not "try fetching again": skip straight to news quotes and YouTube
   comments.
2. **YouTube comments** under 3-5 channels they watch (from the founder's answers plus
   your own search).
3. **Anywhere else they gather**: forums, Facebook groups, review sites for products they
   already buy.

Collect, verbatim and with sources:

- **The pains**, in their exact words. Rank by engagement (likes, replies) when visible.
  These become the offer's fear list.
- **The outcome words**: what they call the result they want. These are the only words
  allowed on anything that sells.
- **The objection words**: what they say when they distrust a pitch in this market. The
  offer must answer these before they are voiced.

Rules for this pass, learned the hard way:

- **A search engine's summary is NOT a quote.** A quote only counts if you read it on the
  source page itself. Never paste a search result's paraphrase as "verbatim."
- **When a source will not open, walk the fallback ladder**: Reddit or forum blocked →
  niche communities that do open (Indie Hackers, founder blogs and newsletters, review
  sites) → news articles quoting real people in this market → competitors' testimonial
  pages (secondhand, and say so on the card).
- **When the buyer's real room is login-gated** (private Facebook groups, member forums),
  say so, and ask the founder to paste 5-10 real quotes from their own inbox, DMs, or
  group. The founder always has buyer language; the internet sometimes does not. And when
  no gated room exists either, say that plainly and move on; never invent a community to
  justify asking. Threshold: fewer than about five real quotes total, from all sources,
  means the card says "the market read is thin here" in plain words instead of building
  a confident pain list on air.
- Never invent a quote; keep the source next to every quote. If real buyer language truly
  cannot be found anywhere, say so plainly; a buyer who talks nowhere is itself a market
  warning.

## Pass 2 · The market read

Reason to state: "Whether this niche holds is a data question, and today the data is what
the market already shows."

Three questions, real numbers only; drop anything you cannot verify:

1. **Who sells to this buyer now?** First name the market's edge: a local business
   competes in its city or metro; everyone else, name the comparable market before
   searching. Then find the operators: ten is a floor, not a ceiling; list every real one
   found while it stays useful. For each, five columns: what they sell, the price,
   published price or call-closed, how they get found, and **the bundle**: exactly what
   the buyer receives (software? curriculum? live calls? community? human labor?), the
   one-time vs recurring split, and what the recurring fee buys. The bundle column is
   what the model decision (the scorecard reference) gets built from. Stopping rule: stop
   adding operators once three consecutive new ones repeat a bundle pattern already in
   the table. One check: if a "top firms" list was written by a firm on that list,
   confirm it against a source that was not.
2. **Growing or decaying?** Recent breakout content in the niche (views vs channel size),
   search interest direction, new entrants in the last year.
3. **Where is the empty seat?** The combination nobody occupies: a price point, a delivery
   model, a buyer segment, a promise. Two seats always get tested: (a) the founder's
   switching itch from step 0, question 5 (is that category actually open, or already a
   price war?), and (b) the transparency seat (when most operators hide their price behind
   a call, a published price IS an empty seat, and their opacity is the evidence). "No
   competition at all" is a warning, not a win: competitors selling is proof the money
   exists.

Output of step 2: one research note the founder can read in five minutes: the pain list,
the allowed words, the operator table, the direction call, the empty seat.
