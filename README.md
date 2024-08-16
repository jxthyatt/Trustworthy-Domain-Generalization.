# Trustworthy Domain Generalization (TruDG)
Official repository for the submitted paper “Both Multi-silo and Multi-modality Matter: Trustworthy Domain Generalization via Personalized Federated Learning and Language-driven Zero-shot Adaptation”. Previous version of Code is [here](https://github.com/jxthyatt/Trustworthy-Domain-Generalization). :rainbow: Final Code will be released after acceptance.

## Replicate Demo and Results
### Federated DG under Distribution Heterogeneity ( :herb::herb: TABLE I)
:rocket::rocket: We evaluate cross-client **personalization** under distribution heterogeneity in demo “from Photo-Art-Cartoon to  Sketch”. ( :star: here model is performed on [PACS](https://datasets.activeloop.ai/docs/ml/datasets/pacs-dataset/) dataset). Please view more details in TABLE I.


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


