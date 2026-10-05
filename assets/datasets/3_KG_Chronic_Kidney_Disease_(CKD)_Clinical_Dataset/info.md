# Information About Dataset

## Characteristics:

DATASET OVERVIEW
Instances (rows):            21000
Columns:                     36
Features (excl. target):     35
Valid instances (no NaN):    21000 (100.00%)
Instances with any NaN:      0
Duplicate rows:              0
Memory:                      10784.0 KB
Features per instance ratio: 0.0017

COLUMN TYPES AND CLASSES
                                          type  unique  missing  missing_%                                                                                                         classes
Target                    categorical (string)       5        0        0.0  [Healthy Kidney, Kidney Failure (Stage 5), Mild CKD (Stage 1–2), Moderate CKD (Stage 3), Severe CKD (Stage 4)]
Age                          numeric (integer)      65        0        0.0                                                                                                               -
Gender                        numeric (binary)       2        0        0.0                                                                                                          [0, 1]
BMI                          numeric (integer)      17        0        0.0                                                                                                               -
Systolic_BP                  numeric (integer)     100        0        0.0                                                                                                               -
Diastolic_BP                 numeric (integer)      60        0        0.0                                                                                                               -
Heart_Rate                   numeric (integer)      50        0        0.0                                                                                                               -
Serum_Creatinine             numeric (integer)      10        0        0.0                                                                                  [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
Blood_Urea_Nitrogen          numeric (integer)     143        0        0.0                                                                                                               -
eGFR                         numeric (integer)     115        0        0.0                                                                                                               -
Urine_Albumin                numeric (integer)     776        0        0.0                                                                                                               -
Urine_Protein                numeric (integer)     473        0        0.0                                                                                                               -
Albumin_Creatinine_Ratio     numeric (integer)     888        0        0.0                                                                                                               -
Urine_Specific_Gravity         numeric (float)   21000        0        0.0                                                                                                               -
Sodium                       numeric (integer)      10        0        0.0                                                              [135, 136, 137, 138, 139, 140, 141, 142, 143, 144]
Potassium                    numeric (integer)       6        0        0.0                                                                                              [3, 4, 5, 6, 7, 8]
Calcium                      numeric (integer)       3        0        0.0                                                                                                      [10, 8, 9]
Phosphorus                   numeric (integer)       7        0        0.0                                                                                           [2, 3, 4, 5, 6, 7, 8]
Chloride                     numeric (integer)      14        0        0.0                                                                                                               -
Bicarbonate                  numeric (integer)      18        0        0.0                                                                                                               -
Hemoglobin                   numeric (integer)      12        0        0.0                                                                                                               -
RBC_Count                      numeric (float)   21000        0        0.0                                                                                                               -
WBC_Count                    numeric (integer)    6645        0        0.0                                                                                                               -...

numeric (float)          4
numeric (binary)         1

TARGET: Target
Task:                  classification
Number of classes:     5
Class values:          ['Healthy Kidney', 'Kidney Failure (Stage 5)', 'Mild CKD (Stage 1–2)', 'Moderate CKD (Stage 3)', 'Severe CKD (Stage 4)']
                          count      %
Target
Healthy Kidney            15744  74.97
Mild CKD (Stage 1–2)       2491  11.86
Moderate CKD (Stage 3)     1489   7.09
Severe CKD (Stage 4)        856   4.08
Kidney Failure (Stage 5)    420   2.00
Imbalance ratio (max/min): 37.49
Majority-class baseline:   74.97%

NUMERIC FEATURE STATS
                                 min        max        mean        std   skew
Age                           20.000      84.00      51.952     18.796 -0.000
Gender                         0.000       1.00       0.501      0.500 -0.002
BMI                           18.000      34.00      25.978      4.890  0.001
Systolic_BP                   90.000     189.00     113.498     19.152  1.320
Diastolic_BP                  60.000     119.00      75.281     12.107  1.131
Heart_Rate                    60.000     109.00      84.281     14.388  0.020
Serum_Creatinine               0.000       9.00       0.630      1.482  3.145
Blood_Urea_Nitrogen            7.000     149.00      21.682     20.800  3.033
eGFR                           5.000     119.00      91.426     26.787 -1.555
Urine_Albumin                  0.000     999.00      59.987    136.149  3.732
Urine_Protein                  0.000     499.00      31.221     73.192  3.683
Albumin_Creatinine_Ratio       0.000    1199.00      68.930    155.758  4.097
Urine_Specific_Gravity         1.005       1.03       1.017      0.007 -0.003
Sodium                       135.000     144.00     139.492      2.872  0.001
Potassium                      3.000       8.00       3.720      0.827  1.834
Calcium                        8.000      10.00       9.004      0.817 -0.007
Phosphorus                     2.000       8.00       2.970      1.102  1.702
Chloride                      96.000     109.00     102.489      4.044  0.004
Bicarbonate                   10.000      27.00      23.286      2.949 -1.213
Hemoglobin                     5.000      16.00      13.449      2.319 -1.289
RBC_Count                      4.000       6.00       4.998      0.578 -0.002
WBC_Count                   4000.000   10999.00    7493.323   2019.807 -0.003
Platelet_Count            150022.000  449942.00  300422.552  86546.236 -0.012
Packed_Cell_Volume            20.000      49.00      42.167      5.497 -1.306
Blood_Glucose_Random          70.000     199.00     134.331     37.624  0.006
Fasting_Glucose               70.000     129.00      99.474     17.301 -0.004
HbA1c                          4.001      10.00       6.998      1.737 -0.003
Cholesterol                  150.000     279.00     214.412     37.452  0.003
Triglycerides                100.000     299.00     199.512     58.168  0.000
Serum_Albumin                  1.000       4.00       3.598      0.764 -1.756
Total_Protein                  5.000       8.00       6.508      0.865 -0.012

## Usage

- Source : https://www.kaggle.com/datasets/priyankabarik/chronic-kidney-disease-ckd-clinical-dataset
