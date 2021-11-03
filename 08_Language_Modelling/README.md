## Language modelling

- [Языковые_модели.pdf](Языковые_модели.pdf)
- [Language_modeling_seminar.ipynb](Language_modeling_seminar.ipynb)


- [Лекция. Языковые модели. Введение. Частотный подход](https://www.youtube.com/watch?v=aS2A7b-4uT4&list=PL0Ks75aof3Ti1GDgeePUkCJWn02c0VDA5&index=10)
- [Лекция. Языковые модели. Нейронные сети](https://www.youtube.com/watch?v=-tK7WcE5Wfo&list=PL0Ks75aof3Ti1GDgeePUkCJWn02c0VDA5&index=9)
- [Семинар. Языковые модели](https://www.youtube.com/watch?v=WoYRZEsWIrg&list=PL0Ks75aof3Ti1GDgeePUkCJWn02c0VDA5&index=8&ab_channel=DeepLearningSchool)


- Что делает языковая модель(LM)?
![](../for_readme/08_Language_Modelling/1.png)
- Пример работы языковой модели(варианты продолжения поискового вопроса)
![](../for_readme/08_Language_Modelling/2.png)
![](../for_readme/08_Language_Modelling/3.png)
- Существует 2 типа языковых моделей
![](../for_readme/08_Language_Modelling/4.png)
- Идея работы Count Based LM
![](../for_readme/08_Language_Modelling/5.png)
![](../for_readme/08_Language_Modelling/6.png)
![](../for_readme/08_Language_Modelling/7.png)
- Идея использовать не всю последоватьность слов, а лишь ближайшие n слов
![](../for_readme/08_Language_Modelling/8.png)
- Пример того, как строиться триграммая языковая модель
![](../for_readme/08_Language_Modelling/9.png)
- Как языковая модель генерирует текст
![](../for_readme/08_Language_Modelling/10.png)
- Оценка качества языковой модели
![](../for_readme/08_Language_Modelling/11.png)
![](../for_readme/08_Language_Modelling/12.png)
- Примерная архитектура Нейронной Языковой Модели(Neural LM)
![](../for_readme/08_Language_Modelling/13.png)
- Обучаем модель с помощью cross entropy loss
![](../for_readme/08_Language_Modelling/14.png)
- Neural LM на основне RNN(можно использовать любое кол-во слов предложении)
![](../for_readme/08_Language_Modelling/15.png)
- Neural LM на основе CNN(вынуждены использовать n ближайших слов)
![](../for_readme/08_Language_Modelling/16.png)
- Ещё одна архитектура Neural LM, позволяющая генерировать эмбеддинг целого предложения
![](../for_readme/08_Language_Modelling/16_1.png)
- Генерация "хороших" эмбеддингов предложений с помощью Neural LM 
![](../for_readme/08_Language_Modelling/17.png)