# Trustworthy-Domain-Generalization (TruDG)
Official repository for the submitted paper “Both Multi-silo and Multi-modality Matter: Trustworthy Domain Generalization via Personalized Federated Learning and Language-driven Zero-shot Adaptation”. Previous version of Code is [here](https://github.com/jxthyatt/Trustworthy-Domain-Generalization). :rainbow: Final Code will be released after acceptance.

## Replicate Demo and Results
### Federated DG under Distribution Heterogeneity ( :herb::herb: TABLE I)
:rocket::rocket: We evaluate cross-client **personalization** under distribution heterogeneity in demo “from Photo-Art-Cartoon to  Sketch”. ( :star: here model is performed on [PACS](https://datasets.activeloop.ai/docs/ml/datasets/pacs-dataset/) dataset). Please view more details in TABLE I.


| Method               | PFL            | Pub’Year        | P(Y)      | P(X)      | P(YX)    | Gain                  | Checkpoint file                                                          |
|----------------------|----------------|-----------------|-----------|-----------|-----------|-----------------------|--------------------------------------------------------------------------|
| q-FFL                | &#10007;       | arXiv’19        | 11.76     | 13.75     | 14.50     | -                     | [Link](https://pan.baidu.com/s/17K2VJVJkjrY-KOUwDNOjoA) (Code: ses8)     |
| AFL                  | &#10007;       | ICML’19         | 74.83     | 69.91     | 47.08     | 11.6                  | [Link](https://pan.baidu.com/s/1TLcvC1kkKdAd80Tj5DIEfg) (Code: vtex)     |
| FedProx              | &#10007;       | MLSys’20        | 71.19     | 66.88     | 62.12     | 4.4                   | [Link](https://pan.baidu.com/s/1Ro30WEFC0NIOc_ye0Y-kCw) (Code: 4dfn)     |
| FedAvg               | &#10007;       | AISTATS’17      | 76.66     | 68.18     | 58.44     | -8.0                  | [Link](https://pan.baidu.com/s/15jGyInrCvRFS5901HdWMEg) (Code: tkpt)     |
| Local                | &#10003;       | -               | 63.08     | 50.87     | 43.07     | 10.3                  | [Link](https://pan.baidu.com/s/1TnqcrC7HNHLKdJ0nu2F36w) (Code: p334)     |
| L2SGD                | &#10003;       | NeurIPS’20      | 63.41     | 49.35     | 44.91     | 8.7                   | [Link](https://pan.baidu.com/s/1GVtMJU1QbJeSls5gq54yGw) (Code: eth5)     |
| pFedMe               | &#10003;       | NeurIPS’20      | 64.57     | 50.65     | 44.81     | 4.0                   | [Link](https://pan.baidu.com/s/16fnnhYwl_ClEEzfJuScx-A) (Code: 9enn)     |
| ClusteredFL          | &#10003;       | TNNLS’20        | 67.22     | 69.91     | 46.97     | 5.7                   | [Link](https://pan.baidu.com/s/1VDULhtLO4VLy7W0l1v-9rw) (Code: exc4)     |
| FedAvg+              | &#10003;       | arXiv’19        | 75.50     | 69.59     | 58.66     | 12.3                  | [Link](https://pan.baidu.com/s/10xerTzDBD2KlOriyjDux9g) (Code: hswv)     |
| FedEM                | &#10003;       | NeurIPS’21      | 74.17     | 67.32     | 52.06     | 8.1                   | [Link](https://pan.baidu.com/s/1i_WcN8wlZRI8T0T1FMS8IA) (Code: yf92)     |
| FedGMM               | &#10003;       | ICML’23         | 75.83     | 70.67     | 59.20     | 9.7                   | [Link](https://pan.baidu.com/s/1XBh_ELFpseHxJr0ODqD3xw) (Code: 3f8r)     |
| pFedMAP (ours)       | &#10003;       | -               | 76.99     | 70.89     | 76.62     | 8.9                   | [Link](https://pan.baidu.com/s/1PrZ0PPoMFy_4JTalV3_cUg) (Code: 5e62)     |


| Method                    | DDA        | Pub’Year            | FC            | FD            | FZ            | Checkpoint file                                                          |
|---------------------------|------------|---------------------|---------------|---------------|---------------|--------------------------------------------------------------------------|
| Source only               | -          | -                   | 31.39         | 33.24         | 23.33         | [Link](https://pan.baidu.com/s/1fEMzwyZtniHnEouLHuwiUA) (Code: 566j)     |
| ADVENT                    | &#10007;   | CVPR’19             | 36.89         | 33.48         | 21.71         | [Link](https://pan.baidu.com/s/14U8ecye-ngEzmXjmpCBs2g) (Code: 2xik)     |
| DISE                      | &#10007;   | CVPR’19             | 41.47         | 34.63         | 22.40         | [Link](https://pan.baidu.com/s/1HUPR8_O18mELWb40sfEMww) (Code: idai)     |
| CAG-UDA                   | &#10007;   | NeurIPS’19          | 45.44         | 35.60         | 37.04         | [Link](https://pan.baidu.com/s/1dNB8IfjrbPIfP3RdJL4FFA) (Code: 8cqq)     |
| MaxSquareLoss             | &#10007;   | ICCV’19             | 38.28         | 35.38         | 24.14         | [Link](https://pan.baidu.com/s/1t-OAsEVnWBJjTu46zvsKnQ) (Code: pviq)     |
| Classes Matter            | &#10007;   | ECCV’20             | 36.53         | 29.59         | 23.31         | [Link](https://pan.baidu.com/s/14ZhBL8HEqplEYbqOJ-iAxQ) (Code: bmcy)     |
| ASANet                    | &#10007;   | TIP’21              | 36.15         | 30.30         | 20.95         | [Link](https://pan.baidu.com/s/1sUoGUYvHgTIQrjqF7E738w) (Code: 29ay)     |
| RobustNet                 | &#10007;   | CVPR’21             | 38.38         | 32.90         | 25.84         | [Link](https://pan.baidu.com/s/1bwpohufMajJg32OAd1ad4w) (Code: 7kki)     |
| Seg-Uncertainty           | &#10007;   | IJCV’21             | 48.17         | 38.39         | 26.39         | [Link](https://pan.baidu.com/s/19Rk-eBtk-7KOWUx2Mp3AZw) (Code: df78)     |
| DisCoGAN (ours)           | &#10003;   | TMM’24              | 43.05         | 35.91         | 30.47         | [Link](https://pan.baidu.com/s/1BLAhZkDKzk0r2crS6BvDoQ) (Code: 4ng5)     |
| ProRA (ours)              | &#10003;   | TMM’24              | 49.71         | 37.65         | 32.28         | [Link](https://pan.baidu.com/s/1n2xCu49kXcVPmTgrlzptBg) (Code: iqgc)     |
| DisCoGAN+ProRA (ours)     | &#10003;   | TMM’24              | 55.26         | 42.24         | 35.51         | [Link](https://pan.baidu.com/s/1tI3rlI0969DwfNwFYZUFcQ) (Code: cswk)     |


