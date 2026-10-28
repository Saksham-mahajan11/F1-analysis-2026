`# Formula 1 Analytics: A Multi-Perspective Tableau Data Story` 🏎️� 

```
## 📌 Project Overview & Objective
This project delivers a comprehensive, interactive data story exploring Formula
1 racing dynamics through advanced data visualization. By processing deep
historical records alongside modern racing metrics, this repository shifts focus
away from raw, confusing spreadsheets and brings clarity to complex racing
dynamics.
```

```
Using **Tableau**, the dataset is engineered into nine distinct visualizations
bound together into a structured narrative. The core objective is to deliver an
intuitive, evidence-based platform for exploring sporting patterns, optimizing
race predictions, and validating team efficiency.
```

`## Framework: The Three Analytical Perspectives` 🗺️� `The architecture of this project is explicitly divided into three separate foundational analytical perspectives:` 

`### 1. Team Performance Strategy` 🏎️� `Investigates the macro-trends of constructor trajectories, team evolution, engineering dominance, and driver points distribution across racing eras. * **Constructor Championship Points Across Seasons (2009–2026):** Traces the historic rise and fall of the sport's core teams. It visually captures the shifting tides of engineering dominance, tracking the initial early-2010s dominance of Red Bull Racing, their sudden performance drop during the 2014 turbo-hybrid transition, the subsequent long-term supremacy of Mercedes AMG, and the modern multi-team battle lines.` 

```
* **Top Drivers by Championship Points (2024–2026):** Focuses sharply on the
contemporary era. The data reveals Lando Norris and Max Verstappen asserting
themselves at the absolute peak of point production, with McLaren and Red Bull
Racing separating themselves into a tier of their own. It contrasts their
success against the extreme point-scoring struggles visible at Alpine and Kick
Sauber.
```

```
* **All-Time Driver Championship Points Leaderboard:** A historic macro-
visualization contextually mapping the most dominant athletes in motorsport
history. This framework explicitly visualizes the massive, historic point
cushions established by titans Max Verstappen and Lewis Hamilton relative to the
incredibly tight midfield cluster occupied by George Russell, Carlos Sainz, and
Charles Leclerc.
```

`### 2. Motorsport Broadcasting & Strategy` 📺 `Analyzes track conditions, race scheduling frequency, global commercial footprints, and tire compounds to assess how sporting strategy meets commercial broadcasting demands.` 

```
* **Podium Rate by Starting Tyre Compound and Circuit Type:** A specialized
matrix breaking down strategic selection advantages. The visualizations reveal
that starting on the Soft tire compound yields high podium success rates across
traditional Permanent tracks (15.84%) and Street tracks (16.49%). However, it
highlights a stark anomaly on hybrid Street/Park circuits, where Soft tires
plummet to a baseline podium rate of just 8.86%, giving Hard compound starters a
dominant 17.82% edge.
```

```
* **Podium Finishes by Driver and Team (2010–2026):** Aggregates podium
frequencies across more than a decade of racing. It highlights a critical
analytical takeaway: while certain constructors lack consistent multi-car
strength across the team championship standings, exceptional individual driver
skill (e.g., Max Verstappen's performance delta) frequently elevates a car far
beyond its baseline engineering capability.
```

```
* **Grand Prix Host Countries (2020–2026):** Maps the commercial expansion of
Formula 1. The data clearly isolates the United States as the expanding
frontrunner in race frequency, driven by the commercial profitability and
addition of distinct high-profile events like Miami and Las Vegas, while
```

```
traditional international venues maintain a highly uniform, static race
rotation.
```

```
### 3. Technical Reliability & Race Management 📌
Examines operational risks, mechanical limits, safety vulnerabilities, and
track-specific attrition rates to quantify the reliability of the grid.
```

```
* **Failure Types by Constructor (2022–2026):** A stacked metric breakdown
classifying every single Did Not Finish (DNF) event into its root engineering
cause. It monitors mechanical failures, engine blowouts, gearbox issues,
hydraulics, brake failures, and track collisions. Surprisingly, despite elite
championship success, Red Bull Racing exhibits a high density of DNFs
originating from car-related failures rather than track incidents. In contrast,
McLaren demonstrates complete immunity to mechanical-specific retirements over
the observed period.
```

```
* **Driver DNF Rate by Circuit Type (2024–2026):** Cross-references driver error
margins with circuit geometry. Permanent tracks represent the highest baseline
threat level across the board, pushing Max Verstappen to a notable 15.38% DNF
rate in those environments. Street tracks introduce distinct hazards that
heavily penalize veteran drivers like Fernando Alonso and George Russell (16.67%
DNF rates), while hybrid Street/Park circuits prove remarkably safe for the vast
majority of the grid.
```

```
* **Race Completion Rate by Season and Team (2010–2026):** A long-term
engineering reliability curve. This view documents how modern quality control
and engine architecture have steadily pushed average grid reliability close to
the 90-100% threshold, mapping distinct engineering anomalies such as Haas F1's
extreme reliability collapse during the 2020 season.
```

# `##` 📊 `Summary of Visualizations in the Tableau Story` 

```
| ID | Visualization Title | Key Data Fields Monitored | Strategic Insight
Target |
| :--- | :--- | :--- | :--- |
| **1** | Constructor Championship Points | `Season`, `Points`, `Team` |
Tracking constructor era dominance & performance dips. |
| **2** | Top Drivers Points (2024-2026) | `Driver`, `Points`, `Team`, `Season`
| Present era evaluation of frontrunners vs. struggling teams. |
| **3** | All-Time Driver Points Leaderboard| `Driver`, `Sum(Points)`, `Team
Details` | Macro historical tracking of legendary career point totals. |
| **4** | Podium Rate Matrix | `Starting Compound`, `Circuit Type`, `Avg. Podium
Flag` | Identifying optimal tire choice configurations by track type. |
| **5** | Podium Finishes by Driver/Team | `Driver`, `Team`, `Sum(Podium Flag)`
| Comparing driver talent index vs. car package efficiency. |
| **6** | Grand Prix Host Countries | `Country`, `Distinct Count(RaceId)`,
`Season` | Visualizing commercial growth and territorial expansion. |
| **7** | Failure Types by Constructor | `Team`, `DNFflag`, `DnfReason` |
Granular profiling of powertrain and mechanical stress points. |
| **8** | Driver DNF Rate by Circuit Type | `Driver`, `CircuitType`, `Avg.
DNFflag` | Highlighting specific environmental weaknesses per driver. |
| **9** | Race Completion Rate Trend | `Season`, `Race Completion Rate`, `Team`
| Mapping long-term mechanical safety and optimization trends. |
```

`## Data Infrastructure & Methodology` 🛠️� `* **Analytical Engine:** Tableau Desktop / Tableau Story interface used to map, sort, filter, and compile relational metrics. * **Temporal Boundaries:** Longitudinal historical data scales from **2009 to 2026**, with focused subsets detailing modern technical regulations from **2022– 2026** and **2024–2026**. * **Methodological Integrity:** Data filters are dynamically linked across worksheets to preserve analytical continuity. Calculations (such as `Avg. DNFflag`, `Race Completion Rate`, and `Avg. Podium Flag`) are derived from` 

```
verified session results.
```

```
## 📌 Critical Analytical Takeaways
```

```
1. **The Street/Park Tire Paradox:** Teams that default to an aggressive Soft
tire strategy on hybrid street/park circuits face a major statistical
disadvantage. The data strongly supports executing a structured shift toward
harder compound strategies on these specific layouts.
```

```
2. **Championship Fragility:** High point yield does not directly correlate with
absolute mechanical reliability. The technical data indicates that frontrunning
teams often extract performance by running components right at their thermal and
structural limits, leading to isolated spikes in mechanical retirements.
3. **Midfield Convergence:** While the elite tier (McLaren, Red Bull) operates
on a distinct tier of point generation, the midfield teams (Ferrari, Mercedes,
Aston Martin) exhibit highly synchronized performance bands, indicating rapid
development convergence under mature regulatory frameworks.
```

`*` ⚠️� `**Data Notice:** The predictive validity and analytical depth of the conclusions presented in this project are strictly bound to the completeness of the baseline datasets, underlying mathematical assumptions, and contextual interpretation of sporting regulations.*` 

