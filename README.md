# Reproducibility-Project

This project is Group 45's take of the mandatory assignment part of the course "Deep Learning (CS4240)" from TU Delft's CS Masters' program.
* Albert Solà Roca
* Theodoros Veneti
* Ronan Hochart

We opted to (try and) reproduce the results from Maurizio Ferrari Dacrema (https://github.com/MaurizioFD/RecSys2019_DeepLearning_Evaluation) who in his turn tried to reproduce the findings from a number of different research from 
major conferences (such as SIGIR, KNN, RecSys and WWW). Specifically, their work succeeded in reproducing 7 out of the 18 papers selected. We tried to also reproduce these 7 papers
but also took a shot with the unreproduced ones, to see why they were deemed unreproducible.



*MCREC* : Results from the MCRec method presented at KDD '18.

*Dataet:Movie-Lens100k*
| Method     | PREC@10 | REC@10 | NDCG@10 |
|------------|---------|--------|---------|
| TopPopular | 0.1907  | 0.1180 | 0.1361  |
| UserKNN    | 0.2913  | 0.1802 | 0.2055  |
| ItemKNN    | 0.3327  | 0.2199 | 0.2603  |
| P<sup>3</sup>α| 0.2137  | 0.1585 | 0.1838  |
| RP<sup>3</sup>β| 0.2357  | 0.1684 | 0.1923  |
| MCRec      | 0.3077  | 0.2061 | 0.2363  |

*Our results*
| Method     | PREC@10 | REC@10 | NDCG@10 |
|------------|---------|--------|---------|
| TopPopular | 0.1907  | 0.1180 | 0.2184  |
| UserKNN    | 0.3370  | 0.2097 | 0.3917  |
| ItemKNN    | 0.3373  | 0.2235 | 0.4065  |
| P<sup>3</sup>α| 0.3361  | 0.2200 | 0.4073  |
| RP<sup>3</sup>β     | 0.3454  | 0.2230 | 0.4118  |
| MCRec      | 0.3047  | 0.2046 | 0.3617  |

*CVAE* : Results from the CVAE method presented at KDD '18.

*Dataset:CiteULike-a*
| Method        | REC@50 | REC@100 | REC@300 |
|---------------|--------|---------|---------|
| TopPopular    | 0.0044 | 0.0081  | 0.0258  |
| UserKNN       | 0.0683 | 0.1016  | 0.1685  |
| ItemKNN       | 0.0788 | 0.1153  | 0.1823  |
| P<sup>3</sup>α| 0.0788 | 0.1151  | 0.1784  |
| RP<sup>3</sup>β| 0.0811 | 0.1184  | 0.1799  |
| ItemKNN-CFCBF | 0.1837 | 0.2777  | 0.4486  |
| CVAE          | 0.0772 | 0.1548  | 0.3602  |

*Our results*
| Method        | REC@50 | REC@100 | REC@300 |
|---------------|--------|---------|---------|
| TopPopular    | 0.0253 | 0.0389  | 0.0704  |
| UserKNN       | 0.0026 | 0.0053  | 0.0154  |
| ItemKNN       | 0.0026 | 0.0053  | 0.0154  |
| P<sup>3</sup>α| 0.0026 | 0.0053  | 0.0154  |
| RP<sup>3</sup>β| 0.0026 | 0.0053  | 0.0154  |
| ItemKNN-CFCBF | 0.0607 | 0.0634  | 0.0730  |
| CVAE          | 0.0779 | 0.1192  | 0.2202  |

*NEUMF* : Results from the NeuMF method presented at WWW '17.

*Dataset:Pinterest*
| Method        | HR@5   | NDCG@5 | HR@10  | NDCG@10 |
|---------------|--------|--------|--------|---------|
| TopPopular    | 0.1663 | 0.1065 | 0.2744 | 0.1412  |
| UserKNN       | 0.7001 | 0.5033 | 0.8610 | 0.5557  |
| ItemKNN       | 0.7100 | 0.5092 | 0.8744 | 0.5629  |
| P<sup>3</sup>α| 0.7008 | 0.5018 | 0.8667 | 0.5559  |
| RP<sup>3</sup>β| 0.7105 | 0.5116 | 0.8740 | 0.5650  |
| NeuMF         | 0.7024 | 0.4983 | 0.8719 | 0.5536  |

*Our results*
| Method        | HR@5   | NDCG@5 | HR@10  | NDCG@10 |
|---------------|--------|--------|--------|---------|
| TopPopular    | 0.1663 | 0.1065 | 0.2744 | 0.1412  |
| UserKNN       | 0.7001 | 0.5033 | 0.8610 | 0.5557  |
| ItemKNN       | 0.7100 | 0.5092 | 0.8744 | 0.5629  |
| P<sup>3</sup>α| 0.7008 | 0.5018 | 0.8667 | 0.5559  |
| RP<sup>3</sup>β| 0.7105 | 0.5116 | 0.8740 | 0.5650  |
| NeuMF         | 0.7077 | 0.5023 | 0.8757 | 0.5572  |

*Dataset:MovieLens-1m*
| Method     | HR@5   | NDCG@5 | HR@10  | NDCG@10 |
|------------|--------|--------|--------|---------|
| TopPopular | 0.3043 | 0.2062 | 0.4531 | 0.2542  |
| UserKNN    | 0.4916 | 0.3328 | 0.6705 | 0.3908  |
| ItemKNN    | 0.4829 | 0.3328 | 0.6596 | 0.3900  |
| P<sup>3</sup>α| 0.4811 | 0.3331 | 0.6464 | 0.3867  |
| RP<sup>3</sup>β| 0.4922 | 0.3409 | 0.6715 | 0.3867  |
| NeuMF      | 0.5486 | 0.3840 | 0.7120 | 0.4369  |
| SLIM       | 0.5589 | 0.3961 | 0.7161 | 0.4470  |

*Our results*
| Method     | HR@5   | NDCG@5 | HR@10  | NDCG@10 |
|------------|--------|--------|--------|---------|
| TopPopular | 0.3043 | 0.2062 | 0.4531 | 0.2542  |
| UserKNN    | 0.4916 | 0.3328 | 0.6705 | 0.3908  |
| ItemKNN    | 0.4829 | 0.3328 | 0.6596 | 0.3900  |
| P<sup>3</sup>α| 0.4811 | 0.3331 | 0.6464 | 0.3867  |
| RP<sup>3</sup>β| 0.4922 | 0.3409 | 0.6715 | 0.3867  |
| NeuMF      | 0.5486 | 0.3840 | 0.7120 | 0.4369  |
| SLIM       | 0.5399 | 0.3745 | 0.7096 | 0.4296  |

*SPECTRALCF*: Results from SpectralCF method presented at RecSys '18.

*Dataset:MovieLens-1m*

*Our results*

*MVAE* : Results from the Mult-VAE method presented at WWW '18.

*Dataset:Netflix*

*Our results*

*CDL* : Results from the CDL method presented at KDD '15.


*CMN* : Results from the CMN method presented at SIGIR '18.

*Dataset:CiteUlike-a*
| Method     | HR@5   | NDCG@5 | HR@10  | NDCG@10 |
|------------|--------|--------|--------|---------|
| TopPopular | 0.1803 | 0.1220 | 0.2783 | 0.1535  |
| UserKNN    | 0.8213 | 0.7033 | 0.8935 | 0.7268  |
| ItemKNN    | 0.8116 | 0.6939 | 0.8878 | 0.7187  |
| P<sup>3</sup>α| 0.8202 | 0.7061 | 0.8901 | 0.7289  |
| RP<sup>3</sup>β| 0.8226 | 0.7114 | 0.8941 | 0.7347  |
| CMN        | 0.8069 | 0.6666 | 0.8910 | 0.6942  |


*Dataset:Pinterest*
| Method     | HR@5   | NDCG@5 | HR@10  | NDCG@10 |
|------------|--------|--------|--------|---------|
| TopPopular | 0.1668 | 0.1066 | 0.2745 | 0.1411  |
| UserKNN    | 0.6886 | 0.4936 | 0.8527 | 0.5470  |
| ItemKNN    | 0.6966 | 0.4994 | 0.8647 | 0.5542  |
| P<sup>3</sup>α| 0.6871 | 0.4935 | 0.8449 | 0.5450  |
| RP<sup>3</sup>β| 0.7018 | 0.5041 | 0.8644 | 0.5571  |
| CMN        | 0.6872 | 0.4883 | 0.8549 | 0.5430  |

*Dataset:Epinions*
| Method     | HR@5   | NDCG@5 | HR@10  | NDCG@10 |
|------------|--------|--------|--------|---------|
| TopPopular | 0.5429 | 0.4153 | 0.6644 | 0.4547  |
| UserKNN    | 0.3506 | 0.2983 | 0.3922 | 0.3117  |
| ItemKNN    | 0.3821 | 0.3165 | 0.4372 | 0.3343  |
| P<sup>3</sup>α| 0.3510 | 0.2989 | 0.3891 | 0.3112  |
| RP<sup>3</sup>β| 0.3511 | 0.2980 | 0.3892 | 0.3103  |
| CMN        | 0.4195 | 0.3346 | 0.4953 | 0.3592  |


*Extension ConvMF* : Results attempting to reproduce the paper by Donghyun Kim et al.

*Dataset:MovieLens1M*
| Method     | RMSE   |
|------------|--------|
| PMF | 0.8971 |
| ConvMF    | 0.8531 |
| ConvMF+    | 0.8549 |

*Our results*
| Method     | RMSE   |
|------------|--------|
| PMF | 0.8731 |
| ConvMF    | 0.8569 |
| ConvMF+    | 0.8570 |

*Dataset:MovieLens10M*
| Method     | RMSE   |
|------------|--------|
| PMF | 0.8311 |
| ConvMF    | 0.7958 |
| ConvMF+    | 0.7958 |

*Our results*
| Method     | RMSE   |
|------------|--------|
| PMF | 0.8668 |
| ConvMF    | 0.7889 |
| ConvMF+    | 0.7863 |
