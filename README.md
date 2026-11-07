### Luke Sargeant

I build trading systems, and the teams that build them. Right now I'm exploring what an engineering org looks like when agents do a real share of the work.

#### What I'm building / things I've built

- **An OTC spot FX venue.** API-first RFQ and firm streaming quotes over WebSockets, a single-writer matching core with an append-only ledger and audit tape, and pre-trade controls: credit caps, price collars, halt/resume and key rotation. A house market-maker quotes real rates so the book is never empty.
- **A margin dealer on top of it.** A double-entry ledger in integer minor units, margin with stop-out and negative-balance protection, OCO take-profit/stop-loss, and a daily financing run. Price feeds go through jump guards before anything trades on them.
- **A tamper-evident eval ledger for AI products.** Every run is hash-chained, so a test set can't quietly shrink: skipped cases count as failures and removals need a stated reason. *Show the denominator.*
- **Correction → test case → better model.** In a document-understanding app, every human correction becomes a test case and an LLM routine improves the reader against the growing corpus.

#### Teams

- [development-team-health-check](https://github.com/lukesargeant/development-team-health-check): the question deck I use to get teams talking candidly about how they really work.

London · Cloud, AWS, Java, Python, Rust, TypeScript, edge runtimes, Durable Objects · whatever language the problem needs
