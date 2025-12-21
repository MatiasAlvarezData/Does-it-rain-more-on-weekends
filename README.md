# 🌦️ Does it really rain more on weekends in Buenos Aires?
> **A statistical analysis of cognitive biases and weather patterns (2020–2025)**

---

## 📌 Project Overview
This project investigates the popular belief that rainfall is more frequent or intense during weekends in the city of Buenos Aires. Using daily precipitation data from the **Buenos Aires Central Observatory (Meteostat/SMN)**, we apply statistical hypothesis testing to demystify whether this phenomenon is a climatological reality or a result of confirmation bias.

---

## 📊 Business & Research Questions
1.  **Probability:** Is there a statistically significant difference in the probability of rain between weekdays (Mon–Thu) and the extended weekend (Fri–Sun)?
2.  **Intensity:** Is the average volume of rainfall ($mm/day$) significantly different between the two groups?

---

## 🛠️ Tech Stack
* **Language:** Python 3.12
* **Libraries:** * `Pandas` & `Numpy` (Data manipulation)
    * `Matplotlib` & `Seaborn` (Data visualization)
    * `Scipy` & `Statsmodels` (Statistical testing)

---

## 🔍 Methodology & Data Quality
* **Source Validation:** The *Meteostat* daily records were cross-referenced against the official **OCBA-SMN** annual summaries. 
* **Reliability:** The dataset showed a **relative error of less than 5%** in both total precipitation and number of rainy days, confirming it as a reliable source for analysis.
* **Data Cleaning:** Handled missing values (imputed as 0 mm based on consistency checks) and validated outliers against historical records.

---

## 💡 Key Findings

### 1. Rain Probability (Z-Test for Proportions)
* **Weekdays:** 26.05% rain probability.
* **Weekends:** 26.44% rain probability.
* **Result:** With a **p-value of 0.85**, we fail to reject the null hypothesis. There is no statistical evidence that the proportion of rainy days differs between weekdays and weekends.

### 2. Rainfall Intensity (Mann-Whitney U Test)
* **Analysis:** Comparing the daily precipitation distributions for both groups.
* **Result:** The **p-value of 0.61** indicates no significant difference in the daily precipitation distribution. The observed variations are due to natural climate variability.

---

## 📈 Featured Visualizations

### Data Validation
<img width="623" height="386" alt="image" src="https://github.com/user-attachments/assets/766a5c16-78e9-403d-a434-3f1be8e24bbb" />

*Absolute percentage error comparison between Meteostat and official OCBA records.*

### Comparative Analysis
<img width="567" height="449" alt="image" src="https://github.com/user-attachments/assets/cb382c0c-cef1-4694-bbc6-595caeac9006" />

*Visual comparison of rain probability showing minimal variance between day types.*

---

## 🏁 General Conclusion
The analysis demonstrates that the perception of a "weekend rain curse" in Buenos Aires is a **cognitive bias**. Data from the last 5 years shows that atmospheric behavior is uniform throughout the week. This project highlights how data science can be used to debunk common urban myths with statistical rigor.

---

## 📂 Repository Structure
* `precip_weekends_bsas_eng.ipynb`: Complete analysis and source code.
* `export.csv`: Raw daily weather data.
* `ocba.csv`: Official annual records used for validation.

---
**Author:** Matías Alvarez

**Contact:** (https://www.linkedin.com/in/mat%C3%ADas-alvarez/)
