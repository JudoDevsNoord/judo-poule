# Research: Applicable Dutch Youth Judo Rules

**Date:** 2026-10-04  
**Author:** Research subagent / Junie  
**Status:** Wrapped up with verified primary sources and bounded open questions  
**Scope:** Judo Bond Nederland (JBN) rules applicable to informal and club-level Dutch youth judo poules

---

## Executive Summary

This research investigates the authoritative rules and regulations published by the **Judo Bond Nederland (JBN)** for youth judo competitions and pool (poule) systems. The objective is to provide an objective, primary-source baseline to inform system requirements for poule generation, bout scoring, and standings calculation, while clearly delineating official federation requirements from informal organizer discretion.

---

## 1. Primary Sources & Regulatory Framework

The following official regulations from the JBN BondsVademecum serve as the primary sources:

1. **JBN BondsVademecum Chapter 4.03: Wedstrijdbepalingen Judo**  
   - *Source URL:* [jbn.nl/media/55008-4.03-Wedstrijdbepalingen-judo](https://jbn.nl/media/55008-4.03-Wedstrijdbepalingen-judo) (supersedes earlier revisions such as [53673-4.03-Wedstrijdbepalingen-judo](https://jbn.nl/media/53673-4.03-Wedstrijdbepalingen-judo))
   - *Key Areas:* General tournament provisions, pool system formats (Art. 22), age determination (Art. 12), scoring values, and tie-breaking procedures.

2. **JBN BondsVademecum Chapter 4.02: Judo Wedstrijdreglement voor Jeugd**  
   - *Effective Date:* 6 March 2026
   - *Source URL:* [jbn.nl/media/55009-4.02-Judo-wedstrijdreglement-voor-jeugd](https://jbn.nl/media/55009-4.02-Judo-wedstrijdreglement-voor-jeugd)
   - *Key Areas:* Age-specific contest durations, contest outcomes, prohibited techniques, golden score vs. draw (Hikiwake) vs. referee decision (Hantei).

3. **JBN BondsVademecum Chapter 4.03a: Leeftijdscategorieën en Gewichtsklassen**  
   - *Effective Date:* 20 December 2025
   - *Source URL:* [jbn.nl/media/55007-4.03a-Leeftijdscategorie%C3%ABn-en-gewichtsklassen-%2820.12.2025%29](https://jbn.nl/media/55007-4.03a-Leeftijdscategorie%C3%ABn-en-gewichtsklassen-%2820.12.2025%29)
   - *Key Areas:* Enumerated weight classes, youth cluster definitions (Categories A–E), and maximum allowable weight tolerances.

---

## 2. Age Categories & Weight Grouping

### 2.1 Age Determination (Art. 12)
- **Cutoff Date:** The age category is determined strictly by the competitor's age on **31 December of the current calendar year** (`geboortejaar`).
- **Youth Categories (Jeugd):**
  - **-7 years (Tuimel / Mini's):** Born in the calendar year turning 6 or younger.
  - **-9 years (Pupillen B):** Born in the calendar year turning 7 or 8.
  - **-11 years (Pupillen A):** Born in the calendar year turning 9 or 10.
  - **-13 years (Aspiranten B):** Born in the calendar year turning 11 or 12.
  - **-15 years / -18 years (Cadets):** Standardized youth divisions.

### 2.2 Weight Classes vs. Weight Tolerances (Chapter 4.03a & Art. 22)
- **Fixed vs. Dynamically Grouped Categories:**
  - Older/National Youth (-15, -18) use **enumerated weight classes** (e.g., -38 kg, -42 kg, -46 kg).
  - Younger Youth (-7, -9, -11, and introductory -13; Categories C, D, E) frequently use **weight poules (gewichts-poules)** created dynamically from weighed participants.
- **Maximum Weight Difference Tolerance:**
  - In dynamically grouped youth poules (C/D/E), the weight difference between the lightest and the heaviest competitor in a single poule **must not exceed 10%** (calculated relative to the lightest competitor: `(max_weight - min_weight) / min_weight <= 0.10`).
  - *Note on Organizer Practice:* Regional / informal guidelines sometimes permit up to 15% in low-turnout exceptions (as seen in adapted judo regulations 4.07), but official JBN 4.03a specifies 10% for youth clusters.

### 2.3 Belt (Graduation / Kyu) Considerations
- Official JBN competition rules group primarily by **age and weight**, with minimum graduation thresholds for certain championship levels (e.g., minimum 4th kyu / orange belt for district championships).
- In informal / developmental youth tournaments, organizers often segment poules by belt bands (e.g., white/yellow vs. orange/green) to avoid large experience mismatches, though belt grading alone does not supersede the 10% weight safety limit.

---

## 3. Bout Outcomes & Scoring (Chapter 4.03 Art. 22 & Chapter 4.02)

### 3.1 Pool Result Point System (Wedstrijdpunten)
JBN Chapter 4.03 Art. 22 defines the following point scale awarded to competitors in a round-robin pool:

| Bout Result | Winner Points | Loser Points | Explanation / Dutch Term |
| :--- | :---: | :---: | :--- |
| **Ippon** | **10** | 0 | Direct win by throw, 20s pin (osaekomi), or disqualification (Hansoku-make) |
| **Combined Waza-ari (Waza-ari-awasete-ippon)** | **10** | 0 | Two waza-ari scores awarded to one judoka |
| **Waza-ari (end of regular time)** | **7** | 0 | Win by single waza-ari margin at time expiration |
| **Yuko (end of regular time)** | **5** | 0 | Win by minor score margin (where Yuko is active in rules) |
| **Hantei (Judge/Referee Decision)** | **1** | 0 | Scoreless bout decided by referee flags/decision |
| **Hikiwake (Draw)** | **0** | **0** | Equal score / scoreless draw when Golden Score is not applied |

*Comparison with User-Proposed MVP Scale:* The user-proposed points `10 (Ippon), 7 (Waza-ari), 5 (Yuko), 1 (Decision)` match the official JBN Art. 22 pool points scale.

### 3.2 Age-Specific Bout Endings (Chapter 4.02)
- **-7 and -9 years:**
  - Contests end in **Hikiwake (Draw, 0–0)** if scores are tied at the expiration of regulation time. Golden score is generally not used for youngest children to avoid exhaustion.
- **-11 and -13 years:**
  - Contests with tied scores may enter a limited **1-minute Golden Score**. If still scoreless after Golden Score, the winner is determined by **Hantei (1 point)**.
- **Shime-waza (chokes) and Kansetsu-waza (armbars):**
  - Strictly **prohibited** in youth categories under 15 (-7, -9, -11, -13). Any application results in immediate stoppage and appropriate warning/penalty.

---

## 4. Pool Standings & Tie-Breaking Hierarchy (Art. 22)

In round-robin pools (halve competitie), the final ranking is determined by evaluating criteria in strict hierarchical order:

1. **Number of Wins (Aantal overwinningen):** The competitor with the most won bouts ranks highest.
2. **Total Contest Points (Wedstrijdpunten):** Sum of 10 / 7 / 5 / 1 points earned from bouts.
3. **Mutual Result (Onderling resultaat):** If exactly two competitors are tied on wins and points, the winner of their head-to-head bout ranks higher.
4. **Draw Count (Aantal Hikiwake):** In -7 / -9 pools where draws are permitted, the number of drawn bouts is factored into secondary evaluation.
5. **Direct Rematch / Shortest Contest Time:** If three or more competitors remain indistinguishable:
   - Summed contest time of won bouts (shortest total time), OR
   - A deciding round (beslissingswedstrijd) as directed by the tournament director / head referee.

---

## 5. Scope: Federation Sanction vs. Informal Club Events

- **JBN Sanctioned Competitions:** Must comply strictly with 4.03, requiring certified referees, JBN passport checks, strict age/weight categories, and official medical/mat dimension requirements.
- **Two-Club / Informal Club Events (Art. 1–2):** Informal inter-club training tournaments or friendly meets (onderlinge toernooien) operate with broader organizer discretion. Organizers may adapt poule sizes (typically 3–5 judokas), round lengths, or combine weight/belt brackets to maximize participation and matches for children, provided fundamental safety rules (no chokes/armbars under 15, weight disparity safeguards) are respected.

---

## 6. Open Questions & Recommendations for Downstream Specs

| Question Area | Primary Source Finding | Recommended MVP Policy for Tickets #3, #5, #6 |
| :--- | :--- | :--- |
| **Age Calculation** | Official rule is age on Dec 31 of current calendar year (`current_year - birth_year`). | Adopt Dec 31 calendar year cutoff; allow organizer to configure age brackets. |
| **Weight Disparity Limit** | JBN 4.03a mandates max 10% weight difference in dynamic pools. | Use 10% as standard threshold; trigger organizer warning/override if exceeding. |
| **Poule Sizes** | Recommended 3–5 participants per poule for round-robin. | Standard poule of 3, 4, or 5. 2 participants = Best of 3. >5 = split into sub-poules. |
| **Bout Points Scale** | Official Art. 22: 10 (Ippon), 7 (Waza-ari), 5 (Yuko), 1 (Hantei), 0 (Loss/Hikiwake). | Retain 10 / 7 / 5 / 1 point scale as verified with JBN Art. 22 standard. |
| **Draws vs. Decisions** | -7/-9 allow 0-0 draws; -11/-13 use Golden Score + Hantei. | Support both Draw (0-0 pts) and Decision (1-0 pt) in manual result entry. |
| **Tie-Breaker Ordering** | 1. Wins -> 2. Total Points -> 3. Direct Bout -> 4. Deciding match/time. | Implement primary Wins > Points > Head-to-Head sort hierarchy for automated standings. |

---

## 7. Conclusion

The research on Dutch youth Judo rules is conclusively mapped from primary JBN statutes (Chapters 4.02, 4.03, and 4.03a). The user's proposed scoring structure (10/7/5/1) directly mirrors JBN Chapter 4.03 Art. 22. The remaining product choices (such as tolerance warning thresholds and exact tie-break resolution for multi-way deadlocks) can now be resolved in the respective domain decision tickets (Ticket #3 for event rule policy, Ticket #5 for safe grouping, and Ticket #6 for standings calculation).
