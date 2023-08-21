# Проект: Отток клиентов

## Описание проекта

Из Банка стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.
Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Нам предоставлены исторические данные о поведении клиентов и расторжении договоров с банком. 
Необходимо пострить модель с предельно большим значением F1-меры. 
Дополнительно измеряйте AUC-ROC, сравнивайте её значение с F1-мерой.

## Навыки и инструменты

* pandas
* numpy
* matplotlib.pyplot
* sklearn.preprocessing.StandardScaler
* sklearn.model_selection.train_test_split
* sklearn.tree.DecisionTreeClassifier
* sklearn.ensemble.RandomForestClassifier
* sklearn.linear_model.LogisticRegression
* sklearn.metrics.f1_score
* sklearn.metrics.roc_auc_score
* sklearn.model_selection.RandomizedSearchCV
* sklearn.utils.shuffle
* sklearn.model_selection.GridSearchCV
* sklearn.metrics.roc_curve
* sklearn.preprocessing.OneHotEncoder
* sklearn.feature_selection.mutual_info_classif
* random.randrange
* tqdm

## Описание данных

Признаки: \
RowNumber — индекс строки в данных \
CustomerId — уникальный идентификатор клиента \
Surname — фамилия \
CreditScore — кредитный рейтинг \
Geography — страна проживания \
Gender — пол \
Age — возраст \
Tenure — сколько лет человек является клиентом банка \
Balance — баланс на счёте \
NumOfProducts — количество продуктов банка, используемых клиентом \
HasCrCard — наличие кредитной карты \
IsActiveMember — активность клиента \
EstimatedSalary — предполагаемая зарплата \
Целевой признак: \
Exited — факт ухода клиента

## Вывод

В результате проделанной работы мы построили модель со значением F1-меры - 0,608 на тестовой выборке. Мы использовали алгоритм RandomForestClassifier с гиперпарамметрами: Глубина(depth) -15,деревья(n_estimators) - 70, минимальное число объектов (min_samples_split) - 3
Ее можно использовать для прогнозирования, уйдёт клиент из банка в ближайшее время или нет.