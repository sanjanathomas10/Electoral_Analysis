# Electoral Analysis <br>
**Python, SQL, Neo4j, Cypher**
---

---
### 📑 Background 📑
---
This project, completed for the university course ST207: Databases, focuses on electoral analysis in the 21st century. The primary goal was to explore trends, patterns, and dynamics in voter turnout, voting methods, and democracy using data from 193 United Nations-recognized countries. The analysis aimed to address critical queries about political participation and democratic processes and to provide a critique of the global political landscape by analyzing contemporary challenges such as declining voter turnout and the evolution of electoral systems.

---
### 🗂️ Data Structure and Sources 🗂️
---
The project utilized a **graph database** built with Neo4j to model the relationships between different entities. 

<img width="482" height="482" alt="Screenshot 2025-09-04 at 9 23 54 PM" src="https://github.com/user-attachments/assets/cd2deeda-75c0-4cc4-8abf-54e8c53f0d2b" />


_**Platforms and data sources used include:**_

[Voter Turnout](https://www.idea.int/data-tools/data/voter-turnout-database) <br>
[Voting Methods](https://www.idea.int/data-tools/tools/special-voting-arrangements/data-explorer) <br>
[Democracy Levels](https://www.systemicpeace.org/polityproject.html) <br>
Opinion Polls: [1](https://www.ipsos.com/en-uk/voting-intentions-great-britain-1997-2002) and [2](https://www.ipsos.com/en-uk/voting-intention-great-britain-recent-trends) <br>
Election Outcomes and Re-election rates: *Wikipedia web-scraping* 

_**Database Management System:**_
Neo4j (local and cloud-based Aura versions) 

_**Querying Language:**_
Cypher 

---
### 📊 Executive Summary 📊
---
This project successfully applied graph database principles to electoral analysis, providing a framework for in-depth insights into political participation and democratic processes. The use of Cypher queries allowed for the exploration of complex relationships within the data.

Insights gained from the analysis are summarized by each query below:

---

**Query 1: How Does Voter Participation Vary Among Institution Type, Region, and Across Time?**

Both parliamentary and presidential countries had fluctuations considering the average voter participation, but it is observed that presidential election voter turnout has faced a larger decline that parliamentary, in the past 5 years, whereas parliamentary election turnout depicts an increasing trend until approximately 2024.

<img width="364" height="267" alt="Screenshot 2025-09-04 at 9 26 43 PM" src="https://github.com/user-attachments/assets/401e853a-ce52-4f81-8c44-576584ad0a92" />

---

**Query 2: Does the Number of Special Voting Arrangements (SVA’s) Available influence Voter Turnout?**

Contrary to predictions, a negative correlation was found between the number of available SVAs and average voter turnout, indicating that as the number of special voting methods increases, the average voter turnout decreases.

| Number of SVA's | Average Voter Turnout (2 d.p) |
|:---|:---|
| 1 | 65.68% |
| 2 | 63.28% |
| 3 | 56.35% |

---

**Query 3: How Well Do Opinion Polls Predict Election Outcome?**

A case study on the UK revealed significantly higher election poll errors for smaller parties. Polls for larger parties proved to be good predictors, with errors below 0.25%, whereas predictors for other parties were less accurate.
<img width="390" height="298" alt="Screenshot 2025-09-04 at 9 28 56 PM" src="https://github.com/user-attachments/assets/95c65b78-3907-4875-a78e-1a0afe83be3c" />

---

**Query 4: What are the countries with the highest re-election rates in both Parliamentary and Parliamentary Elections?**

The analysis identified countries with high re-election rates for parties and candidates. However, the report concluded that a high re-election rate does not necessarily indicate a stable democracy and could instead suggest anti-democratic ruling, election manipulation, or other confounding variables.
| Country_Name | Party_or_Candidate | Election_Type | ReElection Count |
|:---|:---|:---|:---|
| Israel | Likud | Parliamentary | 8 |
| Palau | Independent | Parliamentary | 7 |
| Switzerland | Swiss People's | Parliamentary | 6 |
| Luxembourg | CSV | Parliamentary | 5 |
| Greece | New Democracy | Parliamentary | 5 |
| Belarus | Alexander Lukashenko | Presidential | 5 |
| Azerbaijan | Ilham Aliyev | Presidential | 5 |
| Bulgaria | Georgi Parvanov | Presidential | 4 |
| Bulgaria | Rumen Radev | Presidential | 4 |
| Congo | Denis Sassou Nguesso | Presidential | 4 |

---

**Query 5: How Have Democracy Levels Evolved Over Time and Across Political Regimes?**

The analysis of Polity Scores revealed that the highest rates of democratization typically occur in democratic regimes. Conversely, as expected, countries with the highest negative percentage change in democracy are mostly authoritarian.
| Country Code | Percentage Change | Regime Type |
|:---|:---|:---|
| ZMB | 500.0 | Democratic |
| GHA | 300.0 | Democratic |
| GEO | 250.0 | Democratic |
| COM | 200.0 | Authoritarian |
| DJI | 200.0 | Democratic |
| GIN | -500.0 | Authoritarian |
| ΤΖΑ | -400.0 | Authoritarian |
| KGZ | -366.66666666666663 | Authoritarian |
| HTI | -350.0 | Authoritarian |
| IRN | -333.33333333333337 | Democratic |

---

### 💼 Skills Displayed 💼

---

Exploratory Data Analysis, Database Design and Building, Data Handling and Transformation, SQL/NoSQL Querying, Data Visualization
