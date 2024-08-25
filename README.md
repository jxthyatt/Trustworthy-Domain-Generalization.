# Trustworthy Domain Generalization (TruDG)
Official repository for the submitted paper “Both Multi-silo and Multi-modality Matter: Trustworthy Domain Generalization via Personalized Federated Learning and Language-driven Zero-shot Adaptation”. Previous version of Code is [here](https://github.com/jxthyatt/Trustworthy-Domain-Generalization). :rainbow: Final Code will be released after acceptance.

## Replicate Demo and Results
### Federated DG under Client Heterogeneity ( :herb::herb: TABLE I)
:rocket::rocket: We evaluate cross-client **personalization** under distribution heterogeneity in demo “from Photo-Art-Cartoon to  Sketch” ( :star: here model is performed on [PACS](https://datasets.activeloop.ai/docs/ml/datasets/pacs-dataset/) dataset). Please view more details in TABLE I.


| Method               | PFL            | Pub’Year        | P(Y)           | P(X)           | P(Y&#124;X)    | P(X,Y)         | Checkpoint file                                                          |
|----------------------|----------------|-----------------|----------------|----------------|----------------|----------------|--------------------------------------------------------------------------|
| FedAvg               | &#10007;       | AISTATS’17      | 76.66          | 68.18          | 58.44          | 65.73          | [Link](https://pan.baidu.com/s/1Fy9aB1tenAJBHwKcKZLMjw) (Code: f3kf)     |
| q-FFL                | &#10007;       | arXiv’19        | 11.76          | 13.75          | 14.50          | 15.45          | [Link](https://pan.baidu.com/s/1-x-g4N3PmN6Z_HN6Y7kPIA) (Code: a2bx)     |
| AFL                  | &#10007;       | ICML’19         | 74.83          | 69.91          | 47.08          | 59.62          | [Link](https://pan.baidu.com/s/1jZ57ItZGkktYfWHitp0gWw) (Code: q1by)     |
| FedProx              | &#10007;       | MLSys’20        | 71.19          | 66.88          | 62.12          | 60.27          | [Link](https://pan.baidu.com/s/13uALQVs0XRcyT-dcUQRlgw) (Code: mycg)     |
| Local                | &#10003;       | -               | 63.08          | 50.87          | 43.07          | 57.12          | [Link](https://pan.baidu.com/s/1ZMPyCFLUIDVHsOsIG3PobQ) (Code: 55pw)     |
| FedAvg+              | &#10003;       | arXiv’19        | 75.50          | 69.59          | 58.66          | 63.41          | [Link](https://pan.baidu.com/s/1t9hlB4ZplLWviz1vpxSkjg) (Code: 7utu)     |
| L2SGD                | &#10003;       | NeurIPS’20      | 63.41          | 49.35          | 44.91          | 53.93          | [Link](https://pan.baidu.com/s/17wppT4uBBjOS2sashM1H7Q) (Code: g3rj)     |
| pFedMe               | &#10003;       | NeurIPS’20      | 64.57          | 50.65          | 44.81          | 55.80          | [Link](https://pan.baidu.com/s/107fJ5kTp0QwJbDm2XUj_iQ) (Code: krt3)     |
| ClusteredFL          | &#10003;       | TNNLS’20        | 67.22          | 69.91          | 46.97          | 64.74          | [Link](https://pan.baidu.com/s/1mCjfDL4B7J7lgfNHFmejHw) (Code: ab18)     |
| FedEM                | &#10003;       | NeurIPS’21      | 74.17          | 67.32          | 52.06          | 66.06          | [Link](https://pan.baidu.com/s/1Hh3Nz_x58m_eDzUnLalQXA) (Code: 1c3n)     |
| FedGMM               | &#10003;       | ICML’23         | 75.83          | 70.67          | 59.20          | 63.08          | [Link](https://pan.baidu.com/s/1rV5TyarmSLwxHlnJXMZ5_Q) (Code: mt6f)     |
| pFedMAP (ours)       | &#10003;       | TMM'24          | 76.99          | 70.89          | 76.62          | 68.05          | [Link](https://pan.baidu.com/s/1PuTTOWyt2_kXJbChN0_3nQ) (Code: ymrv)     |


:airplane::airplane: We evaluate out-of-client **generalization** under distribution heterogeneity in demo “from Photo-Art-Cartoon to  Sketch” ( :star: here model is performed on [PACS](https://datasets.activeloop.ai/docs/ml/datasets/pacs-dataset/) dataset). Please view more details in TABLE I.


| Method               | PFL            | Pub’Year        | P(Y)           | P(X)           | P(Y&#124;X)    | P(X,Y)         | Checkpoint file                                                          |
|----------------------|----------------|-----------------|----------------|----------------|----------------|----------------|--------------------------------------------------------------------------|
| FedAvg               | &#10007;       | AISTATS’17      | 73.90          | 72.89          | 24.89          | 41.73          | [Link](https://pan.baidu.com/s/1_XRltbnjGgXDyRSkCSUO2Q) (Code: xzgg)     |
| q-FFL                | &#10007;       | arXiv’19        | 10.66          | 11.11          | 12.89          | 14.69          | [Link](https://pan.baidu.com/s/1l05rrNaoyYng4_Jpw4s0Ag) (Code: h4w3)     |
| AFL                  | &#10007;       | ICML’19         | 74.45          | 70.22          | 14.67          | 15.91          | [Link](https://pan.baidu.com/s/1lYGyLIhNXN4SEXKwZloTFg) (Code: ch2z)     |
| FedProx              | &#10007;       | MLSys’20        | 70.96          | 67.11          | 24.00          | 21.88          | [Link](https://pan.baidu.com/s/1DCvnXvp3QZ_L4ArPZLODbg) (Code: 3y7g)     |
| Local                | &#10003;       | -               | 12.32          | 10.67          | 10.67          | 15.99          | [Link](https://pan.baidu.com/s/1aNgEK_kDZ7Vj6PoYWwxg1Q) (Code: ktg7)     |
| FedAvg+              | &#10003;       | arXiv’19        | 75.92          | 75.11          | 26.67          | 36.40          | [Link](https://pan.baidu.com/s/10dw-S9iq9nDEl9rave0w_g) (Code: 3j82)     |
| L2SGD                | &#10003;       | NeurIPS’20      | 65.99          | 60.00          | 28.89          | 25.03          | [Link](https://pan.baidu.com/s/1F18PVfaucQuMO5_SI8oqOA) (Code: 9ajt)     |
| pFedMe               | &#10003;       | NeurIPS’20      | 63.60          | 55.11          | 23.11          | 22.98          | [Link](https://pan.baidu.com/s/1JKE_ZmRAw-bNsvoGsecQBw) (Code: twae)     |
| ClusteredFL          | &#10003;       | TNNLS’20        | 64.52          | 9.33           | 9.78           | 20.04          | [Link](https://pan.baidu.com/s/14JERZzC4C0DjRXcKexsskA) (Code: j381)     |
| FedEM                | &#10003;       | NeurIPS’21      | 76.10          | 73.78          | 15.56          | 23.53          | [Link](https://pan.baidu.com/s/1qQ3N-Y4H-wx_8SgltmK9rQ) (Code: 2im6)     |
| FedGMM               | &#10003;       | ICML’23         | 76.29          | 74.22          | 29.33          | 35.29          | [Link](https://pan.baidu.com/s/1TSZafZe2TQYDgAzgILYD6w) (Code: thtz)     |
| pFedMAP (ours)       | &#10003;       | TMM'24          | 77.02          | 74.67          | 35.56          | 37.68          | [Link](https://pan.baidu.com/s/1kUu0qBWRCxxVN7cYyu69zw) (Code: jp4v)     |


:hotsprings: **Note:** PFL refers to personalized federated learning. Types of distribution heterogeneity include label distribution of P(Y), marginal distribution of P(X), conditional distribution of P(YIX), and joint distribution of P(X,Y).


### Federated DG for Facial Emotion Recognition ( :herb::herb: TABLE II)
:rocket::rocket: We evaluate cross-client **personalization** in “Leave-One-Domain-Out” experiments ( :star: here model is performed on [RAF-DB](http://www.whdeng.cn/raf/model1.html), [ExpW](https://mmlab.ie.cuhk.edu.hk/projects/socialrelation/index.html), and [FER2013](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data) datasets). Please view more details in TABLE II.


| Method               | PFL            | Pub’Year        | RAF-DB         | ExpW           | FER2013        | Avg.           | Checkpoint file                                                          |
|----------------------|----------------|-----------------|----------------|----------------|----------------|----------------|--------------------------------------------------------------------------|
| FedAvg               | &#10007;       | AISTATS’17      | 52.18          | 60.00          | 52.60          | 54.93          | [Link](https://pan.baidu.com/s/15aKaVOGQzRWYNpTtjjwPKw) (Code: g3cc)     |
| q-FFL                | &#10007;       | arXiv’19        | 14.35          | 14.25          | 10.76          | 13.12          | [Link](https://pan.baidu.com/s/1xtiKSf5SGcHHabRb8QCFIQ) (Code: n7vg)     |
| AFL                  | &#10007;       | ICML’19         | 44.02          | 51.05          | 47.39          | 47.49          | [Link](https://pan.baidu.com/s/19RhR0oAnwN_l-cn-45oeLA) (Code: 3w9h)     |
| FedProx              | &#10007;       | MLSys’20        | 42.25          | 50.48          | 44.43          | 45.72          | [Link](https://pan.baidu.com/s/1gjsHMkMW4utiW_QxvM68Vg) (Code: kwjs)     |
| Local                | &#10003;       | -               | 40.09          | 49.92          | 43.89          | 44.64          | [Link](https://pan.baidu.com/s/1oSU4oxzXGstjzFiQBcY89A) (Code: zw9f)     |
| FedAvg+              | &#10003;       | arXiv’19        | 52.67          | 59.21          | 52.21          | 54.70          | [Link](https://pan.baidu.com/s/1IbWXhW7e9L0b5FYczsGUaQ) (Code: bjyn)     |
| L2SGD                | &#10003;       | NeurIPS’20      | 35.82          | 42.17          | 40.06          | 39.35          | [Link](https://pan.baidu.com/s/1KDgKshhiXg8YHlRaM6OdYg) (Code: uiyt)     |
| pFedMe               | &#10003;       | NeurIPS’20      | 38.87          | 44.20          | 40.02          | 41.03          | [Link](https://pan.baidu.com/s/10tntPijYL4YSPVtzAP4l5w) (Code: c5vh)     |
| ClusteredFL          | &#10003;       | TNNLS’20        | 67.22          | 57.93          | 52.65          | 53.15          | [Link](https://pan.baidu.com/s/1NWgfMe7ecZFwwlvCA1b1EQ) (Code: us7q)     |
| FedEM                | &#10003;       | NeurIPS’21      | 51.08          | 58.59          | 53.91          | 54.53          | [Link](https://pan.baidu.com/s/1_fRvSakAt1rFoe2mog03DQ) (Code: vmqt)     |
| FedGMM               | &#10003;       | ICML’23         | 50.76          | 57.36          | 52.81          | 53.64          | [Link](https://pan.baidu.com/s/1NdkjCc8sr3DAraD4DaogIg) (Code: s2h6)     |
| pFedMAP (ours)       | &#10003;       | TMM'24          | 52.17          | 58.88          | 54.33          | 55.12          | [Link](https://pan.baidu.com/s/1ceVPCIUOJU6FiZte1uhkZw) (Code: fb9d)     |


:airplane::airplane: We evaluate out-of-client **generalization** in “Leave-One-Domain-Out” experiments ( :star: here model is performed on [RAF-DB](http://www.whdeng.cn/raf/model1.html), [ExpW](https://mmlab.ie.cuhk.edu.hk/projects/socialrelation/index.html), and [FER2013](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data) datasets). Please view more details in TABLE II.


| Method               | PFL            | Pub’Year        | RAF-DB         | ExpW           | FER2013        | Avg.           | Checkpoint file                                                          |
|----------------------|----------------|-----------------|----------------|----------------|----------------|----------------|--------------------------------------------------------------------------|
| FedAvg               | &#10007;       | AISTATS’17      | 30.07          | 21.58          | 28.52          | 26.72          | [Link](https://pan.baidu.com/s/1Hgi_1Q6u-n9ofutrTBm_dw) (Code: awqz)     |
| q-FFL                | &#10007;       | arXiv’19        | 11.62          | 13.49          | 13.05          | 12.72          | [Link](https://pan.baidu.com/s/1qpDrBw6nvz6DHeBAOODdZg) (Code: p26n)     |
| AFL                  | &#10007;       | ICML’19         | 26.49          | 12.17          | 17.73          | 18.80          | [Link](https://pan.baidu.com/s/1EtnN_z2wWfDQeSEuZvBkww) (Code: 64dh)     |
| FedProx              | &#10007;       | MLSys’20        | 28.86          | 19.26          | 15.37          | 21.16          | [Link](https://pan.baidu.com/s/1PlyTVG_DUlVzx726Pb2e2A) (Code: 8ewm)     |
| Local                | &#10003;       | -               | 15.64          | 15.31          | 14.55          | 15.17          | [Link](https://pan.baidu.com/s/1J6X_H4TFBiNy4wzjIV4jVw) (Code: 54d4)     |
| FedAvg+              | &#10003;       | arXiv’19        | 32.16          | 27.98          | 40.08          | 33.40          | [Link](https://pan.baidu.com/s/193tAanJODi9VGw-6twFrpQ) (Code: s4te)     |
| L2SGD                | &#10003;       | NeurIPS’20      | 25.09          | 21.96          | 27.94          | 25.00          | [Link](https://pan.baidu.com/s/1y67F9VcJ54sPDZqgsVo66w) (Code: hy8m)     |
| pFedMe               | &#10003;       | NeurIPS’20      | 25.57          | 39.02          | 27.65          | 30.75          | [Link](https://pan.baidu.com/s/1DrrEGyXaBg7P1D3dR2OUag) (Code: uk8d)     |
| ClusteredFL          | &#10003;       | TNNLS’20        | 14.14          | 13.93          | 15.22          | 14.43          | [Link](https://pan.baidu.com/s/1P_dtAyLxLfj2P1KRxdL-cA) (Code: tk6f)     |
| FedEM                | &#10003;       | NeurIPS’21      | 41.45          | 38.83          | 28.28          | 36.19          | [Link](https://pan.baidu.com/s/1col7Wfs2q6vKNY7VpO1ZeA) (Code: 6d74)     |
| FedGMM               | &#10003;       | ICML’23         | 38.31          | 44.54          | 35.89          | 39.58          | [Link](https://pan.baidu.com/s/1T0j-yHxSLEN-fyDpR4N5JA) (Code: yke7)     |
| pFedMAP (ours)       | &#10003;       | TMM'24          | 40.34          | 49.56          | 53.18          | 47.69          | [Link](https://pan.baidu.com/s/1NlQapxvEM4Y7ClU_Tw1SQw) (Code: h52c)     |


:hotsprings: **Note:** PFL refers to personalized federated learning. All methods for federated DG are deployed in Leave-One-Domain-Out experiments, e.g., the first column means choosing one domain (RAF-DB) to hold out as a target client while using others (FER2013 and ExpW) as source clients.


### Federated DG for General Object Classification ( :herb::herb: TABLE IV)
:rocket::rocket: We evaluate cross-client **personalization** in “Leave-One-Domain-Out” experiments ( :star: here model is performed on [PACS](https://datasets.activeloop.ai/docs/ml/datasets/pacs-dataset/) and [VLCS](https://drive.google.com/uc?id=1skwblH1_okBwxWxmRsp9_qi15hyPpxg8) datasets). Please view more details in TABLE IV.


| Method               | PFL            | Photo          | Art            | Cartoon        | Sketch         | Avg.           | Checkpoint file                                                          |
|----------------------|----------------|----------------|----------------|----------------|----------------|----------------|--------------------------------------------------------------------------|
| FedAvg               | &#10007;       | 68.88          | 73.56          | 63.42          | 65.73          | 67.90          | [Link](https://pan.baidu.com/s/13hpYaT1lmY-PZ5qjA8D8Hw) (Code: kpm1)     |
| q-FFL                | &#10007;       | 13.74          | 17.53          | 17.62          | 15.45          | 16.09          | [Link](https://pan.baidu.com/s/1j6m3f6CQKnjGQjq_hJV4AA) (Code: t26g)     |
| AFL                  | &#10007;       | 65.11          | 69.18          | 59.62          | 59.62          | 63.38          | [Link](https://pan.baidu.com/s/1CuelacLoa4uWHhDMAxGgcA) (Code: t579)     |
| FedProx              | &#10007;       | 60.61          | 65.10          | 58.54          | 60.27          | 61.13          | [Link](https://pan.baidu.com/s/1YJd98c6wndZ4YZTEEtpweg) (Code: nvas)     |
| Local                | &#10003;       | 66.99          | 76.56          | 53.12          | 57.12          | 63.45          | [Link](https://pan.baidu.com/s/14n2nwoOdsEtGi41JdJmCVQ) (Code: 4p2m)     |
| FedAvg+              | &#10003;       | 71.98          | 74.71          | 62.06          | 63.41          | 68.04          | [Link](https://pan.baidu.com/s/1JBEVJrYWchZ-zcrxy3Tocg) (Code: 4qm5)     |
| L2SGD                | &#10003;       | 65.59          | 73.25          | 51.22          | 53.93          | 61.00          | [Link](https://pan.baidu.com/s/16RQWIbr2RLSJ2ScMF5rPBg) (Code: weuz)     |
| pFedMe               | &#10003;       | 62.68          | 70.10          | 50.14          | 55.80          | 59.68          | [Link](https://pan.baidu.com/s/1sb8kvQCthcnyFAAv-oKjPA) (Code: 4bn5)     |
| ClusteredFL          | &#10003;       | 69.79          | 70.87          | 61.79          | 64.74          | 66.80          | [Link](https://pan.baidu.com/s/1lYinvDXpZ_AAp8VzbOB3HQ) (Code: vs7u)     |
| FedEM                | &#10003;       | 69.61          | 77.25          | 59.89          | 66.06          | 68.20          | [Link](https://pan.baidu.com/s/1r4GxP238BqTYdrDDiFy9bQ) (Code: y556)     |
| FedGMM               | &#10003;       | 72.22          | 80.09          | 63.14          | 64.07          | 69.88          | [Link](https://pan.baidu.com/s/1cC15SjxnqzmFvD87IUpCAw) (Code: zm3a)     |
| pFedMAP (ours)       | &#10003;       | 78.18          | 81.09          | 63.96          | 68.05          | 72.82          | [Link](https://pan.baidu.com/s/1LacuWVhlL5tpD5dG5E9fzw) (Code: exke)     |


:airplane::airplane: We evaluate out-of-client **generalization** in “Leave-One-Domain-Out” experiments ( :star: here model is performed on [PACS](https://datasets.activeloop.ai/docs/ml/datasets/pacs-dataset/) and [VLCS](https://drive.google.com/uc?id=1skwblH1_okBwxWxmRsp9_qi15hyPpxg8) datasets). Please view more details in TABLE IV.


| Method               | PFL            | Photo          | Art            | Cartoon        | Sketch         | Avg.           | Checkpoint file                                                          |
|----------------------|----------------|----------------|----------------|----------------|----------------|----------------|--------------------------------------------------------------------------|
| FedAvg               | &#10007;       | 50.00          | 52.08          | 34.95          | 41.73          | 44.69          | [Link](https://pan.baidu.com/s/1XXGtO-v2GRCUJAmPYPiliQ) (Code: ubty)     |
| q-FFL                | &#10007;       | 19.23          | 8.33           | 13.78          | 14.69          | 14.01          | [Link](https://pan.baidu.com/s/111A4F0qAkesNRPfFNSdjsQ) (Code: 764z)     |
| AFL                  | &#10007;       | 23.08          | 46.88          | 20.67          | 15.91          | 26.64          | [Link](https://pan.baidu.com/s/1THLNPxao0JVc8gmSUs9akQ) (Code: tsaj)     |
| FedProx              | &#10007;       | 26.92          | 44.79          | 28.37          | 21.88          | 30.49          | [Link](https://pan.baidu.com/s/1Iy1oCMisR5TUr6Q-w-xYnw) (Code: bjdm)     |
| Local                | &#10003;       | 26.92          | 12.50          | 18.34          | 15.99          | 18.44          | [Link](https://pan.baidu.com/s/1E11n2HkvRc6Zu_BlfPfD4A) (Code: sim3)     |
| FedAvg+              | &#10003;       | 46.15          | 60.42          | 50.91          | 36.40          | 48.47          | [Link](https://pan.baidu.com/s/1EU-2aQTJl_UQVzbBoc0u_w) (Code: hqs1)     |
| L2SGD                | &#10003;       | 26.92          | 31.25          | 22.09          | 25.03          | 26.32          | [Link](https://pan.baidu.com/s/1U0sbHocKmmm1FxPBCrZhOA) (Code: 9dbh)     |
| pFedMe               | &#10003;       | 19.23          | 37.50          | 22.80          | 22.98          | 25.63          | [Link](https://pan.baidu.com/s/1qzQcUd0jwM08KQtYox3mfw) (Code: 559w)     |
| ClusteredFL          | &#10003;       | 23.08          | 12.50          | 16.82          | 20.04          | 18.11          | [Link](https://pan.baidu.com/s/12AZ2KEeFQcTvAJr3iTxp1w) (Code: c5rk)     |
| FedEM                | &#10003;       | 57.69          | 61.46          | 27.96          | 23.53          | 42.66          | [Link](https://pan.baidu.com/s/1YKzNpLwn7dfJIq4TeXg1eQ) (Code: ujbb)     |
| FedGMM               | &#10003;       | 46.15          | 70.83          | 28.98          | 31.43          | 44.35          | [Link](https://pan.baidu.com/s/1zXXU40VhyE6ozel7tQOCgw) (Code: ayyd)     |
| pFedMAP (ours)       | &#10003;       | 50.00          | 72.92          | 36.58          | 37.68          | 49.30          | [Link](https://pan.baidu.com/s/1_8bgOcDpHZho0bSDk3Tfbg) (Code: y84y)     |


:hotsprings: **Note:** PFL refers to personalized federated learning. All methods for federated DG are deployed in Leave-One-Domain-Out experiments, e.g., the first column means choosing one domain (Photo) to hold out as a target client while using others (Art, Cartoon and Sketch) as source clients.


### Multimodal DG from Cityscapes to ACDC-Fog ( :foggy::foggy: TABLE V)
:rocket::rocket: We provide quantitative results and checkpoint files in demo “from [Cityscapes](https://www.cityscapes-dataset.com/) to [ACDC](https://acdc.vision.ee.ethz.ch/overview)” ( :star: here model is tested on ACDC-Fog dataset). Please view more details in TABLE V.


| Method                       | LST            | Pub’Year            | Source mIoU     | Target mIoU     | Gain                  | Checkpoint file                                                          |
|------------------------------|----------------|---------------------|-----------------|-----------------|-----------------------|--------------------------------------------------------------------------|
| AdaIN                        | &#10007;       | ICCV’17             | 50.3            | 44.9            | -5.4                  | [Link](https://pan.baidu.com/s/1sVbqQ8NeyYS2dDUc0exmkQ) (Code: 8bca)     |
| CIConv                       | &#10007;       | ICCV’21             | 58.3            | 56.7            | -1.6                  | [Link](https://pan.baidu.com/s/1ckj2X0jDu70jzpgowWytLQ) (Code: edpz)     |
| RobustNet                    | &#10007;       | CVPR’21             | 61.5            | 61.8            | 0.3                   | [Link](https://pan.baidu.com/s/1tbxJYOgj-ZmrAoMyaP7xjw) (Code: dv3a)     |
| SNR                          | &#10007;       | TMM’21              | 50.3            | 51.9            | 1.6                   | [Link](https://pan.baidu.com/s/1QhYIrumQtE6MJtF_eFgbSw) (Code: bc6j)     |
| WildNet                      | &#10007;       | CVPR’22             | 50.3            | 58.7            | 8.4                   | [Link]() (Code: vsfp)     |
| CLIPstyler (fast)            | &#10003;       | CVPR’22             | 50.3            | 51.6            | 1.3                   | [Link](https://pan.baidu.com/s/1utlh90pPn2pZ34_VAA8tZw) (Code: vpse)     |
| CLIPstyler (opti)            | &#10003;       | CVPR’22             | 50.3            | 50.4            | 0.1                   | [Link](https://pan.baidu.com/s/1xu-_xbGwFqlEfCUWF1lGlw) (Code: f29b)     |
| DiffusionCLIP                | &#10003;       | CVPR’22             | 50.3            | 34.3            | -16.0                 | [Link](https://pan.baidu.com/s/16DFzu7snPsHTvlByx0aWPg) (Code: c2c7)     |
| LDAST                        | &#10003;       | ECCV’22             | 50.3            | 36.6            | -13.7                 | [Link](https://pan.baidu.com/s/1NGZ_BiPQsEyxoeu610giWA) (Code: dmg8)     |
| TxST                         | &#10003;       | CVPR’23             | 50.3            | 36.7            | -13.6                 | [Link](https://pan.baidu.com/s/1zNOVk3vbFcNPWrKlGYQL0g) (Code: 2k2m)     |
| PODA                         | &#10003;       | ICCV’23             | 43.7            | 53.2            | 9.5                   | [Link](https://pan.baidu.com/s/1YMqptA60QyyLp1c2D-4q8g) (Code: swms)     |
| MMIST                        | &#10003;       | WACV’24             | 50.3            | 47.5            | -2.8                  | [Link](https://pan.baidu.com/s/1_OFT94IvSrHY1nhlHP20Iw) (Code: gu5y)     |
| DRIVE (ours)                 | &#10003;       | TMM'24              | 49.2            | 61.8            | 12.6                  | [Link](https://pan.baidu.com/s/1buWyvyVZnfpdP-xjZZOIjA) (Code: rctv)     |


:hotsprings: **Note:** LST refers to language-driven style transfer in either image-level space or feature-level space. Gain denotes as mean IoU gain on overall 19-class performance.


### Multimodal DG from Cityscapes to ACDC-Night ( :night_with_stars::night_with_stars: TABLE X)
:rocket::rocket: We provide quantitative results and checkpoint files in demo “from [Cityscapes](https://www.cityscapes-dataset.com/) to [ACDC](https://acdc.vision.ee.ethz.ch/overview)” ( :star: here model is tested on ACDC-Night dataset). Please view more details in TABLE X.


| Method                       | LST            | Pub’Year            | Source mIoU     | Target mIoU     | Gain                  | Checkpoint file                                                          |
|------------------------------|----------------|---------------------|-----------------|-----------------|-----------------------|--------------------------------------------------------------------------|
| AdaIN                        | &#10007;       | ICCV’17             | 15.3            | 24.2            | 8.9                   | [Link]() (Code: sb24)                                                    |
| CIConv                       | &#10007;       | ICCV’21             | 23.9            | 25.5            | 1.6                   | [Link]() (Code: pkvf)                                                    |
| RobustNet                    | &#10007;       | CVPR’21             | 6.8             | 20.1            | 13.3                  | [Link]() (Code: ppdu)                                                    |
| SNR                          | &#10007;       | TMM’21              | 15.3            | 23.3            | 8.0                   | [Link]() (Code: f63p)                                                    |
| WildNet                      | &#10007;       | CVPR’22             | 15.3            | 24.0            | 8.7                   | [Link]() (Code: vsfp)                                                    |
| CLIPstyler (fast)            | &#10003;       | CVPR’22             | 15.3            | 18.3            | 3.0                   | [Link]() (Code: hpfg)                                                    |
| CLIPstyler (opti)            | &#10003;       | CVPR’22             | 15.3            | 24.0            | 8.7                   | [Link]() (Code: cgkp)                                                    |
| DiffusionCLIP                | &#10003;       | CVPR’22             | 15.3            | 14.7            | -0.6                  | [Link]() (Code: spfj)                                                    |
| LDAST                        | &#10003;       | ECCV’22             | 15.3            | 16.3            | 1.0                   | [Link]() (Code: dtm3)                                                    |
| TxST                         | &#10003;       | CVPR’23             | 15.3            | 16.5            | 1.2                   | [Link]() (Code: rxv3)                                                    |
| PODA                         | &#10003;       | ICCV’23             | 18.0            | 23.6            | 5.6                   | [Link]() (Code: v376)                                                    |
| MMIST                        | &#10003;       | WACV’24             | 15.3            | 21.5            | 6.2                   | [Link]() (Code: bv4s)                                                    |
| DRIVE (ours)                 | &#10003;       | TMM'24              | 20.9            | 32.8            | 11.9                  | [Link]() (Code: gsrt)                                                    |


:hotsprings: **Note:** LST refers to language-driven style transfer in either image-level space or feature-level space. Gain denotes as mean IoU gain on overall 19-class performance.


### Multimodal DG from Cityscapes to ACDC-Rain ( :cloud_with_rain::cloud_with_rain: TABLE XI)
:rocket::rocket: We provide quantitative results and checkpoint files in demo “from [Cityscapes](https://www.cityscapes-dataset.com/) to [ACDC](https://acdc.vision.ee.ethz.ch/overview)” ( :star: here model is tested on ACDC-Rain dataset). Please view more details in TABLE XI.


| Method                       | LST            | Pub’Year            | mIoU            | Gain                  | Checkpoint file                                                          |
|------------------------------|----------------|---------------------|-----------------|-----------------------|--------------------------------------------------------------------------|
| AdaIN                        | &#10007;       | ICCV’17             | 44.9            | -5.4                  | [Link]() (Code: sb24)     |
| CIConv                       | &#10007;       | ICCV’21             | 56.7            | -1.6                  | [Link]() (Code: pkvf)     |
| RobustNet                    | &#10007;       | CVPR’21             | 61.8            | 0.3                   | [Link]() (Code: ppdu)     |
| SNR                          | &#10007;       | TMM’21              | 51.9            | 1.6                   | [Link]() (Code: f63p)     |
| WildNet                      | &#10007;       | CVPR’22             | 58.7            | 8.4                   | [Link]() (Code: vsfp)     |
| CLIPstyler (fast)            | &#10003;       | CVPR’22             | 51.6            | 1.3                   | [Link]() (Code: hpfg)     |
| CLIPstyler (opti)            | &#10003;       | CVPR’22             | 50.4            | 0.1                   | [Link]() (Code: cgkp)     |
| DiffusionCLIP                | &#10003;       | CVPR’22             | 34.3            | -16.0                 | [Link]() (Code: spfj)     |
| LDAST                        | &#10003;       | ECCV’22             | 36.6            | -13.7                 | [Link]() (Code: dtm3)     |
| TxST                         | &#10003;       | CVPR’23             | 36.7            | -13.6                 | [Link]() (Code: rxv3)     |
| PODA                         | &#10003;       | ICCV’23             | 53.2            | 9.5                   | [Link]() (Code: v376)     |
| MMIST                        | &#10003;       | WACV’24             | 47.5            | -2.8                  | [Link]() (Code: bv4s)     |
| DRIVE (ours)                 | &#10003;       | TMM'24              | 61.8            | 12.6                  | [Link]() (Code: gsrt)     |


:hotsprings: **Note:** LST refers to language-driven style transfer in either image-level space or feature-level space. Gain denotes as mean IoU gain on overall 19-class performance.


### Multimodal DG from Cityscapes to ACDC-Snow ( :snowflake::snowflake: TABLE XII)
:rocket::rocket: We provide quantitative results and checkpoint files in demo “from [Cityscapes](https://www.cityscapes-dataset.com/) to [ACDC](https://acdc.vision.ee.ethz.ch/overview)” ( :star: here model is tested on ACDC-Snow dataset). Please view more details in TABLE XII.


| Method                       | LST            | Pub’Year            | Source mIoU     | Target mIoU     | Gain                  | Checkpoint file                                                          |
|------------------------------|----------------|---------------------|-----------------|-----------------|-----------------------|--------------------------------------------------------------------------|
| AdaIN                        | &#10007;       | ICCV’17             | 38.2            | 43.3            | 5.1                   | [Link]() (Code: sb24)                                                    |
| CIConv                       | &#10007;       | ICCV’21             | 45.1            | 46.0            | 0.9                   | [Link]() (Code: pkvf)                                                    |
| RobustNet                    | &#10007;       | CVPR’21             | 42.4            | 46.1            | 3.7                   | [Link]() (Code: ppdu)                                                    |
| SNR                          | &#10007;       | TMM’21              | 38.2            | 42.8            | 4.6                   | [Link]() (Code: f63p)                                                    |
| WildNet                      | &#10007;       | CVPR’22             | 38.2            | 42.8            | 4.6                   | [Link]() (Code: vsfp)                                                    |
| CLIPstyler (fast)            | &#10003;       | CVPR’22             | 38.2            | 40.1            | 1.9                   | [Link]() (Code: hpfg)                                                    |
| CLIPstyler (opti)            | &#10003;       | CVPR’22             | 38.2            | 43.7            | 5.5                   | [Link]() (Code: cgkp)                                                    |
| DiffusionCLIP                | &#10003;       | CVPR’22             | 38.2            | 36.5            | -1.7                  | [Link]() (Code: spfj)                                                    |
| LDAST                        | &#10003;       | ECCV’22             | 38.2            | 35.7            | -2.5                  | [Link]() (Code: dtm3)                                                    |
| TxST                         | &#10003;       | CVPR’23             | 38.2            | 39.1            | 0.9                   | [Link]() (Code: rxv3)                                                    |
| PODA                         | &#10003;       | ICCV’23             | 36.4            | 45.1            | 8.7                   | [Link]() (Code: v376)                                                    |
| MMIST                        | &#10003;       | WACV’24             | 38.2            | 35.6            | -2.6                  | [Link]() (Code: bv4s)                                                    |
| DRIVE (ours)                 | &#10003;       | TMM'24              | 39.8            | 54.6            | 14.8                  | [Link]() (Code: gsrt)                                                    |


:hotsprings: **Note:** LST refers to language-driven style transfer in either image-level space or feature-level space. Gain denotes as mean IoU gain on overall 19-class performance.


