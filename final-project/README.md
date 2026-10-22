# Final Project 
## Research Question
How does cholesterol levels differ between patients with and without heart disease?
## Data Source and License
I used the Cleveland portion of the Heart Disease dataset from the UCI Machine Learning Repository. 
The file “processed.cleveland.data”, contains 303 patients and 14 columns, including cholesterol, age and heart disease status.  
Link: https://archive.ics.uci.edu/dataset/45/heart+disease
License: This dataset is licensed under a Creative Commons Attribution 4.0 International (CC BY 4.0) license.
Citation: Janosi, A., Steinbrunn, W., Pfisterer, M., & Detrano, R. (1989). Heart Disease [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C52P4X.
## Data Cleaning Log
- I added the column names since the original file had no header.
- Found 4 missing values in ’ca’  and 2 in ‘thal’ 2. I kept these rows as those columns were not used in my analysis.  
- Age, cholesterol and heart disease had no missing values.
- Kept cholesterol outliers because I had no evidence they were recording errors.
- Kept all 303 rows.
## Findings
### Cholesterol by Heart Disease Status
Patients with heart disease had a mean cholesterol of 251.47 md/dL and median cholesterol of 249 mg/dL. Patients without heart disease had a mean cholesterol of 242.64 md/dL and median cholesterol of 234.5 mg/dL. The boxplot shows cholesterol is slightly higher in patients with Heart Disease. Also, there are a few outliers in both groups.
### Age and Cholesterol by Heart Disease Distribution
Cholesterol levels overlap between patients with and without heart disease, with a few unusually high values.

### Age and Cholesterol
Patients with and without heart disease have overlapping cholesterol levels across ages. There is no clear upward or downward pattern between age and cholesterol.
### T-Test Results
The t-value is 1.483 and p-value=0.139. Since p is greater than 0.05, this dataset doesn't provide enough evidence that the groups mean cholesterol levels differ. Therefore, I failed to reject the null hypothesis since the difference was not statistically significant.
## Conclusion
My research question was "How does cholesterol levels differ between patients with and without heart disease? The mean cholesterol was 251.47 mg/dL with disease versus 242.64 mg/dL without disease. The 8.83 mg/dL was not statistically significant with a p=0.139. The graphs show substantial overlap between the 2 groups. I decided to keep the outliers since I have no evidence that there was recording errors. Since this data only had 303 patients it may not represent the wider population to answer this question, which limits how the results can be applied.
## Limitations
The dataset contains only 303 patients from Cleveland and may not represent the wider population. Cholesterol outliers were retained may skew the means and influence the t-test.  A nonsignificant result doesn’t prove that the groups have equal mean cholesterol value. 

## How to Run
1.	Download the ”Final project” notebook and “processed.cleveland.data” file.
2.	Add both files to the same folder.
3.	Open notebook in Jupyter Notebook.
4.	Check if pandas, seaborn,matplotlib and scipy are installed.
5.	Select ** Kernel -> Restart& Run All** to run every cell from top to bottom. 
