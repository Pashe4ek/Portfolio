# Классификация комментариев 

## Описание проекта

Интернет-магазин «Викишоп» запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Магазину нужен инструмент, который будет искать токсичные комментарии и отправлять их на модерацию. 
Обучите модель классифицировать комментарии на позитивные и негативные. В вашем распоряжении набор данных с разметкой о токсичности правок.
Постройте модель со значением метрики качества F1 не меньше 0.75. 

## Описание данных

Данные находятся в файле /datasets/toxic_comments.csv. Скачать датасет. 
Столбец text в нём содержит текст комментария, а toxic — целевой признак.

## Навыки и инструементы

* pandas 
* nltk
* re
* lightgbm
* tqdm.notebook.tqdm
* nltk.corpus.stopwords.nltk_stopwords
* nltk.corpus.wordnet
* nltk.stem.WordNetLemmatizer 
* sklearn.feature_extraction.text.TfidfVectorizer
* sklearn.linear_model.LogisticRegression
* sklearn.tree.DecisionTreeClassifier
* sklearn.ensemble.RandomForestClassifier
* sklearn.model_selection.train_test_split
* sklearn.metrics.f1_score
* sklearn.utils.shuffle
* sklearn.model_selection.RandomizedSearchCV
* sklearn.metrics.f1_score
* sklearn.metrics.make_scorer
* sklearn.pipeline

## Вывод

В рузльатет проделанной работы было достигнуто, при помощи модели Линейной регресси, значение метрики F1 - 0.753 на тестовой выборке. Для токонизации текста использовался метод TfidfVectorizer, предварительно текст был преобразован при помощи метода WordNetLemmatizer