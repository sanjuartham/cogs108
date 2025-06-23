# Understanding What Drives Hospital Ratings in the U.S.  
*COGS108 Final Project – UC San Diego*

## 🏥 Overview
This project explores which **hospital performance metrics** and **patient experience factors** are most correlated with high hospital ratings in the United States. Using two real-world datasets—one covering clinical outcomes like mortality and readmissions, the other covering patient surveys—we examined how operational metrics and survey responses align with CMS overall star ratings.

---

## 💡 Research Question
What patient-experience aspects and operational performance metrics are most strongly associated with higher CMS overall hospital ratings?

---

## 📊 Datasets
### Dataset 1: Hospital General Information  
- [Source (CMS)](https://data.cms.gov/provider-data/dataset/xubh-q36u)  
- 5,425 observations × 39 variables  
- Metrics: Mortality, Readmission, Safety, Facility Info  
- Cleaned down to 1,903 complete rows across 20 variables

### Dataset 2: HCAHPS Hospital Ratings Survey  
- [Source (Kaggle)](https://www.kaggle.com/datasets/thedevastator/hcahps-hospital-ratings-survey)  
- 254,540 observations × 24 variables  
- Focused on questions like cleanliness, nurse communication, care transitions, and patient recommendation  
- Filtered and joined using `Facility ID` / `Provider ID`

> Due to GitHub file size restrictions, raw datasets are not included in this repository. Download them using the links above.

---

## 🔍 Methodology
- **Cleaned and merged datasets** using unique hospital identifiers
- **Exploratory data analysis** on three key CMS measure groups:
  - Mortality
  - Safety
  - Readmission
- **Survey question correlation analysis** via:
  - Star rating distributions
  - State-level averages
  - Spearman correlation matrices
- Compared hospital performance metrics vs. patient satisfaction metrics

---

## 📈 Key Results

### 📌 From Hospital Performance Metrics:
- **Readmission metrics** had the strongest correlations with overall hospital ratings.
- Hospitals with **more “better than national” readmission scores** had higher overall ratings.
- Mortality and safety measures showed moderate relationships.

### 📌 From Patient Survey Ratings:
- Strongest correlations with overall hospital rating:
  - **Recommendation** (ρ = 0.42)
  - **Care Transition** (ρ = 0.40)
  - **Summary Rating** (ρ = 0.36)
- **Quietness** had the weakest correlation (~0.14) but was still statistically significant.
- Patient experience is tightly linked to overall perception of quality.

### 📊 Visualizations:
- Histograms for performance measure groups
- Correlation matrix heatmaps for HCAHPS questions
- Bar charts comparing average ratings per state and hospital

---

## 🎯 Takeaways
- Improving **patient recommendation likelihood, care transitions, and nurse communication** may be the most effective way to raise hospital ratings.
- Readmission performance also plays a key operational role.
- Hospital administrators should focus on both clinical outcomes and patient interaction quality for holistic improvement.

---

## 👥 Team Members
- **Sanjuktha Artham** — Dataset 1 cleaning, EDA, graphing, hypothesis framing  
- Kaye Falaminiano — Dataset 2 cleaning, statistical merges, final synthesis  
- Beatrice Fernandez — Background, hypothesis, ethical framing  
- Vinuthna Maradana — Survey visualization and analysis  
- Dinh Nguyen — Combined dataset comparison, write-up and conclusion

---

## 📎 Course Info
**COGS108: Data Science in Practice**  
UC San Diego – Spring 2024  
Instructor: [Course staff]

---

## 🧠 Skills Demonstrated
`Python` · `Pandas` · `Seaborn` · `Matplotlib` · `Spearman Correlation` · `Data Cleaning` · `Data Merging` · `Healthcare Analytics` · `EDA` · `Team Collaboration`

---

## 📣 Extras
🎥 [Final Video Presentation](https://drive.google.com/file/d/1Iyf6idnnu8zYZpajj6XrnRo9BIToLWmY/view?usp=drivesdk)  
