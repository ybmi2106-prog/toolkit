# Toolkit

## Tools and Methods of Data Analysis

**SRH University Leipzig | MSc Big Data and AI**

---

## Toolkit 1 Normality Test

* **File:** `Normality_toolkit.ipynb`
* **Dataset:** AI Dependency, Career Anxiety and Student Burnout ([Link to Dataset](https://www.kaggle.com/datasets/sridipbasu/ai-depndency-career-anxiety-and-student-burnout))
* **Column analysed:** burnout_score ($n = 200$ random samples)

### Contents:

1. PDF Plot, KDE curve of the data
2. Fitted Normal Distribution, red curve overlay + goodness of fit
3. Q-Q Plot, visual normality check
4. Normality Tests, Shapiro-Wilk, Kolmogorov-Smirnov, Anderson-Darling
5. Conclusion, interpretation of results

### Results Summary:

| Test | Statistic | p-value |
| --- | --- | --- |
| **Shapiro-Wilk** | 0.9682 | 0.0002 |
| **Kolmogorov-Smirnov** | 0.1244 | 0.0037 |
| **Anderson-Darling** | 2.3107 | < 0.05 |

---

## Toolkit 2 T-Test Toolkit

* **File:** `ttest_toolkit.ipynb`
* **Dataset:** AI Student Impact Dataset (50,000 students)

### Tests performed:

1. **One-Sample t-Test:** Skill Retention Score vs benchmark (75)
2. **Two-Sample t-Test:** Anxiety Level: Paid vs Non-Paid subscribers
3. **Paired t-Test:** Pre vs Post Semester GPA after AI tool use

### Results Summary:

| Test | t-statistic | p-value | Decision |
| --- | --- | --- | --- |
| **One-Sample** | 13.44 | < 0.0001 | Reject H0 |
| **Two-Sample** | 14.65 | < 0.0001 | Reject H0 |
| **Paired** | -242.73 | < 0.0001 | Reject H0 |

---

## How to Run

1. Open the relevant `.ipynb` file in Google Colab or Jupyter Notebook.
2. Upload the dataset CSV file.
3. Run all cells in order.

---

## Libraries Used

* pandas
* numpy
* matplotlib
* scipy
