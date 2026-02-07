## Academic Research

### Picking Winners in Daily Fantasy Sports Using Integer Programming (arXiv)

[Picking Winners in Daily Fantasy Sports Using Integer Programming (arXiv)](https://arxiv.org/abs/1604.01455)

Discovery method: Targeted search for operations research papers on DFS portfolio construction.

What it covers: This paper models top heavy DFS contests as a portfolio selection problem and shows how to build multiple lineups using integer programming with controls for variance and correlation.
Why it is valuable: It gives a clear framework for generating many entries with purpose instead of building random variations. The emphasis on diversification matches how large field tournaments reward unique paths to first place.
Who would find it useful: DFS players building multi entry portfolios, analysts studying lineup construction, and anyone translating payout structure into lineup generation rules.
Limitations: The math is dense and the examples focus on sports other than NFL, so adapting the methods requires extra interpretation and additional assumptions.

### Competing in Daily Fantasy Sports Using Generative Models (Wiley)

[Competing in Daily Fantasy Sports Using Generative Models (Wiley)](https://onlinelibrary.wiley.com/doi/10.1111/itor.13344)

Discovery method: Citation chasing from DFS optimization research and related work sections.

What it covers: This paper estimates fantasy point distributions using generative models, then uses optimization to build lineups while accounting for variance and covariance to match top heavy payouts.
Why it is valuable: It connects simulation style thinking to lineup construction and makes the risk and correlation logic explicit instead of relying on informal stacking rules.
Who would find it useful: DFS players who simulate outcomes, researchers building probabilistic projections, and anyone designing portfolio style lineup generation.
Limitations: The evaluation is on a different sport and contest environment, so direct transfer to DraftKings NFL needs careful testing and sport specific modeling choices.
## DFL-Opt: A Daily Fantasy Lineup Optimizer

[DFL-Opt: A Daily Fantasy Lineup Optimizer (Montclair Digital Commons)](https://digitalcommons.montclair.edu/etd/677/)

Discovery method: Targeted search for DFS lineup optimization papers using linear programming and portfolio style contest logic.

What it covers: This project describes DFL-Opt, a lineup optimizer built around linear programming to generate DFS lineups under roster and salary constraints. It explains how the optimizer handles lineup construction rules and reports a small real contest test in DraftKings Showdown Captain Mode during a short window in 2020. Why it is valuable: It connects DFS lineup building to a repeatable optimization method and shows how lineup generation can be treated as an engineering problem instead of guesswork. Who would find it useful: DFS players who want a reproducible process, plus students interested in optimization applied to sports contests. Limitations: The evaluation window is narrow and results depend on input assumptions, so it should be treated as a starting point and paired with broader testing and better projection inputs.
