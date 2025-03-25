# A/B Testing Projects: Fast Food Marketing Campaign & Cookie Cats

This repository contains two A/B testing projects focused on analyzing the impact of different strategies on key metrics.  The projects utilize two distinct datasets: the "Fast Food Marketing Campaign" dataset and the "Cookie Cats" dataset.

## Project 1: Fast Food Marketing Campaign

This project investigates the impact of different marketing promotions on sales.  The analysis considers both the overall market and individual market sizes (small, medium, and large).

### Dataset

The "Fast Food Marketing Campaign" dataset contains information on sales associated with three different marketing promotions.  The data is segmented by market size.

### Methodology

A/B testing was performed to compare the effectiveness of the three promotions. Statistical tests (ANOVA and post-hoc tests for normally distributed data, and Kruskal-Wallis test and Dunn Test for not normally distributed data) were used to determine if there were significant differences in sales between the promotions.  Analysis was conducted both on the combined dataset (all market sizes) and separately for each market size.

### Conclusions

The analysis consistently showed the following results across all market segments:

* Promotion 1 and Promotion 3 resulted in significantly higher sales compared to Promotion 2.
* There was no statistically significant difference in sales between Promotion 1 and Promotion 3.

Therefore, it is recommended to prioritize Promotions 1 and 3 over Promotion 2 to maximize sales.

### Files

* `[requirements.txt]` : Python packages required to run the project.
* `[fastfoodmarketingcampaign.ipynb]` : Jupyter Notebook containing the analysis for the Fast Food Marketing Campaign dataset.

## Project 2: Cookie Cats

This project analyzes the impact of changing the in-game gate placement (the level at which players encounter a monetization prompt) on player engagement and retention.

### Dataset

The "Cookie Cats" dataset contains data on player behavior, including retention rates and game rounds played, for two different gate placements (level 30 and level 40).

### Methodology

A/B testing was used to compare key metrics between the two gate placement groups. Statistical tests (e.g., Mann-Whitney U test and Z-test) were employed to determine if there were statistically significant differences in player engagement and retention.

### Conclusions

The A/B test revealed the following:

* No statistically significant difference was found in 1-day retention between the two groups.
* A statistically significant decrease in 7-day retention was observed for the group with the gate placed at level 40.
* A slight, but not statistically significant, decrease in the number of game rounds played was also observed for the level 40 gate placement group.

These findings suggest that moving the gate to level 40 may negatively impact player engagement and, specifically, 7-day retention.

### Recommendation

Based on these results, maintaining the current gate placement at level 30 is recommended.

### Files

* `[requirements.txt]` : Python packages required to run the project.
* `[Cookie_Cats.ipynb]`: Jupyter Notebook containing the analysis for the Cookie Cats dataset. 


## Getting Started

To run these analyses, you will need to have Python (version 3.x recommended) and the necessary libraries installed (e.g., pandas, numpy, scipy, matplotlib, seaborn).  You can install these using pip:

```bash

pip install pandas numpy scipy matplotlib seaborn

