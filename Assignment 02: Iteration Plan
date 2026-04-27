# Assignment 02: Iteration Plan

## 1. P01 Evaluation

My Project 01 prototype for Milly Maker Tracker’s simulator is in a much better place than I expected when I first started building it. The main simulator flow now feels solid. The site has a clear navigation bar, the simulator has separate tabs for Slates, Inputs, Settings, and Results, and the user can move through the tool without feeling lost. The design also landed much closer to the standard I wanted. The dark layout, blue simulator branding, compact slate table, team input tables, settings controls, simulation loading screen, and results table all feel connected to the Milly Maker Tracker brand.

The strongest part of P01 is the actual simulator experience. A user can choose a slate, inspect the game inputs, adjust settings, run simulations, and view results in a clean table. The Results tab is probably the most successful part of the prototype because it communicates useful DFS information right away. Players are sorted by Optimal Rate, and the table includes salary, ownership, optimal leverage, and Plus EV. The visual bar next to the numbers makes the results easier to scan. This matters because a DFS tool should not make users dig for the main takeaway.

The Inputs tab also works well because it makes the simulator feel transparent. Instead of hiding all assumptions, the page shows team level inputs and player level inputs. A user can see projections, ownership, salary, market share numbers, pace, rush rate, DST salary, and other variables. This helps the simulator feel less random and more connected to actual DFS research.

The biggest weakness is not the current NFL classic simulator. The bigger issue is scope. Right now, the simulator is built around football logic. That is fine for P01, but for the final MVP, I want Milly Maker Tracker to feel more expandable. The next step is adding another sport so the project shows it can grow past one NFL slate format. Another area needing improvement is user education. The simulator includes payout structure options, but I need to make the UI clearer about what those options actually affect. Payout structure should mostly change EV and grading, not the player Optimal Rate itself. If a user thinks changing payout structure should completely change Optimal Rate, the interface needs better wording.

Compared to my original proposal, I built the core idea I planned: a DFS simulator connected to Milly Maker Tracker. The project changed because I narrowed the scope while building. Early on, I had bigger ideas about every contest type and every sport, but I realized the better path was to make one simulator flow work well first. That decision helped the project become more polished. Instead of having several unfinished tools, I now have one strong simulator base with a clear next step.

## 2. Changes for P02

### Fixes

The first fix is to make sure the simulator results stay reliable after refreshes and new runs. The current behavior is much better now, but I still want to keep testing it so old results do not appear on a fresh visit or confuse the user after a new simulation.

The second fix is to clarify payout structure behavior. I need the Settings tab and Results tab to make it clear that payout structure affects grading, EV, and contest finish logic more than raw Optimal Rate. This matters because users should understand what each control is changing.

The third fix is continued live site testing. The simulator has worked locally and live, but I need to keep checking both environments before submission because a tool can look finished locally and still break once deployed.

### Improvements

I want to improve the Settings tab by adding short, direct helper text near the payout structure section. The text should explain Top Heavy, Standard, and Cash in DFS terms without making the page feel crowded.

I also want to improve the Results tab by keeping the strongest parts while reducing any confusion. The Optimal Rate view is already useful, but the Exposure and Graded tabs should feel equally clear. A user should know why each tab exists within a few seconds.

Another improvement is adding a clearer slate identity area. The page already shows week, operator, game type, number of games, and start time. I want to keep polishing this area so users always know exactly what slate they are running.

### Additions

The main addition for P02 will be another sport. I am leaning toward NBA because it is a natural next DFS sport and would show that the simulator framework can expand beyond NFL. NBA would require sport specific roster rules, player positions, salary logic, and a different input structure than football.

I also want to add sport aware data structures. The current simulator type system supports a general sport field, but the actual engine logic is still built around football. P02 should begin separating shared simulator logic from sport specific logic.

Another addition is better documentation for the simulator workflow. This does not need to be a long tutorial, but the final project should explain how a user moves from slate selection to settings to results.

### Cuts

I am cutting any attempt to support every DFS sport or every contest format in P02. That would make the project too wide and would lower the quality of the final MVP.

I am also cutting any major redesign of the simulator. The current design is working, so P02 should focus on expansion, clarity, and stability instead of tearing down the interface again.

I am cutting overly advanced payout modeling for now. A deeper contest payout engine could be valuable later, but for P02, the goal is to make the existing payout profiles clearer and more useful without overcomplicating the simulator.

## 3. Priority and Timeline

### Must complete

The first must complete item is stabilizing the current NFL simulator. This includes testing the Slates, Inputs, Settings, Results, Save, Reset, Run Sims, and Upload Projections flow on the live site. Estimated effort: a few hours of testing and cleanup.

The second must complete item is adding another sport at a basic MVP level. The new sport does not need every advanced feature on day one, but it should have a slate, inputs, settings, and results path. Estimated effort: most of a weekend, possibly longer depending on roster rules and data formatting.

The third must complete item is clarifying payout structure behavior in the UI. Users need to understand that payout structure mainly affects grading and EV, not the raw Optimal Rate calculation. Estimated effort: one to two hours.

### Should complete

I should complete a cleaner Results explanation for each tab. Optimal Rate, Exposure, and Graded should each have a clear purpose. Estimated effort: a few hours.

I should also improve the slate filtering and sport selection experience. Once another sport is added, the Slates tab needs to make switching between NFL and the new sport feel natural. Estimated effort: a few hours.

I should complete a simple documentation section or short explanation page for the simulator. This would help a first time user understand the tool without needing me to explain it. Estimated effort: one evening.

### If time allows

If time allows, I want to add a more polished comparison between NFL and the new sport. This could include a small note about how projections, salaries, positions, and roster construction change by sport. Estimated effort: a few hours.

If time allows, I would also improve the visual design of the loading screen and results states. The current loading screen already looks good, but small animation and copy improvements could make the tool feel more finished. Estimated effort: one to two hours.

If time allows, I may add more sample slates so the simulator does not feel limited to one test environment. Estimated effort: depends on data availability.

## 4. Updated Tools and Approach

I am not changing the main technology stack for P02. Astro, TypeScript, JSON slate packages, GitHub, and VS Code have been the right tools for this project. The current setup lets me build a live web app while still controlling the simulator data directly through files and API routes.

The most effective workflow during P01 was building in small passes, testing locally, committing changes, pushing to GitHub, and then checking the live site. This helped me catch differences between local behavior and deployed behavior. I also learned that simulator features need live testing because a tool can look correct in screenshots while still failing during a full run.

The JSON slate package approach was one of the better decisions. Having separate files for slate data, games, team inputs, player inputs, settings, and results made the simulator easier to reason through. For P02, I want to continue this structure, but I need to make it more sport aware so NFL logic does not control every future format.

If I were starting over, I would define sport specific simulator rules earlier. I spent a lot of time building around NFL, which made sense for P01, but adding another sport will require cleaner separation between shared simulator behavior and sport specific behavior. I would also document the purpose of each setting earlier, especially payout structure, so the interface explains itself better.

Overall, P01 gave me a working foundation. P02 should not be a rebuild. It should be a focused iteration: stabilize the current simulator, explain the confusing parts better, add another sport, and prove Milly Maker Tracker can grow into a broader DFS research platform.
