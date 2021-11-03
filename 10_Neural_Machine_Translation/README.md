## Neural Machine Translation

- [Seq2Seq_Attention.pdf](Seq2Seq_Attention.pdf)
- [[seminar_class]NeuralMachineTranslation.ipynb]([seminar_class]NeuralMachineTranslation.ipynb)


- [Лекция. Seq2Seq, машинный перевод.](https://www.youtube.com/watch?v=N3TLYsn0TU8&ab_channel=DeepLearningSchool)
- [Лекция. Внимание (Attention)](https://www.youtube.com/watch?v=G4vT5cvJSxY&ab_channel=DeepLearningSchool)
- [Семинар. Seq2Seq](https://www.youtube.com/watch?v=d8A1nxoZDDk&ab_channel=DeepLearningSchool)


- Постановка задачи машинного перевода
![](../for_readme/10_Neural_Machine_Translation/1.png)
![](../for_readme/10_Neural_Machine_Translation/2.png)
- Seq2Seq(или как решать задачу машинного перевода с помощью нейронных сетей)
- Архитектура Encoder-Decoder
![](../for_readme/10_Neural_Machine_Translation/3.png)
![](../for_readme/10_Neural_Machine_Translation/4.png)
- Как обучается Encoder-Decoder?
![](../for_readme/10_Neural_Machine_Translation/5.png)
- Teacher-forcing(подача decoder-у правильных слов)
![](../for_readme/10_Neural_Machine_Translation/6.png)
![](../for_readme/10_Neural_Machine_Translation/7.png)
- Метрика качества машинного перевода
![](../for_readme/10_Neural_Machine_Translation/8.png)
- Проблемы архитектуры Encoder-Decoder
![](../for_readme/10_Neural_Machine_Translation/9.png)
- Пример проблемы жадного декодировани
![](../for_readme/10_Neural_Machine_Translation/10.png)
- Решение проблемы жадного декодирования: Beam search
![](../for_readme/10_Neural_Machine_Translation/11.png)

- Идея Attention
![](../for_readme/10_Neural_Machine_Translation/12.png)
- Attention для Decoder
![](../for_readme/10_Neural_Machine_Translation/13.png)
![](../for_readme/10_Neural_Machine_Translation/14.png)
- Примеры того, что может быть Attention
![](../for_readme/10_Neural_Machine_Translation/15.png)
- Self-Attention
![](../for_readme/10_Neural_Machine_Translation/16.png)
- Self-Attention для Encoder
![](../for_readme/10_Neural_Machine_Translation/17.png)
- Self-Attention для Decoder
![](../for_readme/10_Neural_Machine_Translation/18.png)
- В модели может быть несколько Attention, Self-Attention
![](../for_readme/10_Neural_Machine_Translation/19.png)

