# Information About Dataset (UCI Chronic Kidney Disease Dataset)

## Characteristics:

```
DATASET OVERVIEW
Instances (rows):            400
Columns:                     25
Features (excl. target):     24
Valid instances (no NaN):    158 (39.50%)
Instances with any NaN:      242
Duplicate rows:              0
Memory:                      269.2 KB
Features per instance ratio: 0.0600

COLUMN TYPES AND CLASSES
                       type  unique  missing  missing_%                classes
age         numeric (float)      76        9       2.25                      -
bp          numeric (float)      10       12       3.00                      -
sg          numeric (float)       5       47      11.75                      -
al          numeric (float)       6       46      11.50                      -
su          numeric (float)       6       49      12.25                      -
rbc    categorical (string)       2      152      38.00     [abnormal, normal]
pc     categorical (string)       2       65      16.25     [abnormal, normal]
pcc    categorical (string)       2        4       1.00  [notpresent, present]
ba     categorical (string)       2        4       1.00  [notpresent, present]
bgr         numeric (float)     146       44      11.00                      -
bu          numeric (float)     118       19       4.75                      -
sc          numeric (float)      84       17       4.25                      -
sod         numeric (float)      34       87      21.75                      -
pot         numeric (float)      40       88      22.00                      -
hemo        numeric (float)     115       52      13.00                      -
pcv         numeric (float)      42       71      17.75                      -
wbcc        numeric (float)      89      106      26.50                      -
rbcc        numeric (float)      45      131      32.75                      -
htn    categorical (string)       2        2       0.50              [no, yes]
dm     categorical (string)       3        2       0.50        [ yes, no, yes]
cad    categorical (string)       2        2       0.50              [no, yes]
appet  categorical (string)       2        1       0.25           [good, poor]
pe     categorical (string)       2        1       0.25              [no, yes]
ane    categorical (string)       2        1       0.25              [no, yes]
class  categorical (string)       2        0       0.00          [ckd, notckd]

TYPE COUNTS
type
numeric (float)         14
categorical (string)    11
Constant columns: none

TARGET: class
Task:                  classification
Number of classes:     2
Class values:          ['ckd', 'notckd']
        count     %
class              
ckd       250  62.5
notckd    150  37.5
Imbalance ratio (max/min): 1.67
Majority-class baseline:   62.50%

NUMERIC FEATURE STATS
           min        max      mean       std    skew
age      2.000     90.000    51.483    17.170  -0.668
bp      50.000    180.000    76.469    13.684   1.605
sg       1.005      1.025     1.017     0.006  -0.172
al       0.000      5.000     1.017     1.353   0.998
su       0.000      5.000     0.450     1.099   2.464
bgr     22.000    490.000   148.037    79.282   2.011
bu       1.500    391.000    57.426    50.503   2.634
sc       0.400     76.000     3.072     5.741   7.510
sod      4.500    163.000   137.529    10.409  -6.997
pot      2.500     47.000     4.627     3.194  11.583
hemo     3.100     17.800    12.526     2.913  -0.335
pcv      9.000     54.000    38.884     8.990  -0.434
wbcc  2200.000  26400.000  8406.122  2944.474   1.622
rbcc     2.100      8.000     4.707     1.025  -0.183
```

## Source

- https://archive.ics.uci.edu/dataset/336/chronic+kidney+disease

## Usage

*Allowed only with Citation*

L. Rubini, P. Soundarapandian, and P. Eswaran. "Chronic Kidney Disease," UCI Machine Learning Repository, 2015. https://doi.org/10.24432/C5G020
