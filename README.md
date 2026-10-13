# F21DL PG Group 13

---

## Project Title
Predicting chronic kidney disease risk levels from routine clinical and lab data.

---

## Group Members
| Name | GitHub |
|---|---|
| Mohamed Elgazar | [elgazar24](https://github.com/elgazar24) |
| Vishwas More | [VishwasMore](https://github.com/VishwasMore) |
| Aisan Mojahedi | [amojahedi](https://github.com/amojahedi) |
| Gül Öner | [username] |
| Afzal Patel | [aap4006](https://github.com/aap4006) |
| Pratham Prashant Shah | [username] |

---

## Research Objectives
- Find which machine learning algorithm predicts a patient's kidney disease risk level best (5 classes, from no disease to severe).
- Find which clinical and lab features matter most for the prediction.
- Compare an MLP neural network with classic ML models on the same data.

---

## Datasets

### Dataset comparison
We compared four datasets before choosing.

| | Dataset 1 | $\color{green}{\textsf{Dataset 2 (chosen)}}$ | Dataset 3 | Dataset 4 |
|---|---|---|---|---|
| Name | [UCI Chronic Kidney Disease](https://archive.ics.uci.edu/dataset/336/chronic+kidney+disease) | [Kidney Disease Dataset](https://www.kaggle.com/datasets/amanik000/kidney-disease-dataset) | [CKD Clinical Dataset](https://www.kaggle.com/datasets/priyankabarik/chronic-kidney-disease-ckd-clinical-dataset) | [BD-KDD](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/MB1LES) |
| Source | UCI | Kaggle | Kaggle | Harvard Dataverse |
| Records | 400 | 20,538 | 21,000 | 988 |
| Features | 24 | 42 | 35 | 24 |
| Target | yes/no | 5 risk levels | 5 CKD stages | yes/no |
| Missing data | 60% of rows | none | none | none |
| Core blood and urine tests (creatinine, urea, hemoglobin, albumin) | yes | yes | yes | yes |
| eGFR (main kidney function measure) | no | yes | yes | no |
| Urine microscopy (red cells, pus cells, bacteria) | yes | yes | no | yes |
| Diabetes and hypertension | yes | yes, plus years with each | yes | yes |
| Advanced biomarkers (Cystatin C, CRP, IL-6, PTH) | no | yes | no | no |
| Lifestyle (smoking, BMI, physical activity) | no | yes | smoking and BMI | no |
| Family history of kidney disease | no | yes | yes | no |
| Usage | 135K views on UCI | 48 votes, 5.7K downloads on Kaggle | 28 votes, 1.7K downloads on Kaggle | new (published March 2026), no usage figures |
| Why not | too small, binary, a lot of missing data | | close, but fewer features and less used | small, binary, very new so no previous work to compare with |

Dataset 3 was the closest alternative. We chose Dataset 2 because it has richer features (including 14 categorical features that need encoding) and it is more widely used on Kaggle.

### Chosen: Dataset 2, Kidney Disease Dataset
- **Source:** [Kaggle (amanik000)](https://www.kaggle.com/datasets/amanik000/kidney-disease-dataset). Origin not stated; the first 24 columns match the [UCI CKD dataset](https://archive.ics.uci.edu/dataset/336/chronic+kidney+disease) (Rubini et al., 2015), so it appears to be an extended version of it.
- **License:** "Unknown" on Kaggle; the UCI source is CC BY 4.0.
- **Class balance:** No Disease 80%, Low 10%, Moderate 4%, High 4%, Severe 2%.
- **Extra data collected:** none.

<details>
<summary>Two example rows (selected columns)</summary>

| Age | BP | Creatinine | eGFR | Hemoglobin | Hypertension | Diabetes | Target |
|---|---|---|---|---|---|---|---|
| 54 | 167 | 7.55 | 71.62 | 11.8 | yes | yes | No_Disease |
| 89 | 128 | 8.31 | 117.70 | 13.3 | no | yes | Severe_Disease |

</details>

---

## Project Milestones
We plan the work as weekly objectives. The detailed tasks for each week are in our Trello board and we assign them in our weekly online meeting.

| Week | Milestone | Req. | Status |
|---|---|---|---|
| W1-W3 | Team, GitHub repo and tools set up, coursework reviewed | Setup | done |
| W2-W4 | Topic, research questions, dataset comparison and choice | R1 | done |
| W3-W5 | Data exploration (statistics, class balance, clinical signals) | R2 | done |
| W4 | Project pitch and slides | D1 | done |
| W4-W6 | Preprocessing (encoding, scaling, class imbalance) | R2 | in progress |
| W4-W7 | Feature engineering and feature selection | R2 | in progress |
| W5 | README proposal, up to the milestones | D1 | in progress |
| W7-W8 | k-means clustering compared with the risk levels | R2 | to do |
| W8-W9 | Classic models: Decision Tree, Naive Bayes, kNN, Random Forest | R3 | to do |
| W9-W10 | MLP neural network, build and tune | R4 | to do |
| W10-W11 | Evaluation and comparison (macro-F1, confusion matrices) | R5 | to do |
| W11 | Final report, code and README | D2 | to do |
| after W11 | Viva and peer assessment | D3, D4 | to do |

---

## MoSCoW Priorities
- **Must:** clean data, 3+ classic models and an MLP, macro-F1 evaluation, report and code
- **Should:** class imbalance handling, feature selection, k-means, tuning
- **Could:** test on Dataset 3, demo
- **Won't:** image/CNN models, clinical deployment

---

## Installation
### Requirements
> TODO: libraries

### Setup steps
> TODO: clone and install

---

## Data Preparation
### How to run
> TODO: notebook commands

### Pipeline steps
> TODO: cleaning, encoding, scaling

---

## Requirements and Results
### R2, R3, R4
> TODO: inputs, outputs, link

### Results
> TODO: table and figure
