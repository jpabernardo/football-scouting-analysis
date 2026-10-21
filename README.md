# Benfica Winter Window: A Data-Driven Scouting Report

> **Which signings would make sense for SL Benfica in the January 2026 transfer window?**
> A side project that goes from team diagnosis to player profiles to a budget-friendly shortlist, using public event data and tactical context.

## Context

- **Snapshot date:** the analysis was built before **Matchday 18 of Liga Portugal 2025/26**, during José Mourinho's first months in charge.
- **Team state at the time:** 17 league games, 11 wins, 6 draws, 0 losses. Benfica was 3rd, behind Porto and Sporting CP.
- **Motivation:** the team was unbeaten but had dropped points in six draws, several of them against low blocks (e.g. Rio Ave, Santa Clara). The question was whether a targeted winter intervention could address that.

The goal isn't to "guess the right name". It's to show how **data and tactical context** can produce a shortlist that is coherent and open to debate.

---

## Approach

```
1. Team diagnosis  →  2. Points-dropped analysis  →  3. Profile definition  →  4. Shortlist & player evaluation
```

| Step | What was done |
|---|---|
| **1. Team diagnosis** | Base XI, passing profile (short / medium / long), xG vs goals over time, and comparison with Porto, Sporting CP and Braga: progressive carries vs progressive passes, take-on success, offensive presence, shot accuracy, possession. |
| **2. Points-dropped analysis** | Draws compared with wins: crosses, attacking-third and penalty-area touches, carries into the box, take-ons per player, goals minus xG per player and per match. |
| **3. Profile definition** | Squad needs turned into two target profiles, each with a position, role, age cap and budget constraint. |
| **4. Shortlist** | Three candidates per profile, filtered and ranked on role-specific per-90 metrics and percentiles, followed by a qualitative strengths and weaknesses assessment. |

---

## Key findings

**How the team plays**
- Patient build-up: short and medium passes make up **more than 88%** of total passing volume.
- Aursnes, Otamendi and Dahl are the clear ever-presents and form the team's spine.
- Benfica leads the Big Three in **offensive presence**, with around 54% of play in the final third, and completes more dribbles from fewer attempts than its rivals.

**Where the team struggles**
- **Territorial dominance without matching efficiency:** among the Big Three, Benfica converts the least of its control into goals relative to xG.
- **Against low blocks the central lane gets shut down.** Carries into the box fall and the team switches to crossing (22.2 crosses per game in draws vs 16.4 in wins), which makes the attack predictable.
- **Dependence on Lukebakio for 1v1 disruption:** his successful take-ons fall from 3.7 to 1.3 per game in draws. No one else in the squad consistently provides that unpredictability.
- **Chance wastage from the second line:** Richard Ríos has the largest negative goals-minus-xG gap in the squad.

**Squad planning**
- Otamendi (37, contract expiring) is near the end of his cycle, and António Silva has not yet secured a starting place. A successor at centre-back needs to be planned now.

---

## Target profiles

| | Profile 1 | Profile 2 |
|---|---|---|
| **Position** | Left winger | Centre-back |
| **Role** | Disruptive winger: 1v1, ball carrying, final-third creation | Pragmatic centre-back: defensive solidity, secure build-up, ball winning |
| **Why** | Restores unpredictability on the flank. Frees Sudakov to play centrally and Aursnes to focus on build-up and balance. | Immediate succession plan for Otamendi |
| **Age** | < 30 | < 30 |
| **Budget** | Budget-friendly | Budget-friendly |

---

## Shortlist

### Left wingers

| Player | Age | Club | Market value | Standout metrics (per 90, percentile) |
|---|---|---|---|---|
| **Sondre Ørjasæter** 🇳🇴 | 22 | FC Twente | €6.0M | Progressive carries 6.96 (top 1%) · Carries into penalty area 3.71 (top 1%) · xA 0.38 (top 1%) |
| **Nilson Angulo** 🇪🇨 | 22 | Anderlecht | €7.0M | Successful take-ons 2.71 (top 4%) · Passes into penalty area 2.35 (top 6%) · Att. 3rd tackles 0.50 (top 6%) |
| **Mika Godts** 🇧🇪 | 20 | Ajax | €15.0M | Successful take-ons 2.64 (top 5%) · Passes into penalty area 2.42 (top 4%) · Carries into penalty area 2.42 (top 4%) |

### Centre-backs

| Player | Age | Club | Market value | Standout metrics |
|---|---|---|---|---|
| **Jorge Salinas** 🇪🇸 | 18 | Racing Santander | €4.0M | Tackles won 2.07 p90 · Interceptions 1.43 p90 · Left-footed full-back converting to CB, high ceiling |
| **Fedde Leysen** 🇧🇪 | 22 | Union SG | €5.0M | Progressive passes 5.50 p90 (top 6%) · Ball recoveries 5.12 p90 (top 4%) · 191 cm |
| **Oumar Solet** 🇫🇷 | 25 | Udinese | €18.0M | Interceptions 1.37 p90 (top 7%) · 87.6% pass completion (top 25%) · 192 cm |

Each candidate has a dedicated slide with **strengths and weaknesses** that put the numbers in context: role dependency, decision-making, physical profile, cost and resale margin.

---

## Data & methodology

- **Source:** [FBref](https://fbref.com/) via **Stathead**. Stathead's advanced data has since been discontinued, so the analysis cannot be reproduced with the same source.
- **Time window:** player metrics cover the **last 365 days** before the snapshot date.
- **Percentile pool:** players compared across **14 selected leagues**, including the top 10 European leagues.
- **Normalisation:** player metrics are per 90 minutes.
- **Market values:** <!-- add source, e.g. Transfermarkt, and date -->
- **Team-level data:** Liga Portugal 2025/26, matchdays 1–17.

## Tools

- **Power BI**: data modelling and all visualisations
- **Excel**: data cleaning and preparation <!-- adjust if you used Python -->
- **PowerPoint / Canva**: final report layout <!-- adjust -->

---

## Limitations

- **Small samples:** 17 matches, of which only 6 were draws. The draws-vs-wins splits are directional, not statistically robust.
- **Event data only:** no tracking or physical data, so pace, intensity and off-ball work are judged qualitatively.
- **Cross-league comparison:** percentiles mix leagues of very different levels, and no league-strength adjustment was applied.
- **No availability or financial filter:** contract length, release clauses, agent situation and wages were not considered.
- **Point-in-time snapshot:** form, market values and squads have changed since the analysis.

## Possible next steps

- League-strength adjustment for cross-league percentiles
- Similarity model (e.g. cosine similarity on role-specific feature vectors) to generate candidates instead of filtering manually
- Comparison of the shortlist with what Benfica actually did in the January window

---

```

## Author

**João**, Data professional · MSc Data Science & Advanced Analytics (NOVA IMS)
[LinkedIn](#) · [Original post](#)

*Personal side project with no affiliation to SL Benfica or any of the clubs mentioned.*
