# Модель машинного обучения, предсказывающая уход клиентов оператора связи

## Проект выполнен в качестве финальной работы на курсе по Data Science  от Yandex Practicum

**Описание проекта:** Оператору связи «Ниединогоразрыва.ком» необходимо предсказывать отток клиентов. Если согласно предсказанию, пользователь планирует уйти, ему должны быть предложены промокоды и специальные условия. Для предсказания требуется разработать качественную модель машинного обучения с метрикой ROC-AUC на тестовой выборке в 0.85. Помимо ROC-AUC необходимо предоставить интерпретируемую метрику, такие как accuracy и матрица ошибок.

**Цель работы** - построить модель машинного обучения, предсказывающая уход клиентов оператора, при чем метрика ROC-AUC на тестовой выборке должна составлять не менее 0.85.

**Выполненные задачи**:

- Первоначальное ознакомление с данными
- Объединение данных
- Выделение целевого признака
- Исследование и обработка данных
- Удаление и создание признаков
- Корреляционный анализ
- Разбиение датасета на обучающую и тестовую выборки
- Кодирование и масштабирование признаков
- Выбор и обучение разных моделей машинного обучения на кросс-валидации
- Выбор лучшей модели по метрике ROC-AUC на кросс-валидации
- Оценка качества лучшей модели на тестовой выборке
- Построение и анализ ROC-кривой, accuracy, матрицы ошибок и важности признаков лучшей модели на тестовой выборке.
- Отчет о проделанной работе

#### Выводы по проекту:
Построенная модель машинного обучения LightGBMClassifier эффективно справляется с предсказанием ухода клиентов от оператора связи «Ниединогоразрыва.ком» со значением метрики ROC-AUC в 0.92, что выше поставленной задачи - "метрика ROC-AUC на тестовой выборке должна составлять не менее 0.85". Высокое качество предсказания модели получилось достичь за счет устранения мультиколлиарности, удаления избыточных признаков и признаков, имеющих высокую корреляцию с целевым признаком. Для предотвращения утечки данных в модели используются конвейеры (pipeline) для кодирования и масштабирования признаков.
Также модель дала возможность определить наиболее важные признаки: близость окончания ежемесячного договора, длительность обслуживания клиента, ежемесячные траты на услуги, потраченные деньги на услуги. Заказчику рекомендуется обратить внимание на эти признаки, влияя на которые можно снизить вероятность ухода клиентов.
Модель машинного обучения рекомендуется к вводу в экслуатацию.

#
# A machine learning model able to predict the departure of telecom operator customers

## The project was completed as the final work in the Data Science course from Yandex Practicum

**Description of project:** The telecom operator “Niedinogorazryva.com” needs to predict customers' outflow. According to the prediction, if the user plans to leave, he should be offered promotional codes and special conditions. For prediction, it is necessary to develop a high-quality ML model with a ROC-AUC metric on a test sample of 0.85. In addition to ROC-AUC, interpretable metrics such as accuracy and error matrix should be provided.

**The goal of work** is to build a ML model able to predict the departure of telecom operator customers, and the ROC-AUC metric on the test sample should be at least 0.85.

**Completed tasks**:

- Initial familiarization with the data
- Data merging
- Isolation of the target feature
- Data analysis and processing
- Removing and creating features
- Correlation analysis
- Splitting the dataset into training and test samples
- Feature encoding and scaling
- Selection and training of different machine learning models with cross-validation
- Selecting the best model based on the ROC-AUC metric with cross-validation
- Assessing the quality of the best model on the test sample
- Construction and analysis of the ROC curve, accuracy, error matrix and importance of features for the best model on test sample.
- Progress report

#### Project Conclusions:
The constructed LightGBMClassifier machine learning model effectively copes with predicting clients' departure from the telecom operator “Niedinogorazryva.com” with a ROC-AUC metric value of 0.92, which is higher than the set requirement - “the ROC-AUC metric on the test sample should be at least 0.85.” A high quality of model prediction was achieved by eliminating multicolliarity, removing redundant features, and removing features having a high correlation with the target. To prevent data leakage, the model uses pipelines to encode and scale features.
The model also made it possible to determine the most important features: the proximity of the monthly contract end, the client’s service duration, monthly expenses for services, and money spent on services. 
The contracting authority is recommended to pay attention to these features, which can reduce the likelihood of customers leaving.
The machine learning model is recommended for implementation.
