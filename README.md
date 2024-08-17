# Trustworthy Domain Generalization (TruDG)
Official repository for the submitted paper “Both Multi-silo and Multi-modality Matter: Trustworthy Domain Generalization via Personalized Federated Learning and Language-driven Zero-shot Adaptation”. Previous version of Code is [here](https://github.com/jxthyatt/Trustworthy-Domain-Generalization). :rainbow: Final Code will be released after acceptance.

## Replicate Demo and Results
### Federated DG under Distribution Heterogeneity ( :herb::herb: TABLE I)
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


### Federated DG for Facial Expression Recognition ( :herb::herb: TABLE II)
:rocket::rocket: We evaluate cross-client **personalization** under “Leave-One-Domain-Out” experiments ( :star: here model is performed on [RAF-DB](http://www.whdeng.cn/raf/model1.html), [ExpW](https://mmlab.ie.cuhk.edu.hk/projects/socialrelation/index.html), and [FER2013](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data) datasets). Please view more details in TABLE II.


| Method               | PFL            | Pub’Year        | RAF-DB         | ExpW           | FER2013        | Avg.           | Checkpoint file                                                          |
|----------------------|----------------|-----------------|----------------|----------------|----------------|----------------|--------------------------------------------------------------------------|
| FedAvg               | &#10007;       | AISTATS’17      | 52.18          | 60.00          | 52.60          | 54.93          | [Link]() (Code: f3kf)     |
| q-FFL                | &#10007;       | arXiv’19        | 14.35          | 14.25          | 10.76          | 13.12          | [Link]() (Code: a2bx)     |
| AFL                  | &#10007;       | ICML’19         | 44.02          | 51.05          | 47.39          | 47.49          | [Link]() (Code: q1by)     |
| FedProx              | &#10007;       | MLSys’20        | 42.25          | 50.48          | 44.43          | 45.72          | [Link]() (Code: mycg)     |
| Local                | &#10003;       | -               | 40.09          | 49.92          | 43.89          | 44.64          | [Link]() (Code: 55pw)     |
| FedAvg+              | &#10003;       | arXiv’19        | 52.67          | 59.21          | 52.21          | 54.70          | [Link]() (Code: 7utu)     |
| L2SGD                | &#10003;       | NeurIPS’20      | 35.82          | 42.17          | 40.06          | 39.35          | [Link]() (Code: g3rj)     |
| pFedMe               | &#10003;       | NeurIPS’20      | 38.87          | 44.20          | 40.02          | 41.03          | [Link]() (Code: krt3)     |
| ClusteredFL          | &#10003;       | TNNLS’20        | 67.22          | 57.93          | 52.65          | 53.15          | [Link]() (Code: ab18)     |
| FedEM                | &#10003;       | NeurIPS’21      | 51.08          | 58.59          | 53.91          | 54.53          | [Link]() (Code: 1c3n)     |
| FedGMM               | &#10003;       | ICML’23         | 50.76          | 57.36          | 52.81          | 53.64          | [Link]() (Code: mt6f)     |
| pFedMAP (ours)       | &#10003;       | TMM'24          | 52.17          | 58.88          | 54.33          | 55.12          | [Link]() (Code: ymrv)     |


:airplane::airplane: We evaluate out-of-client **generalization** under “Leave-One-Domain-Out” experiments ( :star: here model is performed on [RAF-DB](http://www.whdeng.cn/raf/model1.html), [ExpW](https://mmlab.ie.cuhk.edu.hk/projects/socialrelation/index.html), and [FER2013](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data) datasets). Please view more details in TABLE II.


| Method               | PFL            | Pub’Year        | RAF-DB         | ExpW           | FER2013        | Avg.           | Checkpoint file                                                          |
|----------------------|----------------|-----------------|----------------|----------------|----------------|----------------|--------------------------------------------------------------------------|
| FedAvg               | &#10007;       | AISTATS’17      | 30.07          | 21.58          | 28.52          | 26.72          | [Link]() (Code: f3kf)     |
| q-FFL                | &#10007;       | arXiv’19        | 11.62          | 13.49          | 13.05          | 12.72          | [Link]() (Code: a2bx)     |
| AFL                  | &#10007;       | ICML’19         | 26.49          | 12.17          | 17.73          | 18.80          | [Link]() (Code: q1by)     |
| FedProx              | &#10007;       | MLSys’20        | 28.86          | 19.26          | 15.37          | 21.16          | [Link]() (Code: mycg)     |
| Local                | &#10003;       | -               | 15.64          | 15.31          | 14.55          | 15.17          | [Link]() (Code: 55pw)     |
| FedAvg+              | &#10003;       | arXiv’19        | 32.16          | 27.98          | 40.08          | 33.40          | [Link]() (Code: 7utu)     |
| L2SGD                | &#10003;       | NeurIPS’20      | 25.09          | 21.96          | 27.94          | 25.00          | [Link]() (Code: g3rj)     |
| pFedMe               | &#10003;       | NeurIPS’20      | 25.57          | 39.02          | 27.65          | 30.75          | [Link]() (Code: krt3)     |
| ClusteredFL          | &#10003;       | TNNLS’20        | 14.14          | 13.93          | 15.22          | 14.43          | [Link]() (Code: ab18)     |
| FedEM                | &#10003;       | NeurIPS’21      | 41.45          | 38.83          | 28.28          | 36.19          | [Link]() (Code: 1c3n)     |
| FedGMM               | &#10003;       | ICML’23         | 38.31          | 44.54          | 35.89          | 39.58          | [Link]() (Code: mt6f)     |
| pFedMAP (ours)       | &#10003;       | TMM'24          | 40.34          | 49.56          | 53.18          | 47.69          | [Link]() (Code: ymrv)     |


:hotsprings: **Note:** PFL refers to personalized federated learning. All methods for federated DG are deployed under Leave-One-Domain-Out experiments, e.g., the first column means choosing one domain (RAF-DB) to hold out as a target client while using others (FER2013 and ExpW) as source clients.
















