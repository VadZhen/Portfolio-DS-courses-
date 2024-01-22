# Классификация изображений
## Kaggle соревнование "Journey to Springfield" (https://www.kaggle.com/competitions/journey-springfield)
№ Kaggle team: Vadim_Bolshev_650024495

### В соревновании участвовал в процессе обучения на курсе по Deep Learning от Школа глубокого обучения, МФТИ

Сериал "Симпсоны" идет на телеэкранах более 25 лет, и за это время скопилось очень много видеоматериала. Персонажи менялись вместе с изменяющимися графическими технологиями, и Гомер Симпсон-2018 не очень похож на Гомера Симпсона-1989. В этом проекте основное задание - это обучить классификатор на основе сверточных сетей, чтобы научиться отличать всех жителей Спрингфилда.
Метрикой в этом соревновании является Mean F1-Score. F1-мера вычисляется на основе точности и полноты.

### **Результаты соревнования:**
В качестве классификатора изображений была выбрана предобученная сверточная сеть inception_v3, была проведена аугементация подаваемых на модель изображений и использован scheduler для плавного уменьшения скорости обучения оптимизатора. На валидационной выборке данный классификатор позволил добиться  Accuracy в 0.9818, при чем минумум loss удалось достичь уже на 18 эпохе. F1 score на валидационной выборке составил 1.0. Итоговый F1 Score на Kaggle (на тестовой выборке) составил 0.98831, что говорит о высоком качестве предсказания обученного классификатора.


#
# Image Classification
## Kaggle Competition "Journey to Springfield" (https://www.kaggle.com/competitions/journey-springfield)
# Kaggle team: Vadim_Bolshev_650024495

### I participated the competition during the Deep Learning course from the with Deep Learning School, MIPT.

The Simpsons series has been on television for more than 25 years, and during this time a lot of video material has accumulated. Characters have changed along with changing graphics technology, and 2018 Homer Simpson doesn't look much like 1989 Homer Simpson. In this project, the main task is to train a classifier based on convolutional networks to learn how to distinguish all the residents of Springfield.

The metric for this competition is the Mean F1-Score. The F1 measure is calculated based on precision and recall.

### **Competition Results:**
The pre-trained convolutional network inception_v3 was chosen as an image classifier. The augmented images were fed to the model and a scheduler was used to smoothly reduce the learning rate of optimizer. The classifier allowed achieving the Accuracy of 0.9818 within the validation set while the minimum Loss was achieved already at the 18th epoch. F1 score within the validation set was 1.0. The final F1 Score on Kaggle (within test sample) was 0.98831, which indicates the high prediction quality of the trained classifier.
