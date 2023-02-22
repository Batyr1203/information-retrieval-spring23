# HA2: collection indexing using Elasticsearch

## Data
WikiIR Collection: https://github.com/getalp/wikIR

Generated lemmatized collection can be found here: https://drive.google.com/file/d/1aXHb-FIN0HdCtUZapwbXmvc9kqDzXkbp/view?usp=sharing

## Evaluation

| Approach      | p@5 | p@10     |  p@20 | MAP |
| :---        |    :----:   |   :----:  |   :----: |  ---:  |
| BM25 (given)      |   0.1840     |  0.1320    | 0.0950 | 0.1120 |
| Without stemming   |     0.3060    |   0.2080    | **0.1500** | **0.1479** |
| With stemming | **0.3120** | **0.2100** | 0.1425 | 0.1463 |
| Lemm. collect. + boost phr. match. | 0.2440 | 0.1850 | 0.1300 | 0.1207 |
