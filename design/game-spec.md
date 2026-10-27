# Daesang! Idol Agency: product spec

**Status:** Draft · **Owner:** solo developer · **Date:** 2026-10-27 · **Platform:** Roblox, designed for phones first
**Scope:** v1 launch in full detail; Comeback 1 and 2 at a lighter level of detail. "Daesang! Idol Agency" is a working title (see Open Questions).
**Related:** `design/economy-model.xlsx` (every number below comes from it) · `design/engagement-research.md` (why each feature exists)

---

## TL;DR

You run an idol agency. Click on the beat to "stream" your group's songs and earn **Hype**. Pull **photocards** to sign idols, fill your **binder**, beat **Noise monsters** in stage battles, and unlock bigger venues, from a practice room up to a world tour.

- **Monetization:** speed, convenience, looks, and packs with honest odds. Free players can reach everything.
- **Retention:** daily reasons to return, a new **comeback** every 3 weeks, and friends.

**What makes it different:** K-pop fandom already works like a gacha game (random photocards, pulling for your favorite member, comebacks, fan clubs). The theme and the monetization are the same thing, not one bolted onto the other.

---

## 1. Problem statement

K-pop and anime fans on Roblox mostly get dress-up games and clones. None of them capture how fandom actually feels: collecting photocards, having a "bias" (favorite member), getting hyped for comebacks, and competing as a fandom. The big Roblox collection and RNG games show the genre can hold players for months. None of them are built around fandom, and many are built on monetization that now breaks Roblox's rules.

The developer's problem: build, alone, a game that keeps players for 28+ days, which is what Roblox's recommendations now reward. It also has to earn money fairly under the paid-random-item rules of **May 26, 2026** and Brazil's ban on loot boxes for minors. If retention isn't solved, discovery dies. If monetization isn't compliant, the game faces takedowns and refunds.

**Evidence so far:** all modelled, nothing measured yet. The model's placeholder retention (25% / 8% / 3% on days 1 / 7 / 30) gives about **$0.078 per new player over 30 days** and **$0.14 over 26 weeks**. About **two-thirds of 30-day revenue arrives after day 7**, so retention matters more than first-session offers. A closed test has to confirm these numbers.

---

## 2. Goals

| # | Goal | Type | Success | Stretch |
|---|---|---|---|---|
| G1 | New players are hooked within the first session | Player | Day-1 retention ≥ 25%; first-play bounce better than the benchmark median in Creator Analytics | D1 ≥ 30%; top quartile |
| G2 | Players build a daily habit | Player | D7 ≥ 8%, D30 ≥ 3%; players still active in week 2 play ≥ 3 days a week | D7 ≥ 10%, D30 ≥ 4% |
| G3 | Fair monetization pays | Business | ≥ $0.078 per new player in 30 days, **and** ≥ 50% of engaged free players reach pity within a comeback | ≥ $0.10 per new player |
| G4 | The game earns its way into recommendations | Business | 100+ average daily players by day 60 (the Audience Expansion Rewards threshold) | 500+ |
| G5 | Fully compliant and trusted | Both | 0 policy strikes; every odds audit passes; like ratio ≥ 85% | Like ratio ≥ 90% |

## 3. Non-goals (v1)

1. **No real K-pop IP**: no real idols, songs, choreography or logos. DMCA takedowns end Roblox games. Everything is original.
2. **No real-time sword and gun combat at launch.** Too big for one developer. Battles are auto-battles with tap-to-boost; a real-time boss mode is P2.
3. **No trading at launch.** A duplication bug or scam wave can destroy the economy, and trading paid items needs extra policy checks. P2, once the economy is stable.
4. **No Robux wagering or casino minigames, ever.** Banned on Roblox and harmful to a young audience.
5. **No rewarded video ads.** Only games averaging 100K+ daily players qualify. Revisit if we get there.

---

## 4. Players

| Persona | Who | Wants | Spends |
|---|---|---|---|
| **The Fan** | 10–14, plays on a phone after school | Their bias's rare card; a binder to show friends | Mostly free; the Debut Pack, maybe one pass |
| **The Grinder** | 12–16, simulator veteran | Numbers going up, rebirths, leaderboards | Auto-Stream, 2x Hype |
| **The Collector** | 14–17 with their own money | Daesang and Signed cards, showing off in the hub | Gem bundles, Lucky, VIP |
| **The Squad** | A friend group playing together | Co-op events, fandom wars | Gifts, Concert Boosts |
| **The Returner** | Away for 60+ days | A fresh start in a comeback | Comeback Pass |
| **Restricted player** | UK or Brazil under-18, and other regulated markets | The full game without paid randomness | Card Shop, passes, cosmetics |
| **The Parent** (secondary) | Pays or approves spending | Clear prices, no tricks | — |

---

## 5. The game on one page

- **Core loop (seconds):** tap on the beat → Hype → combo → **Killing Part** fever (2x for 10 seconds, the song jumps to its chorus, the stage lights up).
- **Session loop (minutes):** clear a stage → drops → open a pack → equip a squad of 3 → next stage or zone.
- **Daily loop:** 28-day attendance calendar, 3 daily quests, the **Daily Encore** at the same time every day, offline concerts, an end-of-day recap.
- **Long-term loop:** binder sets with permanent bonuses, fusion (5 copies → Holo, 5 Holos → Signed), and from v1.2, a skill tree and **New Era** rebirth.
- **Live loop:** a comeback every 3 weeks with a new zone, a limited banner, an event shop and a Comeback Pass.

**Launch content:**
- 12 idols in two original groups of 6.
- 60 cards (12 idols × 5 tiers: Trainee, Rookie, Idol, Center, Daesang).
- 7 zones with 7 bosses.
- 2 original songs plus a hub track.
- 8 gamepasses and 6 gem bundles.

---

## 6. User stories

**The Fan**
1. As a new player, I want something exciting to happen within seconds of my first tap, so that I want to keep playing.
2. As a fan, I want to pick my bias and build my binder around them, so that the collection feels like mine.
3. As a fan, I want to see exactly which cards I'm missing and how close a set is to complete, so that I know what to aim for.
4. As a free player, I want to be able to reach the banner's guaranteed rare card by playing, so that not paying doesn't lock me out.
5. As a player who missed a day, I want my attendance streak to pause instead of resetting, so that one missed day doesn't erase my progress.

**The Grinder**
1. As a grinder, I want a steady stream of upgrades early and bigger goals later, so that progress feels fast first and meaningful after.
2. As a grinder, I want an optional auto-clicker, so that I can progress without tapping for hours.
3. As a grinder, I want hand-clicking on the beat to still beat auto-clicking during fever, so that skill matters.

**The Collector**
1. As a collector, I want to see every card's exact odds (including with my luck boost on) before I buy, so that I know what I'm paying for.
2. As a collector, I want rare pulls to get a big reveal and a server announcement, so that rare cards feel special and others see them.
3. As a collector, I want duplicates to count toward something, so that no pull is wasted.

**The Squad**
1. As a friend group, I want a bonus for playing in the same server, so that playing together pays off.
2. As a friend, I want to send a gift to a friend, so that I can share the fun. (P1)

**Restricted player**
1. As a player in a restricted region, I want to get the cards I want without random packs, so that I can play the full game legally.

**The Parent**
1. As a parent, I want every price shown in Robux and every pack's odds shown before purchase, so that I can trust what my child is buying.

**Edge cases**
1. As a player whose Robux purchase failed or was interrupted, I want to be charged only if I receive the item, and to receive it exactly once.
2. As a player on a low-end phone, I want a Reduce Effects option, so that the game runs smoothly and doesn't overwhelm me.
3. As a player who leaves mid-session, I want my progress saved, so that nothing is lost.

---

## 7. Requirements

### P0: Launch (v1). The game doesn't ship without these.

**R1. Streaming and Killing Part (core loop)**
- [ ] Every tap adds Hype (Hype per click × multipliers) and shows a number pop where the player tapped.
- [ ] Taps within the beat window (default ±120 ms, configurable) build the combo. Off-beat taps still earn base Hype.
- [ ] A full combo (default 16 on-beat taps) triggers **Killing Part**: 2x Hype for 10 seconds, the song jumps to its chorus, and the stage effects follow the "hype bursts" feel spec.
- [ ] In the tutorial, Killing Part triggers within 20 seconds of the first tap (wider beat window).
- [ ] A **Golden Note** appears about once per 500 taps. Catching it starts a 5-second mini-fever.
- [ ] Auto-Stream (a gamepass) earns at 1.25x the manual rate but **does not** build the combo, so only on-beat taps trigger fever.
- [ ] Runs at 60 fps on mid-range phones during fever.

**R2. Upgrades, zones and walls (pacing)**
- [ ] Costs, cost growth, zone boosts and walls come from config, using the values on the model's Pacing tab: first upgrade 12 Hype, +10% Hype per upgrade, zone growth 1.18–1.30.
- [ ] Launch has 7 zones: Practice Room → Busking Street → Showcase Hall → Music Show Stage → Fan Meeting Hall → Concert Hall → Arena.
- [ ] In playtests, free players arrive within ±25% of the model's times: Busking Street ~6 min; the Showcase Hall wall starts ~12 min and takes ~8 min to grind; Music Show Stage ~38 min; Fan Meeting Hall about day 3; Arena about day 10 (at 45 min/day).
- [ ] The wall screen shows a progress bar and an estimated time to unlock.
- [ ] No energy or stamina system. Play time is never capped.

**R3. Idols, cards and squad**
- [ ] 12 idols; each has 1 card per tier (60 cards). Cards give Hype and boss stats.
- [ ] Squad of 3 slots. A 4th slot comes from the +1 Squad Slot pass **or is unlocked free at a set account level**, so power can always be earned.
- [ ] The player picks a bias at onboarding and can change it later. Having your bias in the squad gives +10% Hype. **Choosing a bias never changes pull odds.**

**R4. Packs, odds and pity (paid random items)**
- [ ] Given the player isn't restricted, when they open the pack screen, they see **every possible item (card and version) with its odds as a percentage**, adding up to 100% (exact values available on tap), plus the pity status (e.g. "Center or better by pull 60: 37/60"). All of this shows before any purchase.
- [ ] Base odds: Trainee 60%, Rookie 28%, Idol 9%, Center 2.5%, Daesang 0.5%. Within a tier, odds are split evenly across cards. Holo 5% and Signed 0.5% are rolled separately on every pull.
- [ ] Given a luck boost is active (Lucky pass or potion), the displayed odds **switch to the boosted odds** (Idol/Center/Daesang ×1.5, Trainee takes the remainder) and show the boost's remaining time.
- [ ] Pity: if pulls 1–59 had no Center or better, pull 60 is guaranteed Center or better. The counter is always visible and resets on any Center or better.
- [ ] A 10-pull guarantees at least one Rookie. Every outcome gives a card plus fusion progress. There are no empty results.
- [ ] Reveal animations are tiered by rarity, and **the glow always matches the real rarity** (no fake near misses). Trainee and Rookie can be skipped. Center and above are announced to the server.
- [ ] Every gem price also shows its approximate Robux value.
- [ ] The rolls and the odds screen read from **the same config table**, so the shown odds can't drift from the real ones.
- [ ] QA audit: in 100,000 simulated pulls, each rarity's count is within 3 standard deviations of expected.

**R5. Non-random path (required for restricted players, available to everyone)**
- [ ] `PolicyService:GetPolicyInfoForPlayerAsync` is checked on join. If `ArePaidRandomItemsRestricted` is true, **or the call fails**, gem-bought packs are hidden and can't be bought.
- [ ] **Card Shop:** a rotating set of 6 cards a day, each sold at a fixed price in Robux (about 299) or gems. Open to everyone.
- [ ] **Pack Tickets** are earn-only (attendance, achievements), can never be bought, and are not sped up by any purchase. For restricted players they become **Selector Tickets**: pick a card from a list, with no randomness. This conservative default stays until OQ1 is answered.

**R6. Binder, sets and fusion**
- [ ] The binder shows every card. Missing ones appear as silhouettes, with a count per set (e.g. 8/12).
- [ ] The first set starts with 2 cards already in it, labelled as a "Debut gift".
- [ ] Completing a set gives a permanent bonus. The bonus is shown before completion, e.g. "2 cards to go: +5% Hype forever".
- [ ] Fusion: 5 copies → Holo of that card; 5 Holos → Signed. A preview and a confirm step come before fusing. Fusing an equipped card asks for confirmation.

**R7. Bosses and stages**
- [ ] One boss per zone. The squad auto-attacks; on-beat taps add critical hits.
- [ ] At 20% boss health the finale starts: the remix plays, the action freezes briefly on the hit, then loot bursts out.
- [ ] Playtests show at least 95% of new players beat the first boss on their first try.
- [ ] Losing costs nothing. The loss screen suggests an upgrade or card that would help. Only at the first wall, it also shows the one-time Debut Pack offer.
- [ ] Gem drops count toward the daily farming cap (120).

**R8. First-time experience**
- [ ] By 20 seconds: a big Hype pop and the tutorial Killing Part.
- [ ] By 60 seconds: a free starter pack, **labelled "Guaranteed Epic"**. The player names their group (filtered with `TextService`) and picks a bias.
- [ ] By 5 minutes: first boss beaten. ~6 min: Busking Street. ~12 min: Showcase Hall wall, where the Debut Pack is offered once.
- [ ] No shop pop-ups before the first wall; after that, at most one offer pop-up per session.
- [ ] Every step logs an onboarding funnel event.

**R9. Daily loop**
- [ ] A 28-day attendance calendar with all rewards previewed; big rewards on days 7 and 28. **A missed day pauses the streak; it never resets it.**
- [ ] 3 daily quests. On day 1, the first quest is completed during the tutorial.
- [ ] **Daily Encore:** a bonus stage open in the same daily window (default 3–9 pm, player's local time), giving gems and Hype. Outside the window it shows a countdown.
- [ ] Offline concerts: the player earns a share of their Hype rate while away, up to 8 hours (24 hours with the pass). It's shown on return: "Your idols performed while you were away".
- [ ] When the last daily quest is done, show a recap: today's highlights, tomorrow's reward, and a clear "good place to stop".

**R10. Currencies**
- [ ] **Hype** (soft currency); **Gems** (premium: bought, or earned at about 310 a day, of which at most 120 can come from stage drops); **Pack and Selector Tickets** (earn-only).
- [ ] The server is the authority on every balance; the client can never grant currency. Every change is logged with `LogEconomyEvent`.

**R11. Store**
- [ ] Gamepasses: Auto-Stream 199, 2x Hype 149, 3x Open 249, 8x Open 799, Lucky 349, +1 Squad Slot 299, VIP 499, Offline 24h 149.
- [ ] Gem bundles: 99 / 249 / 499 / 999 / 2,499 / 4,999 Robux, with 0–30% bonus gems. The first purchase of each size gives double gems, clearly labelled.
- [ ] **Debut Pack:** 99 Robux, **fixed contents listed up front**, once per account.
- [ ] Luck potion: 49 Robux for 15 minutes, with boosted odds shown while it's active.
- [ ] Receipts are idempotent: the item is granted and saved **before** `PurchaseGranted` is returned, is never granted twice, and every receipt is logged.
- [ ] No purchase prompts during Killing Part, pack reveals or boss finales.

**R12. Social basics**
- [ ] Center-and-above pulls are announced to the server.
- [ ] The hub showcase stage shows each player's top 3 idols performing.
- [ ] Friend bonus: +10% Hype per friend in the server, up to +30%. **It's Hype, not luck, so it doesn't change odds.**
- [ ] Codes (set in config) are released at like-count milestones; joining the Roblox group gives a one-time reward.

**R13. Feel and safety settings**
- [ ] Bursts follow the feel spec: build-up → peak → release.
- [ ] Large flashes no more than 3 per second, and no saturated red full-screen flashes.
- [ ] A Reduce Effects toggle turns off screen shake and flashes and cuts particles.
- [ ] Separate music and sound-effect volume, with no sudden loud peaks.

**R14. Analytics**
- [ ] Every event on the model's Tracking tab is implemented, and each one carries "days since first join".

**R15. Live-ops config and data safety**
- [ ] All tunable values (costs, odds, rewards, prices, schedules, codes) live in config modules, so changes need no code edits.
- [ ] Player data is saved with session locking (e.g. ProfileStore), autosave, and a save on shutdown (`BindToClose`). Nothing is lost when a server closes.
- [ ] Admin commands can start live events and grant compensation.

### P1: Comeback 1 (v1.1, launch + 3 weeks) and Comeback 2 (v1.2, launch + 6 weeks)

**v1.1 (Comeback 1)**
- **R16. Comeback system:**
  - A teaser week, then a new zone (Stadium).
  - A limited banner whose per-card odds are shown.
  - Event tokens and an event shop.
  - A **Comeback Pass** with a free track and a premium track (399 Robux) that starts at tier 2, plus tier skips at 99 Robux.
  - Comebacks start on a Monday or on the 1st of the month.
- **R17. Concert Boost:** 99 Robux. Gives the whole server 1.5x luck for 15 minutes and announces the buyer. The odds screen updates for everyone in the server.
- **R18. Fandoms and the weekly fandom war:** a leaderboard per fandom, with a final 60-second countdown and a "music show win".
- **R19. Idol birthdays:** that idol's rate goes up (shown as numbers), and everyone gets a free birthday card for logging in.
- **R20. Live server events:** Surprise Live Concert (cards and gems rain down), Album Drop (co-op), Lightstick Ocean (a goal for the whole server), and Fan Stampede.
- **R21. Gifting:** buy any pass or pack for a friend.

**v1.2 (Comeback 2)**
- **R22. Skill tree:** Vocal (damage), Dance (speed), Rap (area damage) and Visual (Hype). Points are earned only; instant respec can be bought.
- **R23. Weapons:** lightstick blades, mic blasters and speaker cannons as boss gear, with cosmetic skins.
- **R24. New Era rebirth:** reset for a permanent multiplier and pick a concept (dark, cute, girl crush), each with its own look. Plus a new zone (World Tour).
- **R25. Variety-show captions** and the extra feel items from the "hype bursts" spec.

### P2: later. Design for these now; don't build them yet.

- **Fan Club subscription:** daily gems and a monthly cosmetic. Payout share needs checking (OQ7).
- **Trading:** behind `IsPaidItemTradingAllowed`, with duplication protection and logging. Store item IDs so trades can be audited later.
- **Real-time boss mode with swords and guns:** keep combat stats separate from auto-battle, so a real-time mode can reuse them.
- **Dorm and stage customization:** the "people value what they build" effect.
- **Rewarded video ads:** only if we pass 100K average daily players.
- **Localization:** Portuguese and Spanish first. Brazil is big, but most players there are under 18 and need the non-random path.

---

## 8. Monetization and economy

**Principle:** sell **speed, convenience, looks and packs with honest odds**. Never sell power that free players can't reach, and never sell through pressure.

| Product | Price (Robux) | First offered | Notes |
|---|---|---|---|
| Debut Pack | 99 | First wall | Fixed contents, once per account |
| Auto-Stream / 2x Hype / Offline 24h | 199 / 149 / 149 | Day 1 | Speed |
| 3x Open / 8x Open / Lucky | 249 / 799 / 349 | Day 1 / Day 7 / Day 7 | Pack-related (restricted where required) |
| +1 Squad Slot / VIP | 299 / 499 | Day 7 | Slot can also be earned |
| Gem bundles | 99–4,999 | Day 1 | 0–30% bonus; first purchase doubles |
| Luck potion | 49 | Day 1 | Boosted odds shown |
| Card Shop | ~299 per card (or gems) | Day 1 | No randomness |
| Concert Boost · Comeback Pass · Gifts · Cosmetics | 99 · 399 · ~199 · ~149 | v1.1 | |

**Key numbers:**
- Free players earn about 3.1 pulls a day and reach pity in about **19 days**, inside a 21-day comeback.
- On average it takes **28 pulls** (about 1,164 Robux) to get a Center or better.
- Holo and Signed versions are mainly earned through fusion, because pulling them would average more than 10,000 Robux.

---

## 9. Compliance and player safety (cross-cutting, P0)

- **Roblox paid-random-item rules (May 26, 2026):**
  - Odds shown for every item, as numbers adding up to 100%, before purchase.
  - Boost and pity effects shown as numbers, and the displayed odds update while a boost is active.
  - Every outcome gives something.
  - `PolicyService` used to gate players, with an alternative for restricted ones.
  - Declared in the maturity questionnaire.
- **Regulated markets** (Australia, Belgium, the Netherlands, the UK, Brazil): handled by R5. Brazil's ECA Digital law has applied since March 17, 2026.
- **Things we won't do:**
  - Fake near misses, or odds that differ from what's shown.
  - Fake countdowns or fake scarcity.
  - Streaks that reset after one missed day.
  - Offers aimed at players who've already spent a lot.
  - Shop pop-ups during hype moments.
  - Robux wagering.
  - Hiding prices behind chains of currencies.
- **Text and safety:** filter all player-entered text with `TextService`. Follow seizure-safe flash limits and offer Reduce Effects.

---

## 10. Success metrics

| Metric | Success | Stretch | Source | Check at |
|---|---|---|---|---|
| **Leading** | | | | |
| First-play bounce | Better than the benchmark median | Top quartile | Creator Analytics: Home recommendations | Week 1 |
| Onboarding funnel: first pack / first boss win / Busking Street / first wall | 85% / 60% / 45% / 35% | 90 / 70 / 55 / 45% | `LogOnboardingFunnelStepEvent` | Week 1 |
| D1 retention | 25% | 30% | Creator Analytics | Week 1 |
| Zone arrival times vs. the model | Within ±25% | Within ±10% | `LogProgressionCompleteEvent` | Week 1 |
| Odds audit (live pulls vs. posted odds) | Pass (within 3 standard deviations) | — | Custom event "PackOpened" | Weekly |
| **Lagging** | | | | |
| D7 / D30 retention | 8% / 3% | 10% / 4% | Creator Analytics | Days 30 / 60 |
| Play days per week (players active in week 2+) | ≥ 3 | ≥ 4 | Custom events | Day 30 |
| Revenue per new player, first 30 days | $0.078 | $0.10 | Monetization analytics + model | Day 30 |
| Share of 30-day revenue arriving after day 7 | ≥ 60% | ≥ 70% | Custom event "Purchase" | Day 30 |
| Engaged free players reaching pity within a comeback | ≥ 50% | ≥ 70% | Economy events | End of Comeback 1 |
| Average daily players | 100 by day 60 | 500 | Creator Analytics | Day 60 |
| Like ratio · policy strikes | ≥ 85% · 0 | ≥ 90% · 0 | Game page · inbox | Ongoing |

The targets are hypotheses from the model, not benchmarks. Reset them after the closed test.

---

## 11. Open questions

| # | Question | Owner | Blocking? |
|---|---|---|---|
| OQ1 | Under Brazil's ECA Digital law, are **free, earned** random packs allowed for minors? Until we know, restricted players get no randomness at all (R5). | Legal | No (safe default) |
| OQ2 | Does Roblox treat Holo and Signed versions as separate items for odds display? We list all 180 combinations, either way. | Roblox policy | No |
| OQ3 | Which content maturity label does the questionnaire give with paid random items declared, and does that limit who can find the game? | Roblox policy | **Yes, before launch** |
| OQ4 | Clearance for the working title and the two fictional group names (trademark search). | Legal / design | **Yes, before marketing** |
| OQ5 | Art for 60 cards, 7 zones and 7 bosses: commission, make in-house, or AI-assisted (within Roblox asset rules)? | Design | **Yes, before content is complete** |
| OQ6 | Who writes the 2+ original songs (with known BPM), and who owns the rights? | Audio | Yes for final Killing Part; prototype uses a placeholder |
| OQ7 | What's the payout share for Fan Club subscriptions? | Data | No (P2) |
| OQ8 | Are the 25% / 8% / 3% retention placeholders realistic for this genre? | Data (closed test) | No |
| OQ9 | Should the Daily Encore window use the device clock (can be spoofed) or fixed UTC times? | Engineering | No |

---

## 12. Timeline and phasing

**Hard constraints:**
- Roblox's paid-random-item rules and Brazil's restrictions are already live, so **the game must comply from day one**.
- Audience Expansion Rewards require an average of 100 daily players.

**Rough plan** (solo developer working with Claude; art and music sourced in parallel):

| Weeks | Milestone | Exit check |
|---|---|---|
| 1–2 | Killing Part prototype in a plain grey test level | Tapping to the beat feels great, or we rethink the core before building more |
| 3–4 | Upgrades, zones and walls from config; bosses; first-time experience | Pacing matches the model in internal play |
| 5–6 | Cards, packs with full odds screens, pity, binder, fusion, the `PolicyService` path, Card Shop | Odds audit passes; restricted path works |
| 7–8 | Store, daily loop, analytics, data safety, feel polish, Reduce Effects | No double grants; no data loss in stress tests |
| 9 | Closed test (20–50 players) | Funnel and arrival times within ±25% of the model |
| 10 | **Launch v1** (7 zones) | — |
| Launch + 3 weeks | **Comeback 1 (v1.1)**, built during weeks 9–12 | Engaged players reach Stadium around day 18 |
| Launch + 6 weeks | **Comeback 2 (v1.2)** | — |

**Dependencies:**
- Card, zone and boss art (OQ5)
- Original songs (OQ6)
- A data-saving library
- The Roblox group and channels for codes

**Key risks:**
- **Retention below the model:** check in the closed test before launch.
- **Art bottleneck:** reuse poses and tier frames.
- **Compliance slip:** one config table drives both rolls and odds; audits run weekly.
- **Economy exploits:** the server is the authority; every currency change is logged.
- **Low-end phone performance:** particle budgets and Reduce Effects.

---

## Appendix: key numbers (from `economy-model.xlsx`)

- **Free-player zone arrival (min played):** Busking Street 5.8 · Showcase Hall 20.4 (wall starts ~12.5) · Music Show Stage 38.5 · Fan Meeting Hall 90 (about day 3) · Concert Hall 206 (about day 5) · Arena 413 (about day 10) · Stadium 779 (about day 18) · World Tour 1,429 (about day 32). Players with 2x Hype and Auto-Stream get there **2.5x faster**.
- **Gems:** 310 free a day → 3.1 pulls → pity in 19.4 days. Bundles give 2.0–2.6 gems per Robux.
- **Odds:** 60 / 28 / 9 / 2.5 / 0.5%; Holo 5%, Signed 0.5%; pity at 60 for Center or better; luck boost ×1.5 on Idol and above.
- **Revenue (placeholder rates):** $0.078 per new player over 30 days, $0.14 over 26 weeks; you keep about 22% of what players spend; paid ads at $0.30 per player don't pay back.
