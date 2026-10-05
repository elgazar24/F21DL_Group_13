# Information About Dataset

## Characteristics:

DATASET OVERVIEW
Instances (rows):            988
Columns:                     26
Features (excl. target):     25
Valid instances (no NaN):    988 (100.00%)
Instances with any NaN:      0
Duplicate rows:              0
Memory:                      200.8 KB
Features per instance ratio: 0.0253

                      type  unique  missing  missing_%          classes
Sl. No.  numeric (integer)     988        0        0.0                -
Age      numeric (integer)      60        0        0.0                -
Bp       numeric (integer)     110        0        0.0                -
Sg         numeric (float)       5        0        0.0                -
Al       numeric (integer)       5        0        0.0  [0, 1, 2, 3, 4]
Su       numeric (integer)       5        0        0.0  [0, 1, 2, 3, 4]
Rbc       numeric (binary)       2        0        0.0           [0, 1]
Pc        numeric (binary)       2        0        0.0           [0, 1]
Pcc       numeric (binary)       2        0        0.0           [0, 1]
Ba        numeric (binary)       2        0        0.0           [0, 1]
Bgr      numeric (integer)     313        0        0.0                -
Bu       numeric (integer)     188        0        0.0                -
Sc         numeric (float)     725        0        0.0                -
Sod      numeric (integer)      20        0        0.0                -
Pot        numeric (float)     288        0        0.0                -
Hemo       numeric (float)     101        0        0.0                -
Pcv      numeric (integer)      35        0        0.0                -
Wbcc     numeric (integer)     948        0        0.0                -
Rbcc       numeric (float)      26        0        0.0                -
Htn       numeric (binary)       2        0        0.0           [0, 1]
Dm        numeric (binary)       2        0        0.0           [0, 1]
Cad       numeric (binary)       2        0        0.0           [0, 1]
Appet     numeric (binary)       2        0        0.0           [0, 1]...

numeric (integer)    10
numeric (float)       5

TARGET: Class
Task:                  classification
Number of classes:     2
Class values:          [0, 1]
       count      %
Class
1        507  51.32
0        481  48.68
Imbalance ratio (max/min): 1.05
Majority-class baseline:   51.32%

NUMERIC FEATURE STATS
              min        max      mean       std   skew
Sl. No.     1.000    988.000   494.500   285.355  0.000
Age        20.000     79.000    50.270    17.336 -0.043
Bp         70.000    179.000   123.756    32.193  0.042
Sg          1.005      1.025     1.015     0.007 -0.047
Al          0.000      4.000     2.030     1.419 -0.064
Su          0.000      4.000     2.000     1.420  0.002
Rbc         0.000      1.000     0.515     0.500 -0.061
Pc          0.000      1.000     0.511     0.500 -0.045
Pcc         0.000      1.000     0.478     0.500  0.089
Ba          0.000      1.000     0.524     0.500 -0.097
Bgr        70.000    399.000   232.094    97.014  0.053
Bu         10.000    199.000   104.243    52.957 -0.012
Sc          0.500     14.980     7.536     4.142  0.065
Sod       130.000    149.000   139.721     5.717 -0.024
Pot         3.510      6.500     4.970     0.853  0.005
Hemo        7.000     17.000    12.078     2.858 -0.048
Pcv        20.000     54.000    36.722     9.879  0.031
Wbcc     4012.000  14987.000  9579.932  3156.570 -0.032
Rbcc        3.500      6.000     4.734     0.734  0.055
Htn         0.000      1.000     0.529     0.499 -0.118
Dm          0.000      1.000     0.491     0.500  0.036
Cad         0.000      1.000     0.499     0.500  0.004
Appet       0.000      1.000     0.504     0.500 -0.016
Pe          0.000      1.000     0.486     0.500  0.057
Ane         0.000      1.000     0.518     0.500 -0.073
Class       0.000      1.000     0.513     0.500 -0.053

- Source : https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/MB1LES
  , https://pmc.ncbi.nlm.nih.gov/articles/PMC13092092/#_ad93_

## Usage
