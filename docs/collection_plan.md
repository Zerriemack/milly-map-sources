# Module 3: Collection Plan + Initial Sources

## 1. Topic statement for Milly Map

I am building Milly Map as a curated, organized reference system for winning large field NFL DraftKings tournaments, with a main focus on Showdown Milly Maker and an expansion path toward Classic Milly Maker. The end goal is a repeatable process that starts with contest rules and roster construction constraints, moves through slate and game environment research, then connects to lineup building rules that can be tested and improved over time.

This topic matters to my current work because I already track winning Showdown lineups and patterns, and I am building tools that shrink my player pool and enforce stricter lineup rules. Milly Map will serve as the one place where my sources live, where my definitions stay consistent, and where every claim can be tied to a rule page, a research paper, a tool output, or a real contest result. I will avoid pick driven content and focus on sources that improve decision making, repeatability, and proof.

## 2. Proposed organizational structure

I will organize Milly Map using the same category logic in the Sources Roadmap document, then narrow each category to NFL DraftKings Milly Maker work.

### Category A. Primary data for analysis
Purpose: Build from evidence.  
Contents: My lineup tracking dataset, exported contest results, and any structured datasets I can query.

### Category B. Contest rules and platform mechanics
Purpose: Keep every strategy aligned with the actual game.  
Contents: DraftKings rules, scoring, roster requirements, late swap rules, entry limits, and payout structure notes.

### Category C. Tools used to test and execute
Purpose: Turn ideas into repeatable builds.  
Contents: Simulation tools, optimizers, lineup builders, and settings documentation.

### Category D. Research and academic work
Purpose: Use formal models where they help, and translate them into usable rules.  
Contents: Optimization, opponent modeling, duplication risk, ownership modeling, and portfolio concepts.

### Category E. Expert process content
Purpose: Capture process thinking that improves slate reading and constraint design.  
Contents: Analysts who explain assumptions, game environments, and decision logic.

### Category F. Community discovery
Purpose: Find new angles and compare approaches without treating it as truth.  
Contents: Discussion threads, disagreements, and examples, plus notes on what needs validation.

### Category G. My rules, notes, and evolving framework
Purpose: Store my own conclusions, backtests, and updates.  
Contents: My final lineup rules, version history, and what changed and why.

## 3. Initial sources list with annotations (seven)

The goal is five to seven initial sources. Each entry below includes an annotation and a short note on where it fits in the plan.

### Source 1. DraftKings NFL rules and scoring
Links:  
https://help.draftkings.com/hc/en-us/articles/4405233935123-NFL  
https://help.draftkings.com/hc/en-us/articles/4405231687571-NFL-Scoring  

Annotation: DraftKings NFL rules and scoring pages define the contest format and the exact scoring events that drive lineup value. This includes roster requirements, salary cap mechanics, position rules for Classic and Showdown, and the points that come from yardage, touchdowns, bonuses, and defense scoring. This is the ground truth for Milly Map. If a strategy ignores these constraints, it is not a real strategy. I will record the date accessed and update notes if DraftKings changes any definitions.

Fits in: Category B

### Source 2. Personal Showdown Milly Maker winner dataset (unpublished)
Location: Local Excel tracker of 213 Showdown Milly Maker winning lineups

Annotation: My self collected dataset tracks winning lineups for 213 NFL Showdown Milly Maker contests. I tag each slate by year, teams, captain position, roster construction traits, and patterns I can measure. This becomes my baseline evidence for what wins under real field behavior, not what people claim should win. I use it to validate ideas from tools and analysts, then update lineup rules using proof. The limitation is that it is Showdown focused and it is manually collected, so I will audit entries and expand the tracker.

Fits in: Category A

### Source 3. FantasyCruncher contest links
Link: https://www.fantasycruncher.com/contest-links/NFL

Annotation: FantasyCruncher contest links help me pull contest context and compare slates. It can show contest types, prize pools, entry fees, field size, and other details that matter when I am studying lineup construction patterns. It supports my research workflow because I can match analysis to a specific contest structure instead of mixing different slates and formats. I will treat it as a helpful reference, then cross check against DraftKings contest information when accuracy matters because third party pages can change or omit details.

Fits in: Category B, with supporting value for Category A

### Source 4. Run The Sims, SimRunner
Link: https://www.runthesims.com/

Annotation: Run The Sims SimRunner lets me simulate outcomes and test lineup constructions across many game scripts. This matters for large field tournaments because results are driven by variance and by how the slate breaks. Simulation outputs help me stress test assumptions about stacking, leverage, and ownership without relying on one set of projections or one storyline. It also connects to my core concept of committing to one or more key outcomes and building around them across entries. I will record sim settings and assumptions because outputs depend on inputs.

Fits in: Category C

### Source 5. Hunter, Vielma, and Zaman, “Picking Winners in Daily Fantasy Sports Using Integer Programming”
Link: https://arxiv.org/abs/1604.01455

Annotation: This paper treats lineup building as an optimization problem. It uses integer programming to build lineups under constraints and discusses ways to represent stacking, overlap limits, and correlation. It supports my approach because it gives academic language for what I already do in practice, which is enforce rules through constraints instead of building lineups by feel. It also supports a repeatable method, since constraints can be documented and rerun. The limitation is that NFL specific translation requires care and contest ecosystems change, so I will focus on the modeling ideas.

Fits in: Category D

### Source 6. Mlcoch and Hubacek, “Competing in Daily Fantasy Sports Using Generative Models”
File: Competing in daily fantasy sports using generative models.pdf

Annotation: This paper models DFS as a competitive environment where opponents matter. It uses generative models to create realistic opponent lineups and evaluates strategies against simulated fields. This lines up with my focus on beating large fields, because it treats the field as part of the problem and not as background noise. It gives language for ownership, duplication risk, and portfolio performance across many entries. The limitation is that modeling choices and tuning decisions shape results, so I will use it as a framework and validate ideas using my own contest data.

Fits in: Category D

### Source 7. Kyle Krims, The Sauce Network, matchup breakdown video
Link: https://youtu.be/aNvc_IeTPog?si=P4KeSKN3R82WmTzf

Annotation: Kyle Krims does team by team breakdowns and turns football context into actionable angles. He explains assumptions about game environment, injuries, coaching tendencies, and how information changes decision making. Even when the target is betting, the process maps to DFS because it affects projection ranges, stacking decisions, and late news adjustments. This supports the mental side of my workflow, which is committing to a strong read and building around it. I will treat this as process education and validate any claim with data.

Fits in: Category E

## 4. Tool choice for collecting and organizing sources

Tool selected: GitHub Pages

Reason: I already use GitHub in my workflow, so GitHub Pages keeps everything versioned and easy to update. It supports folders and markdown pages, so my sources can live in a clear hierarchy instead of scattered notes. It also produces a public link that is easy to submit, and it creates a simple path for future expansion when I add Classic Milly Maker sources.

## 5. Metadata plan

I will use a consistent template at the top of every source page so each entry is easy to scan and compare.

Fields included on every source page:
- Category (A through G)
- Contest type (Showdown, Classic)
- Use stage (Rules, Research, Build, Review)
- Concepts (ownership, stacking, correlation, duplication, leverage, bankroll, late news)
- Reliability tag (Official, Peer reviewed, Tool output, Expert process, Community)
- Date accessed
