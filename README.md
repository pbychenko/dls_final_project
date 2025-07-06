# Решение задачи Face Recognition

## Описание:
Данный репозиторий содержит реализацию итогового проекта по распознованию лиц для курса Deep Learning (семестр 1, весна 2025). 

## Файлы:
* **identity_CelebA.csv** — содержит картинки и id личностей
* **identity_CelebA_mini.csv** — подмножество из identity_CelebA.csv, данные которого используются для обучения и валидации моделей. Более подробно в **0. Подготовка данных.ipynb**
* **list_landmarks_align_celeba.csv** — содержит картинки и координаты ключевых точек на них
* **list_landmarks_align_celeba_mini.csv** — подмножество из list_landmarks_align_celeba.csv, данные которого используются для обучения и валидации моделей. Более подробно в **0. Подготовка данных.ipynb**
* **img_align_celeba_mini.zip** — подмножество из **img_align_celeba** (который можно скачать из https://drive.google.com/drive/folders/0B7EVK8r0v71pTUZsaXdaSnZBZzg?resourcekey=0-rJlzl934LzC-Xp28GeIBzQ, но я не стал его добавлять в гитхаб, так как много весит), которое используются для обучения и валидации моделей. Более подробно в **0. Подготовка данных.ipynb**
* **best_stacked_hourglass_model.pth** — веса для модели StackedHourglassNetwork
* **best_classification_model_with_cross_entropy.pth** — веса для модели, обученнной с CrossEntropy
* **best_classification_model_with_arc_face.pth** — веса для модели, обученнной c ArcFace
* **best_classification_model_with_triplet_loss.pth** — веса для модели, обученнной c TripletLoss и рандомным выбором триплетов
* **best_classification_model_with_semi_hard_mining_triplet_loss.pth** — веса для модели, обученнной c TripletLoss и "semi hard" выбором триплетов
* **yolov10n-face.pt** — детектор лиц


## Порядок чтения:
* **0. Подготовка данных.ipynb**
* **1. Реализация и обучение Stacked_Hourglass_Network .ipynb**
* **2. Реализация ArcFaceLoss и классификация с ArcFaceLoss и CrossEntropy.ipynb**
* **3. Реализация Triplet Loss и классификация с Triplet Loss.ipynb** 
* **4. Реализация Identificaton rate metric.ipynb**
* **5. Пайплайн для демонстрации.ipynb**