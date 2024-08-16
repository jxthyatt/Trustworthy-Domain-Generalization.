# Trustworthy-Domain-Generalization (TruDG)
Official repository for the submitted paper “Both Multi-silo and Multi-modality Matter: Trustworthy Domain Generalization via Personalized Federated Learning and Language-driven Zero-shot Adaptation”. Previous version of Code is [here](https://github.com/jxthyatt/Trustworthy-Domain-Generalization). :rainbow: Final Code will be released after acceptance.

## Replicate Demo and Results
### Federated DG under Distribution Heterogeneity ( :herb::herb: TABLE I)
:rocket::rocket: We evaluate cross-client **personalization** under distribution heterogeneity in demo “from Photo-Art-Cartoon to  Sketch”. ( :star: here model is performed on [PACS](https://datasets.activeloop.ai/docs/ml/datasets/pacs-dataset/) dataset). Please view more details in TABLE I.


| Method               | PFL            | Pub’Year        | P(Y)           | P(X)           | P(Y&#124;X)    | P(X,Y)         | Checkpoint file                                                          |
|----------------------|----------------|-----------------|----------------|----------------|----------------|----------------|--------------------------------------------------------------------------|
| q-FFL                | &#10007;       | arXiv’19        | 11.76          | 13.75          | 14.50          | 15.45          | [Link](https://pan.baidu.com/s/17K2VJVJkjrY-KOUwDNOjoA) (Code: ses8)     |
| AFL                  | &#10007;       | ICML’19         | 74.83          | 69.91          | 47.08          | 59.62          | [Link](https://pan.baidu.com/s/1TLcvC1kkKdAd80Tj5DIEfg) (Code: vtex)     |
| FedProx              | &#10007;       | MLSys’20        | 71.19          | 66.88          | 62.12          | 60.27          | [Link](https://pan.baidu.com/s/1Ro30WEFC0NIOc_ye0Y-kCw) (Code: 4dfn)     |
| FedAvg               | &#10007;       | AISTATS’17      | 76.66          | 68.18          | 58.44          | 65.73          | [Link](https://pan.baidu.com/s/15jGyInrCvRFS5901HdWMEg) (Code: tkpt)     |
| Local                | &#10003;       | -               | 63.08          | 50.87          | 43.07          | 57.12          | [Link](https://pan.baidu.com/s/1TnqcrC7HNHLKdJ0nu2F36w) (Code: p334)     |
| L2SGD                | &#10003;       | NeurIPS’20      | 63.41          | 49.35          | 44.91          | 53.93          | [Link](https://pan.baidu.com/s/1GVtMJU1QbJeSls5gq54yGw) (Code: eth5)     |
| pFedMe               | &#10003;       | NeurIPS’20      | 64.57          | 50.65          | 44.81          | 55.80          | [Link](https://pan.baidu.com/s/16fnnhYwl_ClEEzfJuScx-A) (Code: 9enn)     |
| ClusteredFL          | &#10003;       | TNNLS’20        | 67.22          | 69.91          | 46.97          | 64.74          | [Link](https://pan.baidu.com/s/1VDULhtLO4VLy7W0l1v-9rw) (Code: exc4)     |
| FedAvg+              | &#10003;       | arXiv’19        | 75.50          | 69.59          | 58.66          | 63.41          | [Link](https://pan.baidu.com/s/10xerTzDBD2KlOriyjDux9g) (Code: hswv)     |
| FedEM                | &#10003;       | NeurIPS’21      | 74.17          | 67.32          | 52.06          | 66.06          | [Link](https://pan.baidu.com/s/1i_WcN8wlZRI8T0T1FMS8IA) (Code: yf92)     |
| FedGMM               | &#10003;       | ICML’23         | 75.83          | 70.67          | 59.20          | 63.08          | [Link](https://pan.baidu.com/s/1XBh_ELFpseHxJr0ODqD3xw) (Code: 3f8r)     |
| pFedMAP (ours)       | &#10003;       | -               | 76.99          | 70.89          | 76.62          | 68.05          | [Link](https://pan.baidu.com/s/1PrZ0PPoMFy_4JTalV3_cUg) (Code: 5e62)     |


