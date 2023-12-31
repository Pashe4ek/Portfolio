# Определение возраста покупателей

## Описание проекта

Сетевой супермаркет «Хлеб-Соль» внедряет систему компьютерного зрения для обработки фотографий покупателей. Фотофиксация в прикассовой зоне поможет определять возраст клиентов, чтобы:
Анализировать покупки и предлагать товары, которые могут заинтересовать покупателей этой возрастной группы;
Контролировать добросовестность кассиров при продаже алкоголя.
Необходимо построить и обучить свёрточную нейронную сеть на датасете с фотографиями людей. Необходимо добится значения MAE на тестовой выборке не больше 8.

## Навыки и инструменты

* pandas
* matplotlib.pyplot
* seaborn
* numpy
* tensorflow.keras.preprocessing.image.ImageDataGenerator
* tensorflow.keras.applications.resnet.ResNet50
* tensorflow.keras.layers.Dense
* tensorflow.keras.layers.GlobalMaxPool2D
* tensorflow.keras.models.Sequential
* tensorflow.keras.optimizers.Adam

## Анализ обученной модели

Мы разработали модель для супермаркета, которая по фотографии покупателя может определит его примерный возраст. \
Для реализации данного проекта мы провели исследовательский анализ набора фотографий. Минимальный возраст 1 год, максимальный - 100 лет.  Средний возраст 31 год, медианный - 29 лет. Визуально, возраст людей на фотографиях, соотвествует указанному возрасту в датасете. \
В качестве модели мы использовали нейронную сеть с архитектурой ResNet50 и обучили ее на датасете с фотографиями людей \
Обученную модель мы проверили на тестовой выборке. Метрика MAE составила 6.4013 \
Минимальный порог метрики установленный заданием достигнут.

