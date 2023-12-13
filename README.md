# Extracting drug-drug interactions from texts

This problem was approached from multiple methods that can be classified into two big groups: classic machine learning and deep neural networks. From recent studies, we found that the various architectures of deep neural networks achieve the best results.

In order to choose one method to be our representative state-of-the-art, we will consider the F1 metric over all the classes as the ordering element. The best result was obtained in the article [3] with an F-score(%) of 85.40.

The authors used more algorithms, but they named the winning one "PubMedBERT + HKG". This is using the well-known pre-trained BERT language model specialized for medical and biochemistry terms. The training process was done using the largest open-source collection of chemical structures. The HKG abbreviation stands for heterogeneous knowledge graph.

The main idea of this model is the preprocessing of the medical articles, the way of text embedding with the scope of giving a simple dense neural network as much information as it can. To achieve that, they combine the above-mentioned methods in the following way: in the embedding lookup layer, they concatenate the output of the BERT's word embedding table with the output of the HKG word embedding table and feed the resulting vector to the classic BERT layer. After the language model layer, the output is then concatenated and sent to a classification network. 


<img src="https://oup.silverchair-cdn.com/oup/backfile/Content_public/Journal/bioinformatics/39/1/10.1093_bioinformatics_btac754/1/btac754f2.jpeg?Expires=1705505680&Signature=LVO5w-n2z2YmrSzMqKnoteC06zcJMeoa0lYdhZLRsTjwW6EqG4NhyaHKqL1WHHNAV6TL4LVdZ1uWVImeK5FGhiwlcC64IbzdaYFaMN36eccy1dDx7LmrmbvlptV5YWduH4wjgpaJQ6UZxKQfRPQix~OtVeXwIy1ols4uhzumflrT9DAvf18vbFuh484NiwtpA648MNkeX0GZI6ebh4RuaesjoqJQbo30H20iATblSOkj0bGlLpemdJji~eHMIiZd-PH6hRUvzFPZ7nCg-EE9lp26S4IENNMa5b6pfGhyEjkjkiBkLgWFV2sFoU-nZKu5BlvtTbk0YWeaX5pKlLSLfA__&Key-Pair-Id=APKAIE5G5CRDK6RD3PGA">

# Bibliography

1. [Yu Zhu, Lishuang Li, Hongbin Lu, Anqiao Zhou, Xueyang Qin, Extracting drug-drug interactions from texts with BioBERT and multiple entity-aware attentions, Journal of Biomedical Informatics, Volume 106, 2020](https://www.sciencedirect.com/science/article/pii/S1532046420300794) 
2. [Masaki Asada, Makoto Miwa, Yutaka Sasaki, Using drug descriptions and molecular structures for drug–drug interaction extraction from literature, Bioinformatics, Volume 37, Issue 12, June 2021, Pages 1739–1746](https://doi.org/10.1093/bioinformatics/btaa907)
3. [Masaki Asada, Makoto Miwa, Yutaka Sasaki, Integrating heterogeneous knowledge graphs into drug–drug interaction extraction from the literature, Bioinformatics, Volume 39, Issue 1, January 2023, btac754](https://doi.org/10.1093/bioinformatics/btac754)
4. [Yang, Jie and Ding, Yihao and Long, Siqu and Poon, Josiah and Han, Soyeon Caren, DDI-MuG: Multi-aspect graphs for drug-drug interaction extraction, Frontiers in Digital Health, Volume 5, 2023](https://www.frontiersin.org/articles/10.3389/fdgth.2023.1154133)

## Deadlines:

- December 14th: state of the art
- 

