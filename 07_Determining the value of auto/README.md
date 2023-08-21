# Определение стоимости автомобилей

## Описание проекта

Сервис по продаже автомобилей с пробегом «Не бит, не крашен» разрабатывает приложение, чтобы привлечь новых клиентов. В нём можно будет узнать рыночную стоимость своего автомобиля. \
Постройте модель, которая умеет её определять. В вашем распоряжении данные о технических характеристиках, комплектации и ценах других автомобилей.
Критерии, которые важны заказчику:
качество предсказания;
время обучения модели;
время предсказания модели.

## Описание данных

Признаки: \
DateCrawled — дата скачивания анкеты из базы \
VehicleType — тип автомобильного кузова \
RegistrationYear — год регистрации автомобиля \
Gearbox — тип коробки передач \
Power — мощность (л. с.) \
Model — модель автомобиля \
Kilometer — пробег (км) \
RegistrationMonth — месяц регистрации автомобиля \
FuelType — тип топлива \
Brand — марка автомобиля \
Repaired — была машина в ремонте или нет \
DateCreated — дата создания анкеты \
NumberOfPictures — количество фотографий автомобиля \
PostalCode — почтовый индекс владельца анкеты (пользователя) \
LastSeen — дата последней активности пользователя \
Целевой признак: \
Price — цена (евро) 

## Навыки и инструменты

* pandas
* statistics.mode
* time
* numpy
* lightgbm
* sklearn.model_selection.train_test_split
* sklearn.ensemble.RandomForestRegressor
* sklearn.tree.DecisionTreeRegressor
* sklearn.preprocessing.StandardScaler
* sklearn.preprocessing.OrdinalEncoder
* sklearn.metrics.mean_squared_error
* sklearn.model_selection.GridSearchCV
* sklearn.metrics.make_scorer

## Вывод:

Самой лучшей моделью для определения стоимости автомобиля стала модель линейной регрессии с гиперпараметрами: \
learning_rate': 0.1 \
max_depth: 7 \
num_leaves: 90 \
RMSE на тесте составил 1588.67
