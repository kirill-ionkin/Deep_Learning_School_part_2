# Deep_Learning_School_part_2
Данный репозиторий является кратким, структурированным конспектом
изучаемого материала в процессе обучения в Deep Learning School


## Оглавление

- [Организационная информация](#Организационная-информация)
- [Введение в NLP и классификация текста](#Введение-в-NLP-и-классификация-текста)
  - [Homework: Simple Embeddings](#Homework-Simple-Embeddings)
- [Embeddings](#Embeddings)
  - [Homework: Embeddings](#Homework-Embeddings)
- [Рекуррентные нейронные сети](#Рекуррентные-нейронные-сети)
  - [Homework: Text Classification](#Homework-Text-Classification)
- [Language modelling](#Language-modelling)
  - []()
- [Neural Machine Translation](#Neural-Machine-Translation)
  - [Homework: Seq2Seq with Attention](#Homework-Seq2Seq-with-Attention)


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

### Homework Simple Embeddings
```
Ставится задача поиска похожих по смыслу  вопросов(вопросы StackOverflow), а именно задача ранжирования вопросов.
1. Используются предобученные эмбеддинги слов
  - from gensim.models.keyedvectors import KeyedVectors
  - KeyedVectors.load_word2vec_format("SO_vectors_200.bin?download=1", binary=True)
2. Представление эмбеддинга предожения через эмбеддинги слов
3. Метрики ранжирования
  - Hits@K
  - DCG@K
4. Ранжирование по косинусной похожести
5. Обучение Word2Vec на корпусе похожих вопросов
- from gensim.models import Word2Vec
6. Применение различный токенизаторов, стеммингов, лемматизаторов, стоп-слов и т.д.
```
- [[homework]simple_embeddings.ipynb](03_hw_Simple_embeddings/[homework]simple_embeddings.ipynb)


## Embeddings

- [Embeddings.pdf](04_Embeddings/Embeddings.pdf)
- [word2vec.ipynb](04_Embeddings/word2vec.ipynb)


- [Лекция. Embeddings.](https://www.youtube.com/watch?v=eXQAOTsbhLQ)
- [Семинар. Word2Vec.](https://www.youtube.com/watch?v=iLzZO_4xyMg)

### Homework Embeddings
```
Ставится задача семантической классификации твитов с помощью эмбеддингов(предобученных или обученных нами)
  1. Использование word2veс(предобученного) для получения эмбеддингов
    - word2vec = api.load("word2vec-google-news-300")
  2. Препроцессинг данных + различные способы получения эмбеддингов предложения по эмбеддингам слов
    - import gensim
    - import gensim.donloader as api
    - import nltk
  3. Нормализация эмбеддингов перед подачей их в нейронную сеть.
  4. Создание кастомного Datset для обучения модели
  5. Визуализация векторов предложений с помощью PCA
  6. Embedding for unknown words
    - Представление эмбеддинга незнакомого слова через его "ближний" контекст
    - Представление эмбеддинга незнакомого слова чреез обученный tfidf
      - from sklearn.feature_extraction.text import TfidfVectorizer
        - !pip install sparsesvd
        - from sparsesvd import sparsesvd
        - Библиотека для SVD разложения sparse matrix
```
- [[homework]embeddings.ipynb](05_hw_Embeddings/[homework]embeddings.ipynb)


## Рекуррентные нейронные сети

- [RNN.pdf](06_Рекуррентные_нейронные_сети/RNN.pdf)
- [seminar_cnn_and_rnn.ipynb](06_Рекуррентные_нейронные_сети/seminar_cnn_and_rnn.ipynb)
  - [библиотека Datasets от huggingface](https://huggingface.co/docs/datasets/)


- [Лекция. Embeddings.](https://www.youtube.com/watch?v=eXQAOTsbhLQ&ab_channel=DeepLearningSchool)
- [Семинар. Рекуррентные нейронные сети](https://www.youtube.com/watch?v=_wpAkWZmlyg&t=1474s&ab_channel=DeepLearningSchool)

### Homework Text Classification
```
Ставится задача бинарной классификации текстов на "neg"(негативные) и "pos"(позитивные),
а такде предлагается понять, насколько хорошо модель "понимает" смысл слов и какие слова
влиют на результат  ответа модели.
  1. Использование torchtext:
    - datasets
    - Field, LabelField, BucketIterator
    - Vectors, GloVe
  2. Использование LSTM для задачи классификации
  3. Использование CNN для задачи классификации
  4. Библиотека для интерпретации того, насколько модель хорошо  понимает смысл слов 
    - !pip install -q captum
    - LayerIntegratedGradients, TokenReferenceBase, visualization
  5. Использование предобученных эмбеддингов для инициализации словаря модели 
```
- [_[homework]classification.ipynb](07_hw_Text_Classification/_[homework]classification.ipynb)
- Вспомогательные источники:
  - Understanding BucketIterator, Field, LabelField, Glove
    - [Better Batches with PyTorchText BucketIterator](https://gmihaila.medium.com/better-batches-with-pytorchtext-bucketiterator-12804a545e2a)
    - [Sentiment Analysis with LSTM and TorchText with Code and Explanation](https://www.analyticsvidhya.com/blog/2021/09/sentiment-analysis-with-lstm-and-torchtext-with-code-and-explanation/)
  - Understanding Glove, Vectors and why do i need it
    - [Deep Learning For NLP with PyTorch and Torchtext](https://towardsdatascience.com/deep-learning-for-nlp-with-pytorch-and-torchtext-4f92d69052f)
  - Understanding Bidirectional
    - [Understanding Bidirectional RNN in PyTorch](https://towardsdatascience.com/understanding-bidirectional-rnn-in-pytorch-5bd25a5dd66)
  - CNN for text classifications
    - [practice02_CNN_for_texts.ipynb(семинар от Родослава Нейчева)](ml-mipt/week1_02_CNN_for_texts_and_more_embeddings/practice02_CNN_for_texts.ipynb)


## Language modelling

- [Языковые_модели.pdf](08_Language_Modelling/Языковые_модели.pdf)
- [Language_modeling_seminar.ipynb](08_Language_Modelling/Language_modeling_seminar.ipynb)


- [Лекция. Языковые модели. Введение. Частотный подход](https://www.youtube.com/watch?v=aS2A7b-4uT4&list=PL0Ks75aof3Ti1GDgeePUkCJWn02c0VDA5&index=10)
- [Лекция. Языковые модели. Нейронные сети](https://www.youtube.com/watch?v=-tK7WcE5Wfo&list=PL0Ks75aof3Ti1GDgeePUkCJWn02c0VDA5&index=9)
- [Семинар. Языковые модели](https://www.youtube.com/watch?v=WoYRZEsWIrg&list=PL0Ks75aof3Ti1GDgeePUkCJWn02c0VDA5&index=8&ab_channel=DeepLearningSchool)

### Homework Part of Speech Tagger


## Neural Machine Translation

- [Seq2Seq_Attention.pdf](10_Neural_Machine_Translation/Seq2Seq_Attention.pdf)
- [[seminar_class]NeuralMachineTranslation.ipynb](10_Neural_Machine_Translation/[seminar_class]NeuralMachineTranslation.ipynb)


- [Лекция. Seq2Seq, машинный перевод.](https://www.youtube.com/watch?v=N3TLYsn0TU8&ab_channel=DeepLearningSchool)
- [Лекция. Внимание (Attention)](https://www.youtube.com/watch?v=G4vT5cvJSxY&ab_channel=DeepLearningSchool)
- [Семинар. Seq2Seq](https://www.youtube.com/watch?v=d8A1nxoZDDk&ab_channel=DeepLearningSchool)

### Homework Seq2Seq with Attention
```
Ставится задача машинного перевола, для чего необходимо
реализовать архитектуру Seq2Seq с механизмом Attention для декодера.
  1. Использование torchtext для препроцессинга данных.
    - Field(tokenizer= ...,
            init_token="<sos>",
            eos_token="<eos>",
            lower=True
            )
    - TabularDataset
    - BucketIterator
  2. Encoder
    - LSTM
    - n_layers = 1
    - bidirectional = True
    - Преобразование hidden, cell на выходе из encoder, т.к.
      вследствие bidirectional размерность увеличивается  
  3. Temperature Softmax
    - Температурный Softmax, благодаря которому можно с помощью
      температуры сильнее выделять вероятность классов или
      наоборот делать распределение равномерным
  4. Attention(concat attention)
  5. Decoder with attention
    - GRU
    - n_layers = 1
    - bidirectional = False
  6. Seq2Seq
  7. Init params to Encoder, Decoder, Attention, Seq2Seq
  8. Other
    - Train loop
    - Val loop
    - Plot 
    - translation
    - Metric:  BLEU
```
- [[homework]NeuralMachineTranslation.ipynb](11_hw_Seq2Seq_with_Attention/[homework]NeuralMachineTranslation.ipynb)
- Вспомогательные источники:
  - [Sequence to Sequence (seq2seq) and Attention](https://lena-voita.github.io/nlp_course/seq2seq_and_attention.html)