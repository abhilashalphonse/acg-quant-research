ACG Quant Research
Systematic market research · Quantitative strategy development · Evidence-first validation

ACG Quant Research is an independent research initiative focused on understanding market behavior, designing testable trading hypotheses, and evaluating whether those hypotheses survive realistic execution costs and out-of-sample scrutiny.

The project brings market-structure concepts—including breaks of structure (BOS), market structure shifts (MSS), fair value gaps (FVG), and liquidity behavior—into a reproducible quantitative workflow. Its objective is not to find a visually convincing setup, but to distinguish measurable, repeatable evidence from hindsight, overfitting, and execution assumptions.
Research status: Experimental. Historical analyses and frozen prospective protocols are included. No strategy in this repository should be interpreted as a verified live-trading edge, and this repository does not place broker orders.

Research philosophy
The core question is simple:

Can a precisely defined market hypothesis produce a measurable advantage after data limitations, execution assumptions, statistical uncertainty, and independent evaluation are accounted for?

We approach that question through a repeatable research cycle:
1. Observe — collect and validate historical or prospectively observed market data.
2. Specify — turn qualitative market ideas into unambiguous, timestamped rules.
3. Replay — test candidate signals and trade paths with explicit position, exit, and cost assumptions.
4. Freeze — version the strategy, dataset, analysis plan, and code before independent testing.
5. Observe prospectively — preserve first-seen evidence, timestamps, missing data, and revisions.
6. Evaluate — report outcomes, uncertainty, stress sensitivity, exposure, and failure cases.
7. Decide — retain, revise in a new version, or reject a hypothesis without rewriting its historical record.
Current research areas
Area	Research question	Current treatment
Market structure	Can BOS, MSS, FVG, and liquidity events be identified with consistent, non-anticipatory rules?	Historical detectors and exploratory replays
Entry timing	Does waiting for a defined post-BOS acceptance condition improve outcomes relative to immediate entry?	Frozen ACG-ACCEPT-01 comparison
Market state	Do prespecified price-path features add information beyond an acceptance-only baseline?	Frozen observational ACG-STATE-01 companion
Execution	How sensitive are results to spread, slippage, session exclusions, entry timing, and data gaps?	Explicit central/stress proxy assumptions
Trade-path and exits	How do stop placement, holding time, and exit policy influence realized R and risk exposure?	Ongoing research direction; not a demonstrated edge

Market data (Twelve Data proxy)
                |
                v
       OHLC validation / UTC alignment
                |
                v
    Historical datasets + first-seen ledger
                |
                v
       Frozen detectors and protocols
                |
        +-------+-------+
        |               |
        v               v
  ACCEPT-01         STATE-01
 Policy comparison  State observation
        |               |
        +-------+-------+
                |
                v
  Auditable outcomes, limitations,
  uncertainty and future decisions



  
