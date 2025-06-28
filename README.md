Road Accident Analysis in Million-Plus Cities of India (2020)
Project Overview
This project analyzes road accident data from 50 million-plus cities in India for the year 2020, focusing on identifying the primary causes, subcategories, outcomes, and counts of accidents. Using Python and data analysis libraries like Pandas, Matplotlib, Seaborn, Plotly, and scikit-learn, this project uncovers patterns in accident data to inform targeted road safety interventions. The dataset includes information on various accident causes (e.g., Road Features, Traffic Violations, Over Speeding) and outcomes (e.g., Total Number of Accidents, Persons Killed, Grievous Injuries).
Key Objectives

Identify High-Risk Areas: Highlight cities with the highest accident rates, such as Chennai, Delhi, and Bengaluru, to prioritize infrastructure improvements.
Analyze Accident Causes: Determine the most prevalent causes (e.g., Over Speeding, Driving under Influence) and their subcategories (e.g., Poor Visibility, Defective Vehicle Conditions).
Evaluate Outcome Severity: Assess the severity of outcomes, focusing on fatalities and grievous injuries, to guide emergency response strategies.
Provide Actionable Recommendations: Offer data-driven policy recommendations to enhance road safety, including enforcement, infrastructure upgrades, and public awareness campaigns.

Repository Contents

Analysis_of_Road_Accident_Causes_and_Outcomes_in_Million_Plus_Cities_of_India_(2020).ipynb: The core Jupyter notebook containing the complete analysis, including data loading, cleaning, exploratory data analysis (EDA), visualizations, and insights.
accident_analysis_summary.md: A Markdown file summarizing key findings and policy recommendations for quick reference.
distribution_of_counts.png: A histogram visualizing the distribution of accident counts across all records, enhanced with mean and median lines for clarity.
accident_causes_vs_outcomes.png: A stacked bar chart illustrating the relationship between accident causes and outcomes, highlighting high-impact categories like Junctions.
Regulatory Affairs of Road Accident Data 2020 India.csv (optional): The dataset used for analysis, containing columns for Million Plus Cities, Cause category, Cause Subcategory, Outcome of Incident, and Count. Note: Include this file only if it is publicly shareable.

Dataset Description
The dataset, Regulatory Affairs of Road Accident Data 2020 India.csv, contains 9,550 records across 50 million-plus cities in India for 2020. Key columns include:

Million Plus Cities: Name of the city (e.g., Agra, Chennai, Delhi).
Cause category: Broad cause of the accident (e.g., Road Features, Traffic Violation, Junction).
Cause Subcategory: Specific cause within the category (e.g., Poor Visibility, Flashing Signal/Blinker).
Outcome of Incident: Outcome of the accident (e.g., Total number of Accidents, Persons Killed, Grievous Injured, Total Injured, Minor Injury).
Count: Number of incidents for each combination of city, cause, and outcome (float, with 3 missing values filled with 0 during cleaning).

Data Insights

Shape: 9,550 rows, 5 columns.
Missing Values: 3 missing values in Count, handled by filling with 0.
Duplicates: No duplicate rows detected.
Key Statistics:
Total Accidents: 352,416
Persons Killed: 81,252
Total Injured: 252,575
Grievous Injuries: 123,192
Minor Injuries: 179,898


Notable Trends: Reduced accidents in 2020 likely due to COVID-19 lockdowns, with high-fatality causes like Drunken Driving and Poor Visibility standing out.

Setup Instructions
Prerequisites

Python: Version 3.8 or higher.
Required Libraries:
pandas: For data manipulation and analysis.
matplotlib: For creating static visualizations like histograms.
seaborn: For enhanced statistical visualizations.
plotly: For interactive visualizations like stacked bar charts.
tabulate: For formatting tables in the console or Markdown.
scikit-learn: For data preprocessing (e.g., LabelEncoder).


Jupyter Notebook: For running the analysis interactively.

Installation

Install Python 3.x from python.org or via a package manager like Anaconda.
Install the required libraries using pip:pip install pandas matplotlib seaborn plotly tabulate scikit-learn


If using Jupyter Notebook, install it with:pip install jupyter


Start Jupyter Notebook:jupyter notebook



Running the Analysis

Clone or download this repository to your local machine.
Place the dataset file (Regulatory Affairs of Road Accident Data 2020 India.csv) in the same directory as the notebook, or update the file path in the notebook if stored elsewhere.
Open Analysis_of_Road_Accident_Causes_and_Outcomes_in_Million_Plus_Cities_of_India_(2020).ipynb in Jupyter Notebook.
Run all cells to reproduce the analysis, visualizations, and summary output.
View the generated accident_analysis_summary.md for a concise summary or check the output images (distribution_of_counts.png, accident_causes_vs_outcomes.png).

Methodology
Data Cleaning

Missing Values: Filled 3 missing Count values with 0, assuming no incidents occurred.
Data Types: Ensured Count is float for numerical analysis.
Validation: Checked for negative counts (none found) and verified maximum count (3,148) for outliers.

Exploratory Data Analysis (EDA)

Distribution Analysis: Created a histogram of Count values with Seaborn, enhanced with mean and median lines to show data spread.
City-Level Analysis: Summarized total accidents by city, calculating percentages to identify high-risk areas (e.g., Chennai: 7.47%, Delhi: 7.11%).
Cause and Outcome Analysis: Generated a pivot table and stacked bar chart to explore relationships between causes (e.g., Junction, Traffic Violation) and outcomes (e.g., Fatalities, Injuries).
Rate Analysis: Calculated fatality and injury rates per accident by cause category, visualized with bar charts showing overall rates for comparison.

Visualizations

Histogram: Displays the distribution of accident counts with KDE and statistical markers.
Stacked Bar Chart: Shows accident counts by cause category and outcome, with annotations for the top contributor (Junction: 173,308).
Bar Charts for Rates: Visualizes fatality and injury rates by cause, with text labels and overall rate lines for context.
Tables: Uses tabulate to present top cities, causes, subcategories, and outcomes with counts and percentages.

Key Findings

High-Risk Cities: Chennai (7.47%), Delhi (7.11%), and Bengaluru (5.5%) account for the highest shares of accidents, likely due to high population and traffic density.
Prevalent Causes: Over Speeding and Driving under Influence are the most common causes, with Road Features (20.94%) and Impacting Vehicle/Object (18.85%) leading cause categories.
High-Severity Causes: Drunken Driving has a higher fatality rate despite lower frequency, while subcategories like Poor Visibility and Defective Vehicle Conditions show elevated fatality percentages.
Outcome Distribution: Grievous Injuries (20.94%) and Minor Injuries (20.94%) are highly prevalent, with Total Accidents (352,416) and Total Injured (252,575) indicating significant impact.
City-Specific Trends: Cities like Lucknow and Kanpur have fewer accidents but higher severity, suggesting a need for targeted interventions.

Policy Recommendations
Based on the analysis, the following interventions are recommended:

Infrastructure Improvements: Prioritize road design upgrades (e.g., better signage, junction layouts) in high-risk cities like Chennai, Delhi, and Bengaluru.
Enforcement Campaigns: Strengthen traffic law enforcement targeting Over Speeding and Driving under Influence, especially in cities with high accident rates.
Emergency Response: Enhance trauma care and emergency medical services in cities with high grievous injury rates, such as those linked to Road Features.
Public Awareness: Launch driver education campaigns focusing on avoiding high-risk subcategories like Poor Visibility and ensuring vehicle maintenance to address Defective Vehicle Conditions.
Proactive Monitoring: Implement real-time accident tracking and predictive analytics in high-risk areas to identify and mitigate recurring causes.

Usage Instructions

For Analysts: Run the Jupyter notebook to explore the data interactively, modify visualizations, or extend the analysis with additional metrics (e.g., time-based trends if available).
For Policymakers: Refer to accident_analysis_summary.md for a concise overview of findings and recommendations to inform road safety strategies.
For Developers: The code is modular and can be adapted for other datasets with similar structures. Ensure the dataset has consistent column names and handle any additional cleaning steps as needed.

Future Work

Temporal Analysis: Incorporate data from other years to identify trends over time, especially post-COVID-19 lockdown effects.
Geospatial Analysis: Map accident locations within cities to pinpoint high-risk zones (requires geolocation data).
Machine Learning: Apply predictive models to forecast accident-prone areas or causes based on historical patterns.
Subcategory Deep Dive: Analyze specific subcategories (e.g., Others) in detail to uncover underlying factors.

License
This project is licensed under the MIT License. See the LICENSE file for details.
Contact
For questions or contributions, please contact [Your Name/Email] or open an issue on the repository.
