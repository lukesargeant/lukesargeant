### Luke Sargeant

I build trading systems, and the teams that build them. At the moment I'm working out what an engineering org looks like when agents do a real share of the work.

#### What I'm building / things I've built

- **An OTC spot FX venue.** API-first RFQ and firm streaming quotes over WebSockets, a single-writer matching core with an append-only ledger and audit tape, and pre-trade controls: credit caps, price collars, halt/resume and key rotation. A house market-maker quotes real rates so the book is never empty.
- **A margin dealer on top of it.** A double-entry ledger in integer minor units, margin with stop-out and negative-balance protection, OCO take-profit/stop-loss, and a daily financing run. Price feeds go through jump guards before anything trades on them.
- **A tamper-evident eval ledger for AI products.** Every run is hash-chained, so a test set can't quietly shrink: skipped cases count as failures and removals need a stated reason. *Show the denominator.*
- **Correction → test case → better model.** In a document-understanding app, every human correction becomes a test case and an LLM routine improves the reader against the growing corpus.

#### How I think about AI in engineering

- **Evals are the new tests.** An AI feature without a visible, honest pass rate is a demo.
- **Agents go through the same gates as engineers.** On my own systems, agents open PRs, review code, triage incidents and roll back bad deploys. All of that runs through CI, an approval inbox, an audit log and a kill switch.
- **In regulated domains, audit is the architecture.** Append-only logs, hash chains and a human in the loop where the risk is. That's what lets AI move fast somewhere a mistake costs money.
- **Transformation is a product problem, not a mandate.** Time as a chief of staff taught me that change sticks when it's tied to outcomes the business already measures, and when it's measured honestly.

#### Teams

- [development-team-health-check](https://github.com/lukesargeant/development-team-health-check): the question deck I use to get teams talking candidly about how they really work.

London · Cloud, AWS, Java, Python, Rust, TypeScript, edge runtimes, Durable Objects · whatever language the problem needs
