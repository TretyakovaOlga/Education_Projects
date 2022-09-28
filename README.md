# Учебные проекты
_______

## NLP: Определение токсичности комментариев
(ссылка)</br>
**Задача:** построить модель для отсева токсичных комментариев. Метрика f1 - не менее 0.75.</br>
</br>
Для создания словаря используется размеченный набор с комментариями. Лемматизация проводится с помощью nltk. Для получения признаков использованы мешок слов, TF-IDF, биграммы и word2vec.</br>
Использованные модели: логистическая регрессия, LGBM, LinearSVC, метод ближайших соседей. Лучший результат получен на CountVectorizer + bigrams + LogisticRegression.
На базе трёх лучших моделей составлен решающий ансамбль, проведено тестирование. Итоговое f1 - 0.77.</br>
Библиотеки: nltk, sklearn, gensim, lightgbm </br>
</br>
</br>
## ML: Определение рыночной стоимости автомобиля
[Predict_of_car_prices.ipynb] https://github.com/TretyakovaOlga/Education-Projects-Description/blob/main/Predict_of_car_prices.ipynb </br>
**Задача:** разработать модель, которая будет предсказывать рыночную автомобиля в зависимости от его характеристик (сервис по размещению объявлений о продаже авто).
</br>
Модель разрабатывается на базе исторических данных о продажах автомобилей. Проведено исследование данных и предобработка: заполнение пропусков и удаление некорректных данных. Метрика RMSE. Рассмотрены линейные модели, метод ближайших соседей, CatBoost и LGBM, точность работы, скорость обучения и предсказания. Проведено тестирование.</br>
Библиотеки: sklearn, lightgbm, catboost</br>
</br>
</br>
## Анализ тарифов для оператора связа
(ссылка)
**Задача:** необходимо проанализировать поведение пользователей и определить более прибыльный тариф </br>
Проведен анализ поведения пользователей при пользовании услугами связи. Проверены гипотезы о различии средней выручки тарифов, а также о различии выручки в Москве и других регионах.
</br>
Библиотеки: numpy, scipy, matplotlib
