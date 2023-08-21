# Прогнозирование заказов такси

## Описание проекта

Компания собрала исторические данные о заказах такси в аэропортах. Чтобы привлекать больше водителей в период пиковой нагрузки, нужно спрогнозировать количество заказов такси на следующий час. Постройте модель для такого предсказания.
Значение метрики RMSE на тестовой выборке должно быть не больше 48.

## Навыки и инструменты

* pandas
* matplotlib.pyplot
* lightgbm
* statsmodels.tsa.seasonal.seasonal_decompose
* sklearn.ensemble.RandomForestRegressor
* sklearn.linear_model.LinearRegression
* sklearn.model_selection.train_test_split
* sklearn.metrics.mean_squared_error
* sklearn.metrics.make_scorer
* sklearn.model_selection.GridSearchCV
* sklearn.model_selection.RandomizedSearchCV
* sklearn.model_selection.cross_val_score
* sklearn.model_selection.TimeSeriesSplit

## Описание данных

Количество заказов находится в столбце 'num_orders' (от англ. number of orders, «число заказов»).

## Вывод

В результате проделанной работы была построена модель прогнозирования количества заказов такси. В модели мы использовали алгоритм LGBMRegressor с гиперпараметрами ('num_leaves': 65, 'max_depth': 7, 'learning_rate': 0.1) , на тестовой выборке модель показала RMSE - 41.85.