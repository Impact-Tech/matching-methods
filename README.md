# Matching Methods Utility 
## Run impact analysis using matching methods.

### Intended flow:
- Step 1. **Data Prep/Load**: Normalized labelled data (CSV) with response column, independent variables & the treatment column. Generates "AnalysisID" for step-by-step analysis.
- Step 2. **Data Check**: Run Balance & Overlap checks for AnalysisID - prints histograms and stat summaries. If satisfactory, proceed to Step 3.
- Step 3a. **Run Matching**: Run Matching Method (default Nearest Neighbor, but can use other in the future) and print the matched samples subset. It will also print a summary of how the propensity scores for original data vs matched.
- Step 3b. **Matching Checkpoint**: Concurrently, we need to review how the balance has altered after matching (report on distribution pre / post matching), 
- Step 4. **Difference in Response Variables**: Calculate the difference and report in the response variables between the matched entities.
