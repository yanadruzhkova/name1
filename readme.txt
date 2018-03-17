1. Скачать датасет DeepFashion 
http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion/AttributePrediction.html

Структура датасета выглядит следующим образом:
---Anno
------list_attr_cloth.txt
------list_attr_img.txt
------list_bbox.txt
------list_category_cloth.txt
------list_category_img.txt
------list_landmarks.txt
---Eval
------list_eval_partition.txt
---Img
------img

Необходимо положить все скачанные папки в fashion_data/

2. Создаем датасет для работы
Применим селективный поиск, чтобы найти ограничивающие поля для каждого изображения. Обрезаем по ним картинку и копируем внутрь папки dataset.
Для запуска:
python dataset_create.py

3. Проводим обучение модели
python train.py

4. Предсказываем тип одежды на фотографии и рисуем область, где она находится. 
python predict.py