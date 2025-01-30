# Tampa-Bay-Rays-Relocation-Analysis

**Overview**

This project sought to assess, analyze, and improve the Tampa Bay Rays team performance for the 2024 season through fiscally-appropriate player acquisitions and financial state via a collaboration of proven ticketing and promotional strategies.  Due to the damages caused by Hurricane Milton, the report was expanded to assess the effectiveness of previous team relocations and to use predictive modeling to analyze which potential location could be the best fit based on relevant factors of each Metropolitan area.

**Background**

As a team, the Tampa Bay Rays failed to achieve their yearly goal to qualify for the Major League Baseball (MLB) Playoffs in 2024. As an organization, the Rays valuation of $1.25 billion ranks 27th and generated revenues of $301 million ranks 28th in the league (Forbes, 2024).

**Methodology**

Player Performance Metrics Analyzed - Hitters: Plate appearances, Home Runs, Runs Scored, Runs Batted In (RBI), Stolen Bases, Batting Average, Walk Percentage, Strikeout Percentage, Batting Average for balls-in-play (BABIP), On-Base plus Slugging Percentage (OPS), Weighted On-Base Average (wOBA), Weighted Runs above Average (wRAA)

Player Performance Metrics Analyzed - Pitchers: Wins,	Losses, Games Started (starting pitchers only), Saves (relief pitchers only), Innings Pitched, Strikeouts per 9 Innings Pitched, Walks per 9 Innings Pitched, Batting Average against for balls-in-play (BABIP), Earned Run Average (ERA)

Team Metrics Analyzed: Team Wins (2024 season), Team Losses (2024 season), Team Payroll, Player Salaries, Home Attendance by Day, Home Attendance by Opponent,
Home Attendance by Promotion Offered

Metropolitan Area Metrics Analyzed: Metropolitan area population – impacting potential attendance, Per-capita income rank – impacting potential revenue generated per fan, TV market rank (Nielsen ratings) – impacting media and broadcasting revenue, Distance to nearest MLB competitor – impacting professional competition, Local Fortune 1000 companies – impacting potential sponsors

**Model Development**

To determine which Rays players underperformed given their salary, a player required a negative performance in wRAA or a high ERA and a minimum of 10 players with higher wRAA or lower ERA who are also earning a lower salary. For player acquisitions, a Constrained Optimization best-case, worst-case approach was applied based on projected outcomes from Fangraphs.com.

To evaluate the economic impact of dynamic pricing, a linear regression prediction model was created to estimate revenues if the average ticket price increased by $2. 

For relocation factors, data was extracted for 11 current MLB team host cities and 14 potential relocation candidate cities. A random forest prediction model was trained on 20 cities to predict the relocation accuracy of 5 cities, plus Tampa as a comparison point. Charlotte was determined as the best relocation option with 69% confidence from the prediction model, besting Tampa with 61% confidence.

**Limitations and Future Work**

Data Coverage - Limited in size fo training dataset which could attribute to overfitting.
•	Lack of publicly available data for concessions, parking, and merchandise revenues. 

Mean Imputation - To predict missing data for Montreal's TV market rank (as Canada does not use Nielsen ratings). 

Future adaptations of team assessments should include a train and test dataset to use in a prediction model for next year’s player performance metrics and to execute a regression analysis on the model to verify accuracy. Also, future assessments should include metropolitan area data for all 30 MLB team host cities as a “baseline city” comparison. Finally, adding adjustments for local cost of living and individual state taxes would benefit the player payroll analysis.

**Authors**

Patrick Holsey, Connor Walsh

**Acknowledgments**

Chen, K. et al. (2023). “Pay to Play: An Analysis of Payroll and Performance in the MLB and NBA”. 
In a blog published in the Harvard Sports Analysis Collective, the authors evaluated how team payroll impacts wins. In their analysis, the authors defined “Relative Salary” for an MLB team and utilized the Herfindahl–Hirschman index (HHI) to measure payroll concentration among players.

Miller, T. (2015). “Sports Analytics and Data Science: Winning the Game with Methods and Models”. 
In Chapter 8, Miller defines consumer’s market segmentation and how target marketing actions can increase organizational revenues. In Chapter 9, Miller uses a cost-volume-profit analysis to assess particular aspects of MLB game-day revenues from ticket, concessions, and merchandise sales.

Mornat, G. and Garg, T. (2022). “Valuation Drivers of Major League Baseball Franchises: Revenue Streams, Cost Structure, and M&A Rationales". 
The authors’ break down specific MLB profitability metrics, including drivers of game-day attendance. Factors including: day of the week, current performance of the home team, and quality of the venue are discussed.

**License**

This project is licensed under the MIT License - see the LICENSE file for details
