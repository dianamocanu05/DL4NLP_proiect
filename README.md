# Extracting drug-drug interactions from texts with BioBERT and multiple entity-aware attentions

This problem was approached from multiple methods that can be classified into two big groups: classic machine learning and deep neural networks. From recent studies, we found that best results are achieved by the various architectures of deep neural networks.

In order to choose one method to be our representative state-of-the-art, we will take into consideration the F1 metric over all the classes as the ordering element. The best result was optained in the article [3] with an F-score(%) of 85.40.

The authors used more algorithms, but the winning one was named by them as "PubMedBERT + HKG". This is using the well-known pre-trained BERT language model specialized for medical and biochemistry terms. The training process was done using the largest open-source collection of chemical structures. The HKG abbreviation stands for heterogeneous knowledge graph.


# Bibliography

1. [Yu Zhu, Lishuang Li, Hongbin Lu, Anqiao Zhou, Xueyang Qin, Extracting drug-drug interactions from texts with BioBERT and multiple entity-aware attentions, Journal of Biomedical Informatics, Volume 106, 2020](https://www.sciencedirect.com/science/article/pii/S1532046420300794) 
2. [Masaki Asada, Makoto Miwa, Yutaka Sasaki, Using drug descriptions and molecular structures for drug–drug interaction extraction from literature, Bioinformatics, Volume 37, Issue 12, June 2021, Pages 1739–1746](https://doi.org/10.1093/bioinformatics/btaa907)
3. [Masaki Asada, Makoto Miwa, Yutaka Sasaki, Integrating heterogeneous knowledge graphs into drug–drug interaction extraction from the literature, Bioinformatics, Volume 39, Issue 1, January 2023, btac754](https://doi.org/10.1093/bioinformatics/btac754)
4. [Yang, Jie and Ding, Yihao and Long, Siqu and Poon, Josiah and Han, Soyeon Caren, DDI-MuG: Multi-aspect graphs for drug-drug interaction extraction, Frontiers in Digital Health, Volume 5, 2023](https://www.frontiersin.org/articles/10.3389/fdgth.2023.1154133)

## Deadlines:

- December 14th: state of the art
- 

