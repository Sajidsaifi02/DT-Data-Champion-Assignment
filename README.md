# DT-Data-Champion-Assignment
This assignment helps you evaluate your ability to automate a live dashboard using spreadsheet formulae and conditional formatting. 
Personality Assessment Dashboard
This project calculates and ranks participants based on personality assessment scores, displaying results on a leaderboard with visual performance indicators.

Tools Needed
Google Sheets or Excel
Lookup Functions (VLOOKUP, INDEX, MATCH)
Conditional Formatting (Green, Yellow, Red for score ranges)
Array Formulas to automate calculations
File Structure
DataSet1 Basic Screening: Raw participant data for basic screening.
DataSet2 Advanced Screening: Raw participant data for advanced screening.
DataSet3 Key Basic: Answer key for basic screening.
DataSet4 Key Advanced2: Answer key for advanced screening.
Formulae: Scoring formulas.
Sample Leaderboard: Example leaderboard format.
Steps to Implement
Import Data: Load raw data from DataSet1 and DataSet2.
Score Calculation: Use lookup functions to match answers with the keys and calculate total scores.
excel
Copy code
=IF(C2=VLOOKUP(A2, '[DataSet3 Key Basic]DataSet3 Key Basic'!$A$2:$C$32, 2, FALSE), VLOOKUP(A2, '[DataSet3 Key Basic]DataSet3 Key Basic'!$A$2:$C$32, 3, FALSE), 0)
Ranking: Use RANK to assign rankings based on scores.
Conditional Formatting: Color-code scores: Green (80+%), Yellow (50-80%), Red (<50%).
Feedback: Add feedback based on score ranges.
Finalization: Share the final Google Sheet link with "view only" permissions.
Optional Enhancements
Add visualizations (charts) for score distributions.
Implement dynamic filters for data exploration.
