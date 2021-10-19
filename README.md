# Deep_Learning_School_part_2
Данный репозиторий является кратким, структурированным конспектом
изучаемого материала в процессе обучения в Deep Learning School


## Оглавление

- [Организационная информация](#Организационная-информация)
- [Введение в NLP и классификация текста](#Введение-в-NLP-и-классификация-текста)
- [Embeddings](#Embeddings)
- [Рекуррентные нейронные сети](#Рекуррентные-нейронные-сети)


## Организационная информация


## Введение в NLP и классификация текста
 
- [Введение_в_NLP.pdf](02_Введение_в_NLP_и_классификация_текста/Введение_в_NLP.pdf)
- [[seminar]text_preprocessing_and_classification.ipynb](02_Введение_в_NLP_и_классификация_текста/[seminar]text_preprocessing_and_classification.ipynb)
    - [nltk](https://www.nltk.org/)
    - [Gensim](https://radimrehurek.com/gensim/)
    - [Razdel](https://natasha.github.io/razdel/)
    - [natasha](https://natasha.github.io/)


- [Лекция. Введение в NLP.](https://www.youtube.com/watch?v=d0oV1MZ_KdE&ab_channel=DeepLearningSchool)
- [Семинар. Обработка текста.](https://www.youtube.com/watch?v=Aa-p8ddbxpQ)
- [Семинар. Решение задачи классификации текста](https://www.youtube.com/watch?v=ltyWeIPrAVA)


- Предобработка текста
![](for_readme/02_Введение_в_NLP_и_классификация_текста/1.png)
- Выделение признаков
![](for_readme/02_Введение_в_NLP_и_классификация_текста/2.png)
![](for_readme/02_Введение_в_NLP_и_классификация_текста/3.png)
![](for_readme/02_Введение_в_NLP_и_классификация_текста/4.png)
![](for_readme/02_Введение_в_NLP_и_классификация_текста/4_1.png)
![](for_readme/02_Введение_в_NLP_и_классификация_текста/5.png)
- Коллокация, NGramms
![](for_readme/02_Введение_в_NLP_и_классификация_текста/6.png)
- Pointwise mutual information
![](for_readme/02_Введение_в_NLP_и_классификация_текста/7.png)
![](for_readme/02_Введение_в_NLP_и_классификация_текста/7_1.png)
- Context embeddings
![](for_readme/02_Введение_в_NLP_и_классификация_текста/8.png)
![](for_readme/02_Введение_в_NLP_и_классификация_текста/8_1.png)
- Уменьшение размерности данных
![](for_readme/02_Введение_в_NLP_и_классификация_текста/9.png)
- Co-Occurrence Count + dimensional reduction
![](for_readme/02_Введение_в_NLP_и_классификация_текста/10_1.png)
![](for_readme/02_Введение_в_NLP_и_классификация_текста/10.png)
- PMI + dimensional reduction
![](for_readme/02_Введение_в_NLP_и_классификация_текста/11.png)
- TF-IDF + dimensional reduction
![](for_readme/02_Введение_в_NLP_и_классификация_текста/12.png)


## Embeddings

- [Embeddings.pdf](04_Embeddings/Embeddings.pdf)
- [word2vec.ipynb](04_Embeddings/word2vec.ipynb)


- [Лекция. Embeddings.](https://www.youtube.com/watch?v=eXQAOTsbhLQ)
- [Семинар. Word2Vec.](https://www.youtube.com/watch?v=iLzZO_4xyMg)


- Word2Vec(идея скользящего окна для подсчёта pmi, Co-Occurrence Count, etc.)
![](for_readme/04_Embeddings/1.png)
- Cross-Entropy(мера расхождения между двумя распределениями)
![](for_readme/04_Embeddings/2.png)
- Target function, log-likelihood для Word2Vec
![](for_readme/04_Embeddings/3.png)
- Схема работы Word2Vec
![](for_readme/04_Embeddings/4.png)
- 2 схемы работы Word2Vec(Skip-Gram, CBOW)
![](for_readme/04_Embeddings/5.png)
![](for_readme/04_Embeddings/6.png)
- Word2Vec + negative sampling ~ SVD
![](for_readme/04_Embeddings/7.png)
- Видоизменённая лосс-функция
![](for_readme/04_Embeddings/8.png)


# Рекуррентные нейронные сети

- [RNN.pdf](06_Рекуррентные_нейронные_сети/RNN.pdf)
- [seminar_cnn_and_rnn.ipynb](06_Рекуррентные_нейронные_сети/seminar_cnn_and_rnn.ipynb)


- [Лекция. Embeddings.](https://www.youtube.com/watch?v=eXQAOTsbhLQ&ab_channel=DeepLearningSchool)
- [Семинар. Рекуррентные нейронные сети](https://www.youtube.com/watch?v=_wpAkWZmlyg&t=1474s&ab_channel=DeepLearningSchool)


![](for_readme/06_Рекуррентные_нейронные_сети/1.png)
![](for_readme/06_Рекуррентные_нейронные_сети/1_1.png)
![](for_readme/06_Рекуррентные_нейронные_сети/2.png)
![](for_readme/06_Рекуррентные_нейронные_сети/3.png)
![](for_readme/06_Рекуррентные_нейронные_сети/4.png)
- Более сложные структуры для рекуррентных нейронных сетей
![](for_readme/06_Рекуррентные_нейронные_сети/5.png)
![](for_readme/06_Рекуррентные_нейронные_сети/6.png)
![](for_readme/06_Рекуррентные_нейронные_сети/7.png)
![](for_readme/06_Рекуррентные_нейронные_сети/8.png)


