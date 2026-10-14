# Student Performance & Academic Analytics

## 1. Project Objective

This project is downloaded from internet for using for this EDA proj

**Source-** https://archive.ics.uci.edu/dataset/320/student+performance 
**used dataset from here is student-mat.csv**

The objective of this project is to analyze student mathematics performance and understand how final grades relate to study time, attendance, parental education, family background, previous academic results, extracurricular activities, and sex.

The project uses Exploratory Data Analysis (EDA) to identify patterns, relationships, and factors associated with students' final mathematics grades.

## 2. Dataset

- **Dataset file:** `student-mat.csv`
- **Dataset focus:** Student achievement in mathematics.
- **Number of rows:** 395
- **Number of columns:** 33
- **Target variable:** `G3` — final mathematics grade.
- **Previous grade variables:** `G1` and `G2`.

The dataset contains student-related information, including study time, absences, parental education, family size, family relationships, guardian, extracurricular activities, and previous academic performance.

The dataset was loaded using Pandas with a semicolon (`;`) separator.

## 3. Analysis Performed

The following analyses were performed in the project:

- **Dataset Overview:** Examined the number of rows and columns, column names, data types, summary statistics, and unique values.
- **Data Quality Checks:** Checked missing values and duplicate records.
- **Final Grade Distribution:** Analyzed the distribution of final mathematics grades (`G3`).
- **Study Time Analysis:** Compared final grades across different study-time categories.
- **Absences Analysis:** Examined the relationship between student absences and final grades.
- **Parental Education Analysis:** Compared student performance based on the education levels of mothers (`Medu`) and fathers (`Fedu`).
- **Family Background Analysis:** Explored grades in relation to family size, parents' living status, family relationship quality, and guardian.
- **Previous Academic Performance:** Analyzed the relationships between `G1`, `G2`, and `G3`.
- **Extracurricular Activities:** Compared grades of students who participated in extracurricular activities with those who did not.
- **Performance by Sex:** Compared final-grade distributions and averages between female and male students.
- **Correlation Analysis:** Examined correlations between numerical variables and final grades.
- **Outlier Analysis:** Used box plots to identify unusually high or low final grades.

### Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## 4. Key Findings

- **Previous grades have the strongest relationship with final grades.** The correlation between `G1` and `G3` is approximately **0.801**, while the correlation between `G2` and `G3` is approximately **0.905**.
- **Absences have a very weak linear relationship with final grades.** The correlation between `absences` and `G3` is approximately **0.034**.
- **Study time shows differences in average grades.** The average `G3` is approximately 10.05 for study-time category 1, 10.17 for category 2, 11.40 for category 3, and 11.26 for category 4.
- **Parental education shows differences in average performance.** Students in higher parental education categories generally show higher average final grades in this dataset.
- **Extracurricular activities show a small difference in average grades.** Students reporting participation have an average `G3` of approximately 10.49, compared with 10.34 for students reporting no participation.
- **Average grades differ between sex groups.** The average `G3` is approximately 9.97 for female students and 10.91 for male students.
- **Family background groups show differences in average grades.** These differences are descriptive and do not establish that family circumstances cause particular academic outcomes.
- **Box plots help identify unusual grade values** that may require further investigation.

## 5. Important Insights

1. **Previous academic performance is an important indicator:** The strong correlations of `G1` and `G2` with `G3` suggest that earlier grades can help identify students who may need additional academic support.

2. **Multiple factors should be considered:** Student performance should be examined using several indicators, including previous grades, study time, absences, and individual circumstances.

3. **Absences alone do not explain final grades:** The correlation between absences and `G3` is very weak in this dataset. However, this does not prove that attendance is unimportant in every situation.

4. **Group differences do not prove causation:** Differences related to parental education, family background, extracurricular activities, and sex may be influenced by other factors not included in the analysis.

5. **Unusual grades should be reviewed carefully:** Outliers may represent genuine student performance and should not automatically be removed without investigation.

## Conclusion

This project analyzes mathematics performance among 395 students using Exploratory Data Analysis. It examines academic history, study time, absences, parental education, family background, and extracurricular activities.

The findings show that previous grades, particularly `G2`, have the strongest observed relationships with the final grade `G3`. Absences have a very weak linear correlation with final grades, while other variables show differences across student groups.

The analysis provides useful insights into student performance and demonstrates how data analysis and visualization can help identify academic patterns.

## Limitations

- The dataset focuses on mathematics performance and may not represent performance in other subjects.
- The dataset contains 395 student records and may not represent all student populations.
- The analysis identifies associations and does not establish cause-and-effect relationships.
- Some factors affecting student performance may not be included in the dataset.
- The correlation between absences and final grades measures a linear relationship and may not capture every possible relationship.
- Unusual grade values are identified for review and are not automatically treated as errors.
