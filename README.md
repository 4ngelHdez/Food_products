# User Behavior Analysis in a Food Products Mobile Application

### Project Description<br>

In this project, I focused on analyzing user behavior within the mobile application of a food products start-up. The main goal was to investigate how users interact with the app over a specific time period, identify usage patterns, and evaluate the effectiveness of different stages of the event funnel using an A/A/B test.

### Objectives:<br>

   * Validate the integrity of the app’s data.<br>
   * Analyze the event funnel to understand user flow throughout the app.<br> 
   * Study the results of an A/A/B experiment to identify potential significant differences between groups.<br>

### Methodology:<br>

I used Python and libraries such as pandas, numpy, seaborn, plotly, scipy, and statsmodels to conduct an exploratory analysis and evaluate the validity of the A/A/B test. Key tasks included:<br>
  * Analyzing user data collected between July 25, 2019, and August 7, 2019.<br>
  * Performing thorough data preparation, including data type checks, detection and removal of duplicates, and column transformations for deeper analysis.<br>
  * Examining event frequencies and the number of unique users at each funnel stage.<br>
  * Reviewing the time period covered to identify and exclude early outliers that could distort experimental results, focusing on the app’s peak activity period (August 2019).<br>
  * Conducting proportion tests and the Mann-Whitney U test to compare experimental groups (246, 247, and 248) and determine if significant differences existed among them.<br>

### Key Findings:<br>

   - The most frequent event was MainScreenAppear, followed by OffersScreenAppear, CartScreenAppear, and PaymentScreenSuccessful. Tutorial was the least frequent event.<br>

   - A total of 7,551 unique users were recorded during the study period.<br>

   - Average number of events per user: 32.28.<br>

   - The largest drop-offs occurred between the main screen and the offers screen (loss of 2,826 unique users) and from successful payment to tutorials (2,699 unique users lost).<br>

   - Only 11.15% of users completed the full process from their first event to a successful payment.

   - Despite threshold adjustments and Sidak alpha correction, the statistical tests (Z-test for proportions and Mann-Whitney U) indicated significant differences between experimental groups (246, 247, and 248). This suggests either improper randomization or inherent behavioral differences between groups.<br>
   
### Tools & Technologies:<br>

   * Python (pandas, numpy, seaborn, matplotlib, plotly express, scipy).<br>
   * Jupyter Notebook for analysis documentation.<br>
   * Z-test for proportions and Mann-Whitney U for statistical validation.<br>

This analysis provided a detailed understanding of user behavior within the app, highlighting key areas for improving the conversion funnel and the importance of ensuring proper group randomization in future A/A/B experiments.
