## Embeddings

- [Embeddings.pdf](Embeddings.pdf)
- [word2vec.ipynb](word2vec.ipynb)


- [Лекция. Embeddings.](https://www.youtube.com/watch?v=eXQAOTsbhLQ)
- [Семинар. Word2Vec.](https://www.youtube.com/watch?v=iLzZO_4xyMg)


- Word2Vec(идея скользящего окна для подсчёта pmi, Co-Occurrence Count, etc.)
  ![](../for_readme/04_Embeddings/1.png)
- Cross-Entropy(мера расхождения между двумя распределениями)
  ![](../for_readme/04_Embeddings/2.png)
- Target function, log-likelihood для Word2Vec
  ![](../for_readme/04_Embeddings/3.png)
- Схема работы Word2Vec
  ![](../for_readme/04_Embeddings/4.png)
- 2 схемы работы Word2Vec(Skip-Gram, CBOW)
  ![](../for_readme/04_Embeddings/5.png)
  ![](../for_readme/04_Embeddings/6.png)
- Word2Vec + negative sampling ~ SVD
  ![](../for_readme/04_Embeddings/7.png)
- Видоизменённая лосс-функция
  ![](../for_readme/04_Embeddings/8.png)