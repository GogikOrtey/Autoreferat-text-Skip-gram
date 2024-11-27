### Реализация алгоритма автореферирования текста Skip-gram

Данный алгоритм основан на обученной модели нейросети, работающей на ядре Word2Vec  
Оно представляет все слова текста в виде векторов, и таким образом может предсказывать их появление

В отличие от стандартных алгоритмов нейросетей, которые предсказывают текущее слово исходя из окружающего его контекста, архитектура типа Skip-gram действует наоборот: она использует текущее слово, чтобы предугадывать окружающие его слова

Достаточно обучить такую модель на нужном нам тексте (полная версия большого текста), а затем - попросить составить окружающий контекст для одного, например самого важного слова  

Если мы укажем ширину окна контекста 10, то на выходе получим предложение из 21 слова - 10 справа, и 10 слева будут сгенерированы

Так мы получим реферат большого текста, по одному ключевому слову
