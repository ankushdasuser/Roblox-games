# What keeps players coming back: research notes for the idol sim

This doc covers four things:
- what research says about why people return to a game;
- what Roblox rewards in 2026;
- where "pull" turns into harm (or breaks the law);
- how each finding becomes a feature.

Most Roblox players are young, which raises the stakes on all four. The numbers behind these choices are in `economy-model.xlsx`.

## The short version

- **What brings players back for months is feeling skilled, free to choose and connected to others.** Compulsion without those three gets more hours but less enjoyment.
- **Roblox now judges a game on its first 28 days.** That covers play days, playing with friends, days with a purchase, and retention. Retention *is* growth.
- **Several small, well-studied effects stack up.** They are: head starts, visible near goals, real surprises, fresh starts, owning what you build, and ending sessions on a high.
- **Loot boxes are where pull turns harmful.** Research consistently links them to problem gambling. Brazil has banned paid loot boxes for minors since March 2026, and Roblox tightened its rules in May 2026.
- **Our line:** sell speed, convenience, looks and packs with honest odds. Never sell through deception or pressure.

## 1. What the research says, and what we build from it

| Finding | Evidence | What we build |
|---|---|---|
| **Need satisfaction creates the pull.** | Ryan, Rigby & Przybylski (2006): in four studies, feeling competent and free to choose predicted enjoyment and wanting to keep playing. In an online game, feeling connected to others also mattered. | **Skill:** clicking on the beat, readable boss patterns, numbers that visibly grow. **Choice:** skill-tree paths, picking your bias and fandom, picking each New Era's concept. **Connection:** fandoms, the co-op Album Drop, gifting, a luck bonus for each friend in the server. |
| **"Want to play" beats "have to play".** | Przybylski et al. (2009): when those needs went unmet, play became obsessive: more hours, more tension afterwards, less enjoyment. Heavy play hurt well-being mainly in obsessive players. | Design for players who leave happy and return tomorrow, not for the longest possible sessions. Roblox's algorithm counts play days alongside playtime. |
| **Habits come from repeating something in the same context.** | Lally et al. (2010): habits strengthened with daily repetition and levelled off after a median of 66 days (range 18–254). Missing one day did not set people back. | A daily anchor: a concert at the same time each day, plus the attendance calendar. Streaks *pause* instead of resetting, because a missed day doesn't break a habit and punishing it only adds pressure. |
| **Surprise beats predictability.** | Schultz, Dayan & Montague (1997): dopamine neurons respond to unexpected rewards. Once a reward is predictable, the response moves to the cue that predicts it. A missing expected reward causes a dip. | Reliable basics (attendance, quests) plus real surprises: Golden Notes, surprise concerts, Album Drops. Never promise a reward and then take it away. |
| **A head start raises completion.** | Nunes & Drèze (2006): car-wash cards with 2 of 10 stamps already filled were completed 34% of the time. Blank 8-stamp cards were completed 19% of the time. Both needed 8 more washes. | Binder sets start with two cards filled. The Comeback Pass starts at tier 2. The first daily quest is completed during the tutorial. |
| **Effort speeds up near a goal.** | Kivetz, Urminsky & Zheng (2006): coffee buyers bought more often the closer they got to a free coffee. | Always show the next near goal: the pity meter, "2 cards from a set bonus", the next upgrade. |
| **Fresh starts motivate.** | Dai, Milkman & Riis (2014): gym visits and goal commitments rise after markers like a new week or month. | Comebacks start on a Monday or on the 1st of the month. Idol birthdays act as markers. New Era is a personal fresh start. Returning players get a welcome-back bonus. |
| **People value what they build.** | Norton, Mochon & Ariely (2012), the IKEA effect. | Name your group, design your stage and dorm, choose your lineup. |
| **The ending shapes the memory.** | Kahneman et al. (1993): people rated a longer unpleasant experience as better when it ended less badly. | End each session with a recap ("3 new cards, Busking Street unlocked, 5 pulls to pity"), not on a wall. The recap is also a natural place to stop. |

## 2. What Roblox rewards (growth)

**Recommendations (Recommended For You, updated June 15, 2026).** Roblox now looks at a game's first 28 days, split into day 1, days 2–7 and days 8–28. It measures these signals for players who arrived from the Recommended For You row:
- playtime
- play days
- qualified play sessions
- intentional co-play days
- spend days (days with a purchase)
- Robux spent

The old qualified play-through rate is gone. It was replaced by play-through rate (how many people who see the game click into it) and first-play bounce (players who leave their first session early). For us, that means:
- **The first minute decides bounce.** Hype and the first Fever within 20 seconds, and the first pack within a minute (see the Pacing tab).
- **Play days need a reason to return each day.** That's the daily concert, attendance, offline earnings and idol birthdays.
- **Co-play days need features that work better with friends.** That's the friend luck bonus, the co-op Album Drop and fandom wars.
- **Spend days favour small, fair items people buy now and then over one giant bundle.** Don't chase this signal with daily pressure to buy.
- **Thumbnails and titles affect play-through rate.** Test them; Roblox is also testing personalized thumbnails.

**Creator Rewards (since July 2025).** Roblox pays you for engagement, on top of what players buy in your game:
- **Daily Engagement Rewards.** You get 5 Robux when an "Active Spender" plays your game for 10+ minutes in a day, as long as yours is one of the first three games they open that day. An Active Spender is someone who spent $9.99+ on Robux, Premium or subscriptions in the last 60 days. So be one of the first games kids open after school: a daily event at a consistent time helps.
- **Audience Expansion Rewards.** You get 35% of the first $100 of Robux purchases by players who are new to Roblox, or back after 60+ days away, during their first two months. It only counts if they arrived through a direct link to your game page or by searching your game's name, then played 10+ minutes. For returning players, yours must be the first game they play. So off-Roblox clips (Daesang reveals, dance emotes) should link straight to the game page.
- **Conditions.** Payouts are held for 60 days, and you need an average of 100 daily players. The Growth tab models both rewards.

**Rewarded video ads** came later. As of August 2025 they were only for games averaging 100K+ daily players, and only shown to users 13+. They aren't in the model yet.

## 3. Where pull becomes harm, and why we stay clear

- **Loot boxes and gambling.**
  - Drummond & Sauer (2018) found loot boxes share the structural and psychological features of gambling.
  - Zendle & Cairns (2018), a large survey, linked loot box spending to problem gambling severity.
  - A meta-analysis (Garea et al., 2021) found a small-to-moderate link: r ≈ 0.26 with problem gambling, or 0.37 after adjustment, and r ≈ 0.25 with excessive gaming. Which causes which is still unclear.
- **Predatory monetization** is defined by King & Delfabbro (2018) as systems that hide the long-term cost of play until players are financially and psychologically committed.
- **Near misses.** Clark et al. (2009) found near misses increase the urge to keep gambling and activate the brain's win circuitry. That's why we never fake one.
- **Dark patterns are expensive.** In 2022 Epic paid $245M in FTC refunds over design that led to unwanted purchases, plus a $275M children's privacy (COPPA) penalty.
- **The law and Roblox's rules.**
  - **Brazil:** the ECA Digital law (Law 15,211/2025) bans paid loot boxes in games minors are likely to play, effective March 17, 2026. Roblox blocked paid random items for Brazilian under-18s that day, and for unverified adults from March 31.
  - **Roblox rules (May 26, 2026):**
    - Odds are shown per outcome, as numbers that add up to 100%, before purchase.
    - Luck boosts and pity must show their effect as numbers, and the odds on screen must update while a boost is on.
    - Every outcome must give something.
    - Use `PolicyService` (`ArePaidRandomItemsRestricted`, and `IsPaidItemTradingAllowed` for trading) to give restricted players an alternative without randomness.
    - Declare paid random items in the maturity questionnaire.
    - Roblox names Australia, Belgium, the Netherlands, the UK and Brazil as regulated markets.

**What this changes in our design**
1. Packs bought with gems count as paid random items, because the gems were bought with Robux. The pack screen shows base odds, and switches to the boosted odds whenever Lucky, a potion or a Concert Boost is on. The Odds tab has both columns.
2. Every outcome gives something: the lowest card still gives Hype and fusion material.
3. Restricted players get the **Card Shop**, where they pick the exact card, plus packs earned through play. Their pack-related purchases are reduced on the Revenue tab.
4. The Debut Pack has fixed contents, so it can be sold everywhere.
5. Holo and Signed versions can be earned through fusion and events. The Odds tab flags any chase item that averages more than 10,000 Robux.

## 4. How the loops fit together

| Loop | What brings players back | Research behind it | Roblox signal it moves | What to track |
|---|---|---|---|---|
| First minute | Explosive first clicks, early Fever, a guaranteed (and labelled) Epic | Surprise; head start | First-play bounce | Onboarding funnel |
| Daily | Concert at a set time, attendance, 3 quests, offline earnings, birthdays | Habit; surprise | Play days; Daily Engagement Rewards | Economy events, session recap |
| Weekly | Fandom war final countdown, weekend Album Drop | Connection; near goals | Co-play days | PlayWithFriend |
| Every 3 weeks | Comeback: new zone, banner, Comeback Pass | Fresh start; head start | 28-day retention; returning players | ComebackJoin |
| Long term | Binder sets, New Era, fusion toward Signed | Skill; choice; ownership | Retention days 8–28 | Progression events |

## 5. Things we won't do

- Fake near misses, or odds that differ from what's shown.
- Fake countdowns or fake scarcity.
- Streaks that wipe progress after one missed day, or selling streak repairs.
- Offers aimed at players who've already spent a lot, or shop pop-ups during hype moments.
- Robux gambling, coin flips, case battles, or anything with cash value.
- Hiding prices behind a chain of currencies.

These hurt young players and break Roblox's rules or consumer law in places. They also come back as refunds, moderation and dislikes, all of which hurt discovery.

## Sources

- Ryan, Rigby & Przybylski (2006). The motivational pull of video games: A self-determination theory approach. *Motivation and Emotion*. https://doi.org/10.1007/s11031-006-9051-8
- Przybylski, Weinstein, Ryan & Rigby (2009). Having to versus wanting to play. *CyberPsychology & Behavior*. https://doi.org/10.1089/cpb.2009.0083
- Lally, van Jaarsveld, Potts & Wardle (2010). How are habits formed. *European Journal of Social Psychology*. https://doi.org/10.1002/ejsp.674
- Schultz, Dayan & Montague (1997). A neural substrate of prediction and reward. *Science*. https://doi.org/10.1126/science.275.5306.1593
- Nunes & Drèze (2006). The endowed progress effect. *Journal of Consumer Research*. https://doi.org/10.1086/500480
- Kivetz, Urminsky & Zheng (2006). The goal-gradient hypothesis resurrected. *Journal of Marketing Research*. https://doi.org/10.1509/jmkr.43.1.39
- Dai, Milkman & Riis (2014). The fresh start effect. *Management Science*. https://doi.org/10.1287/mnsc.2014.1901
- Norton, Mochon & Ariely (2012). The IKEA effect. *Journal of Consumer Psychology*. https://doi.org/10.1016/j.jcps.2011.08.002
- Kahneman, Fredrickson, Schreiber & Redelmeier (1993). When more pain is preferred to less. *Psychological Science*. https://doi.org/10.1111/j.1467-9280.1993.tb00589.x
- Drummond & Sauer (2018). Video game loot boxes are psychologically akin to gambling. *Nature Human Behaviour*. https://doi.org/10.1038/s41562-018-0360-1
- Zendle & Cairns (2018). Video game loot boxes are linked to problem gambling. *PLOS ONE*. https://doi.org/10.1371/journal.pone.0206767
- Garea et al. (2021). Meta-analysis of the relationship between problem gambling, excessive gaming and loot box spending. *International Gambling Studies*. https://doi.org/10.1080/14459795.2021.1914705
- King & Delfabbro (2018). Predatory monetization schemes in video games and internet gaming disorder. *Addiction*. https://doi.org/10.1111/add.14286
- Clark et al. (2009). Gambling near-misses enhance motivation to gamble. *Neuron*. https://doi.org/10.1016/j.neuron.2008.12.031
- FTC (2022). Fortnite video game maker Epic Games to pay more than half a billion dollars. https://www.ftc.gov/node/80135
- Banning loot boxes for minors: the case of Brazil (2026). *Journal of Behavioral Addictions*. https://www.akjournals.com/view/journals/2006/15/1/article-p5.xml
- Roblox DevForum (May 26, 2026). Clarifying requirements for paid random items. https://devforum.roblox.com/t/clarifying-requirements-for-paid-random-items/4654622
- Roblox DevForum (June 15, 2026). Recommended For You algorithm improvements that better value long-term retention. https://devforum.roblox.com/t/recommended-for-you-algorithm-improvements-that-better-value-long-term-retention/4684575
- Roblox DevForum (2025). Introducing Creator Rewards. https://devforum.roblox.com/t/introducing-creator-rewards-earn-more-by-growing-the-community/3777628
- Roblox DevForum (2025). More creators can now use rewarded video ads. https://devforum.roblox.com/t/more-creators-can-now-use-rewarded-video-ads/3838678
- Roblox Creator Docs. Earn on Roblox. https://create.roblox.com/docs/production/earn-on-roblox
- Roblox Creator Docs. AnalyticsService. https://create.roblox.com/docs/reference/engine/classes/AnalyticsService
