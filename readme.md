# Jakub Mazur - Scientific & Data Analysis Portfolio
I am a biotechnology student and data analyst passionate about solving high-impact problems. My work spans from leading academic projects against antimicrobial resistance to driving data-informed decisions in a commercial environment.

# Real scientific projects
As part of the activity at university, I've had a chance to prepare an analysis from real scientific data:
1) Literature review - available on [Zenodo](https://doi.org/10.5281/zenodo.15640143).
   
2) [Dashboard](https://github.com/AaKuba/Portfolio/blob/e11f87003f9d5c86531726e7679ecadd8fe39eef/Scientific%20dashboard.pdf) from a report - a description can be found [here](https://github.com/AaKuba/Portfolio/blob/d81c718e847164bc03c56abdb660f00f0e464316/Projects%20files/Description%20-%20scientific%20dashboard).
3) Report on the effects of the funding program for the agriculture sector - LLM were used for translations the original paper, available [here](https://github.com/AaKuba/Portfolio/blob/fe725c8ed851efdfcdc2808ddca7bfb91bfe76a4/Projects%20files/Jakub%20Mazur%20-%20O%20efektach%20statystycznych%20poddzia%C5%82ania%206%2C2%20ENG.pdf).

Upcoming projects: literature reviews about ESKAPE pathogens, original articles about vitamin C in fighting pathogens, and environmental and social analysis.

# Project 1 
This project focuses on the basic analysis of flights in India. The dataset was obtained from [Kaggle](https://www.kaggle.com/datasets/rohitgrewal/airlines-flights-data).
The dashboard was prepared in Power BI and can be obtained [here](https://github.com/AaKuba/Portfolio/blob/3ecf810c7d119ce906bbea2917deb0516db4ee75/Projects%20files/Flight%20analysis%20porfolio.pbix).
Also, SQL code was prepared that could be used for data extraction, on which the dashboard had been based and is available [here](https://github.com/AaKuba/Portfolio/blob/fa9b092ca693a3410a5078e0fadb6b08f203f891/Projects%20files/Project%201%20-%20flight%20analysis%20SQL%20code).

Key Findings & Strategic Insights:
1. Market Landscape
The market is heavily skewed towards Economy Class, which constitutes over 2/3 of all flights (A). This indicates a large, price-sensitive customer base.
Vistara is a dominant player, especially in the premium segment, being one of only two airlines offering Business Class (B).

   Strategic Insight: Direct competition with Vistara in the business segment would be capital-intensive. The primary opportunity lies in capturing the economy market.


2. Geographical Opportunity: The Kolkata Pricing Anomaly
While Mumbai is the most popular destination (C), our analysis revealed that Kolkata is consistently the most expensive destination and departure city, for both classes (D).
Crucially, there is no strong correlation between flight duration/distance and price (E), suggesting that high prices in Kolkata are driven by different factor, for example lack of competition rather than operational costs.

    Strategic Insight: This "pricing anomaly" represents the single greatest market opportunity. A new entrant can disrupt the market by offering significantly lower fares on routes to/from Kolkata.


3. Pricing & Scheduling Strategy: Exploiting Inefficiencies
Morning flights are consistently the most expensive, likely targeting business travelers. The cheapest available carriers are AirAsia (Economy) and Air India (Business).

    Strategic Insight: A new airline can attract a large segment of leisure and budget travelers by focusing on a dynamic pricing model with competitive fares for off-peak hours (afternoon, evening).


Business Recommendations for a new airline:

Market Entry Strategy: Focus operations on high-demand, overpriced routes connecting Kolkata with major hubs like Mumbai and Delhi. Offer a base fare 15-20% below the current market average to rapidly gain market share.

Core Offering: Concentrate primarily on a high-density Economy Class configuration to maximize volume and cater to the largest market segment. A small, competitively priced "Economy Plus" section could be tested as an alternative to a full Business Class.

Pricing Model: Implement a dynamic pricing strategy that offers the lowest fares for off-peak travel (e.g., afternoon, late evening), explicitly targeting budget-conscious travelers and filling planes outside of the morning business rush.


# Project 2
This project focuses on the analysis of students' scores and the impact of the selected factors. The dataset used was obtained from [Kaggle](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors).
The data was additionally extracted using MySQL and the prepared code is available [here](https://github.com/AaKuba/Portfolio/blob/25932dba12b89dd19a77fd6f95c5862c744d73dd/Projects%20files/Students%20results%20SQL%20code.txt).
Due to the selected format (poster) some data wasn't shown and mentioned. Below, the more detailed analysis is shown. The poster can be downloaded from [here](https://github.com/AaKuba/Portfolio/blob/7a0a4aa97dc1c6e56e62bed6225abda3816bdcb0/Projects%20files/Students%20results.png).

Bulletpoints of the analysis (in the brackets, the difference between the two border groups is presented; pp - % points):
1. Parental education and involvement (Δ = 1,08 pp. and 1,59 pp. respectively) have a slight impact on the mean exam results. In addition it's worth noting that the group with low parental involvement could reach a maximum 94 points, compared to the group with high parental involvement, where the maximum score was 100 points.
2. The greater distance from home impacts the mean exam score negatively (Δ = 1,05 pp.)
3. Teacher quality has a greater influence (Δ = 0,93 pp.) than the type of school (Δ = 0,08 pp.)
4. Negative peer influence results in lower exam scores (Δ = 1,06 pp.)
5. Students with learning disabilities are at risk of gaining lower exam scores (Δ = 1,08 pp.). The aspect of maximum score is also worth noting - the highest score in the group with disabilities was 89 points.
6. A moderate positive correlation can be found between exam score and hours spent on studying, and attendance level
7. No significant correlation can be found between exam score and hours of sleep or previous score
8. Students with internet access had a lower mean exam score compared to the group with no internet access (data not shown, Δ = 0,75 pp.)
9. Students from higher class are more likely to receive greater exam scores (data not shown, Δ = 0,99 pp.)
10. Male students tend to receive greater exam scores (data not shown, Δ = 0,32 pp.)


Recommendations
1. Different types of parental involvement should be promoted
2. Implement a teacher screening process focusing on teaching quality metrics
3. Students should be taught about assertiveness to minimize the negative influence of other people
4. Greater aid for students with disabilities should be implemented
5. Classes about motivation for studying and studying techniques should be organized
6. It should be explained to students why attendance in classes is important and how it may help them reach a higher score

In summary, we can see that many factors can impact the exam results. But we have to consider whether changes are significant - comparing mean scores, we can observe differences not reaching 2 percentage points. But for more detailed analysis, it's worth paying attention to the distribution and maximum scores, as they vary. However, the dataset is not perfect and contains surprising but not deeply disturbing data - for example, in the group with no learning disabilities score of 101 points can be found. For real and deep analysis, the data for every group should be additionally screened if incorrect values are present - in SQL it can be done usinga  command like "Select * from results where [name of the column/group] > 100"
