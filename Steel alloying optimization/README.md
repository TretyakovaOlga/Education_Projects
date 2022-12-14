## Оптимизация производственного процесса легирования стали

**Цель**</br>
Разработка модели, позволяющей снизить затраты на процесс легирования стали путем снижения энергопотребления</br>
</br>

**Задача**</br>
На имеющихся исторических данных построить модель, которая будет прогнозировать температуру конечного расплава в зависимости от заданных параметров производственного процесса. Оптимизация достигается путем снижения энергозатрат за счёт предварительного подбора оптимальных условий легирования.</br>


### Вывод

В ходе работы над проектом:
- подготовлены данные - именены типы данных и названия колонок
- проведён исследовательский анализ данных, построены гистограммы, рассмотрены взаимосвязи величин
- данные подготовлены для построения модели, сведены в один датасет, разделены на тестовую и тренировочную выборки; рассмотрены два варианта планирования процесса заказчиком
- обучены 4 регрессионные модели - Lasso, Random Forest, LGBM, CatBoost
- проведено финальное тестирование
</br>
Лучший результат на кросс-валидации показал CatBoostRegressor. Для тестирования была выбрана модель, когда планирование легирования осуществляется через регулировку времени нагрева и подачи. MAE на кросс-валидации 5,77, на тестовой выборке - 5,68, т.е при прогнозировании температуры модель ошибается в среднем на 5,7 - 5,8 градуса (в рамках задачи измерения ведутся с округлением до целого, поэтому можно сказать, что модель ошибается на 6 градусов).
