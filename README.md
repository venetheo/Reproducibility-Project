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
| RP<sup>3</sup>β| 0.3454  | 0.2230 | 0.4118  |
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
| TopPopular    | 0.1665 | 0.1064 | 0.2740 | 0.1409  |
| UserKNN       | 0.7042 | 0.5051 | 0.8656 | 0.5577  |
| ItemKNN       | 0.7126 | 0.5118 | 0.8778 | 0.5656  |
| P<sup>3</sup>α| 0.7016 | 0.5018 | 0.8687 | 0.5563  |
| RP<sup>3</sup>β| 0.7139 | 0.5141 | 0.8775 | 0.5674  |
| NeuMF         | 0.7046 | 0.4994 | 0.8766 | 0.5556  |

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
| TopPopular | 0.3048 | 0.2064 | 0.4533 | 0.2542  |
| UserKNN    | 0.4921 | 0.3319 | 0.6714 | 0.3899  |
| ItemKNN    | 0.4914 | 0.3377 | 0.6624 | 0.3931  |
| P<sup>3</sup>α| 0.4687 | 0.3232 | 0.6430 | 0.3796  |
| RP<sup>3</sup>β| 0.4947 | 0.3418 | 0.6694 | 0.3985  |
| NeuMF      | 0.5406 | 0.3807 | 0.7098 | 0.4356  |
| SLIM       | 0.5560 | 0.3939 | 0.7136 | 0.4450  |

*SPECTRALCF*: Results from SpectralCF method presented at RecSys '18.

*Dataset:MovieLens-1m*
| Method     | REC@20 | MAP@20 | REC@60 | MAP@60 | REC@100 | MAP@100 |
|------------|--------|--------|--------|--------|---------|---------|
| TopPopular | 0.1853 | 0.0576 | 0.3335 | 0.0659 | 0.4244  | 0.0696  |
| UserKNN CF | 0.2881 | 0.1106 | 0.4780 | 0.1238 | 0.5790  | 0.1290  |
| ItemKNN CF | 0.2819 | 0.1059 | 0.4712 | 0.1190 | 0.5737  | 0.1243  |
| P^3α       | 0.2853 | 0.1051 | 0.4808 | 0.1195 | 0.5760  | 0.1248  |
| RP^3β      | 0.2910 | 0.1088 | 0.4882 | 0.1233 | 0.5884  | 0.1288  |
| SpectralCF | 0.1843 | 0.0539 | 0.3274 | 0.0618 | 0.4254  | 0.0656  |

*Our results*
| Method     | REC@20 | MAP@20 | REC@60 | MAP@60 | REC@100 | MAP@100 |
|------------|--------|--------|--------|--------|---------|---------|
| TopPopular | 0.1941 | 0.0611 | 0.3399 | 0.0693 | 0.4299  | 0.0729  |
| UserKNN CF | 0.3013 | 0.1219 | 0.4870 | 0.1349 | 0.5851  | 0.1400  |
| ItemKNN CF | 0.2972 | 0.1180 | 0.4864 | 0.1309 | 0.5847  | 0.1361  |
| P^3α       | 0.3025 | 0.1174 | 0.4981 | 0.1316 | 0.5935  | 0.1371  |
| RP^3β      | 0.3101 | 0.1225 | 0.5071 | 0.1369 | 0.6058  | 0.1424  |
| SpectralCF | 0.1619 | 0.0488 | 0.3132 | 0.0567 | 0.4037  | 0.0598  |

*MVAE* : Results from the Mult-VAE method presented at WWW '18.

*Dataset:Netflix*
| Method     | REC@20 | NDCG@20 | REC@50 | NDCG@50 | REC@100 | NDCG@100 |
|------------|--------|---------|--------|---------|---------|----------|
| TopPopular | 0.0782 |         | 0.1643 |         |         | 0.1570   |
| ItemKNN CF | 0.2088 |         | 0.3386 |         |         | 0.3086   |
| P^3α       | 0.1977 |         | 0.3346 |         |         | 0.2967   |
| RP^3β      | 0.2196 |         | 0.3560 |         |         | 0.3246   |
| SLIM       | 0.2551 | 0.2473  | 0.3995 | 0.3196  | 0.5289  | 0.3745   |
| Mul-VAE    | 0.2626 | 0.2448  | 0.4138 | 0.3192  | 0.5476  | 0.3756   |

*Our results*
| Method     | REC@20 | NDCG@20 | REC@50 | NDCG@50 | REC@100 | NDCG@100 |
|------------|--------|---------|--------|---------|---------|----------|
| TopPopular | 0.0782 |         | 0.1643 |         |         | 0.1570   |
| ItemKNN CF | 0.2088 |         | 0.3386 |         |         | 0.3086   |
| P^3α       | 0.1977 |         | 0.3346 |         |         | 0.2967   |
| RP^3β      | 0.2196 |         | 0.3560 |         |         | 0.3246   |
| SLIM       | 0.2551 | 0.2473  | 0.3995 | 0.3196  | 0.5289  | 0.3745   |
| Mul-VAE    | 0.2641 | 0.3163  | 0.4174 | 0.3417  | 0.5508  | 0.3829   |

*CDL* : Results from the CDL method presented at KDD '15.

*Dataset:CiteULike-a*
| Method        | REC@50 | REC@100 | REC@300 |
|---------------|--------|---------|---------|
| TopPopular    | 0.0038 | 0.0073  | 0.0258  |
| UserKNN       | 0.0685 | 0.1028  | 0.1710  |
| ItemKNN       | 0.0846 | 0.1213  | 0.1861  |
| P^3α          | 0.0718 | 0.1079  | 0.1777  |
| RP^3β         | 0.0800 | 0.1167  | 0.1815  |
| ItemKNN-CBF   | 0.2135 | 0.3038  | 0.4707  |
| ItemKNN-CFCBF | 0.1945 | 0.2896  | 0.4620  |
| Mul-VAE       | 0.0543 | 0.1035  | 0.2627  |


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


*Extension ConvMF* : Results attempting to reproduce the paper by Donghyun Kim et al (One of the papers, the work by Ferrari could not reproduce).

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
