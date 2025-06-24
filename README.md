

## 1. Introduction

### Purpose  
Analyze football player performance data across countries, leagues, and clubs to extract actionable insights for scouting, coaching, and analytics.

### Objective  
Evaluate and compare players using goals, xG, minutes, substitutions, shots, and accuracy to identify top performers and uncover league/country trends.

### Problem Being Addressed  
Clubs and scouts need a data-driven method to identify impactful players and discern performance patterns across various competitions.

### Key Datasets & Methodologies  
- **Dataset:** Player stats (Country, League, Club, Player, Matches, Mins, Goals, xG, Shots, OnTarget, Substitution, Year)  
- **Methods:** Data cleaning, metric creation, segmentation, visualization

---

## 2. Story of Data

### Data Source  
Compiled from Kaggle.com

### Data Collection Process  
Extracted via APIs and manual aggregation; includes season-level player statistics.

### Data Structure  
Rows: One record per player-season  
Columns: Identifiers (Country, League, Club, Player, Year)  
Performance Metrics: Matches, Minutes, Goals, xG, Shots, OnTarget, Substitution

### Key Features & Relevance  
- **Goals & xG:** Measure attacking efficiency  
- **Minutes & Substitution:** Contextualize playing time  
- **Country & League:** Used to compare regional performance

### Limitations or Biases  
- Incomplete xG values imputed using league averages  
- Variations in xG modeling across sources  
- No data on assists or defensive contributions

---

## 3. Data Splitting & Preprocessing

- **Cleaning:** Removed duplicates, standardized naming  
- **Missing Values:** xG values supplemented with league averages  
- **Transformations:** Created Metrics:  
  - Goals per 90 mins  
  - Goal Conversion Rate  
  - xG Performance (Goals – xG) 
- **Variable Separation:**  
  - **Independent:** Country, League, Club, Player, Year  
  - **Dependent:** Goals, Shots, xG, OnTarget, Minutes, Substitution  

**Industry Context:** Sports Analytics  
**Stakeholders:** Clubs, Scouts, Coaches, Media, Fantasy Platforms  
**Value:** Informs recruitment, tactics, performance optimization

---

## 4. Pre‑Analysis

- **Trends:** Messi leads in offensive metrics; Kramaric excels as a substitute; Burgos has top conversion.  
- **Correlations:** Minutes ↔ Goals, xG/match ↔ Goals in certain leagues  
- **Insights:** La Liga sees high xG/match; Italy leads in total goals

---

## 5. In‑Analysis

- **Unconfirmed Hypotheses:** Some players underperform relative to xG; league-dependent shooting efficiency  
- **Excel Techniques:** PivotTables, `SUMIFS`, `IFERROR`, conditional formatting  
- **Early Recommendations:**  
  1. Scout in high-xG leagues (e.g., La Liga)  
  2. Feature substitutes with impact efficiency in lineup  
  3. Prioritize players with high conversion rates

---

## 6. Post‑Analysis & Insights

- **Key Findings:**  
  - Messi tops multiple metrics  
  - Kramaric is an elite “super‑sub”  
  - Burgos is most clinical finisher  
  - La Liga drives high-xG games  
  - Italy leads in aggregate goals  

- **Confirmations & Surprises:** While Messi’s dominance was expected, Burgos’s efficiency and Kramaric’s role were less obvious at the outset.


---

## 7. Recommendations & Observations

- Focus scouting on leagues with higher attacking metrics  
- Deploy high-impact substitutes in key game phases  
- Prioritize players with high conversion efficiency  
- Reallocate resources based on minute/goal efficiency

**Unexpected Findings:** Some substitutes outperform starters; discrepancy between xG and actual goals in certain leagues.

---

## 8. Conclusion

- **Learnings:** Efficiency and context (minutes, conversions) matter as much as raw totals  
- **Limitations:** No assist/defensive data, xG modeling varies  
- **Future Work:** Include assist/defensive metrics, longitudinal tracking, and team-level context

---

## 9. References & Appendices

- **References:** Kaggle, Power BI

---
![TASK 34A](https://github.com/user-attachments/assets/e5478b30-1ca7-490b-86f0-c661582e4283)


