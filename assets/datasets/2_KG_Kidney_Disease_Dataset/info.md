# Information About Dataset

## Characteristics:

DATASET OVERVIEW
Instances (rows):            20538
Columns:                     43
Features (excl. target):     42
Valid instances (no NaN):    20538 (100.00%)
Instances with any NaN:      0
Duplicate rows:              0
Memory:                      20748.1 KB
Features per instance ratio: 0.0020


COLUMN TYPES AND CLASSES
                                                             type  unique  missing  missing_%                                                           classes
Age of the patient                              numeric (integer)      86        0        0.0                                                                 -
Blood pressure (mm/Hg)                          numeric (integer)     101        0        0.0                                                                 -
Specific gravity of urine                         numeric (float)      21        0        0.0                                                                 -
Albumin in urine                                numeric (integer)       6        0        0.0                                                [0, 1, 2, 3, 4, 5]
Sugar in urine                                  numeric (integer)       6        0        0.0                                                [0, 1, 2, 3, 4, 5]
Red blood cells in urine                     categorical (string)       2        0        0.0                                                [abnormal, normal]
Pus cells in urine                           categorical (string)       2        0        0.0                                                [abnormal, normal]
Pus cell clumps in urine                     categorical (string)       2        0        0.0                                            [not present, present]
Bacteria in urine                            categorical (string)       2        0        0.0                                            [not present, present]
Random blood glucose level (mg/dl)              numeric (integer)     431        0        0.0                                                                 -
Blood urea (mg/dl)                                numeric (float)   20538        0        0.0                                                                 -
Serum creatinine (mg/dl)                          numeric (float)    1451        0        0.0                                                                 -
Sodium level (mEq/L)                              numeric (float)   20538        0        0.0                                                                 -
Potassium level (mEq/L)                           numeric (float)   20538        0        0.0                                                                 -
Hemoglobin level (gms)                            numeric (float)     121        0        0.0                                                                 -
Packed cell volume (%)                          numeric (integer)      36        0        0.0                                                                 -
White blood cell count (cells/cumm)             numeric (integer)    9784        0        0.0                                                                 -
Red blood cell count (millions/cumm)              numeric (float)      36        0        0.0                                                                 -
Hypertension (yes/no)                        categorical (string)       2        0        0.0                                                         [no, yes]
Diabetes mellitus (yes/no)                   categorical (string)       2        0        0.0                                                         [no, yes]
Coronary artery disease (yes/no)             categorical (string)       2        0        0.0                                                         [no, yes]
Appetite (good/poor)                         categorical (string)       2        0        0.0                                                      [good, poor]
Pedal edema (yes/no)                         categorical (string)       2        0        0.0                                                         [no, yes]...

categorical (string)    15
numeric (integer)       11

Constant columns: none


TARGET: Target
Task:                  classification
Number of classes:     5
Class values:          ['High_Risk', 'Low_Risk', 'Moderate_Risk', 'No_Disease', 'Severe_Disease']
                count      %
Target
No_Disease      16432  80.01
Low_Risk         2054  10.00
Moderate_Risk     821   4.00
High_Risk         821   4.00
Severe_Disease    410   2.00
Imbalance ratio (max/min): 40.08
Majority-class baseline:   80.01%


NUMERIC FEATURE STATS
                                                  min        max      mean       std   skew
Age of the patient                              5.000     90.000    47.478    24.942  0.008
Blood pressure (mm/Hg)                         80.000    180.000   130.352    29.064 -0.020
Specific gravity of urine                       1.005      1.025     1.015     0.006 -0.004
Albumin in urine                                0.000      5.000     2.501     1.697  0.001
Sugar in urine                                  0.000      5.000     2.495     1.701 -0.002
Random blood glucose level (mg/dl)             70.000    500.000   284.630   124.633  0.002
Blood urea (mg/dl)                              7.002    199.994   104.094    55.726 -0.015
Serum creatinine (mg/dl)                        0.500     15.000     7.782     4.180 -0.005
Sodium level (mEq/L)                          120.001    150.000   135.077     8.651 -0.010
Potassium level (mEq/L)                         3.500      6.500     4.992     0.871  0.014
Hemoglobin level (gms)                          6.000     18.000    11.958     3.450  0.014
Packed cell volume (%)                         20.000     55.000    37.499    10.414 -0.002
White blood cell count (cells/cumm)          3000.000  15000.000  9033.067  3481.774 -0.009
Red blood cell count (millions/cumm)            2.500      6.000     4.245     1.011 -0.000
Estimated Glomerular Filtration Rate (eGFR)     5.000    120.000    62.231    33.353  0.003
Urine protein-to-creatinine ratio               0.100      4.500     2.280     1.272  0.014
Urine output (ml/day)                         300.000   3000.000  1653.683   776.214  0.009
Serum albumin level                             2.000      4.500     3.256     0.722 -0.006
Cholesterol level                             100.000    300.000   200.236    57.863  0.000
Parathyroid hormone (PTH) level                10.000     70.000    40.265    17.310 -0.018
Serum calcium level                             7.500     10.500     9.002     0.867  0.004
Serum phosphate level                           2.500      6.000     4.241     1.007  0.012
Body Mass Index (BMI)                          15.000     40.000    27.544     7.221 -0.003
Duration of diabetes mellitus (years)           0.000     30.000    14.918     8.964  0.009
Duration of hypertension (years)                0.000     30.000    14.947     8.945 -0.004
Cystatin C level                                0.500      3.000     1.749     0.719 -0.001
C-reactive protein (CRP) level                  0.100     10.000     5.062     2.853 -0.011
Interleukin-6 (IL-6) level                      0.500     15.000     7.703     4.192  0.009

- Source : https://www.kaggle.com/datasets/amanik000/kidney-disease-dataset

## Usage
