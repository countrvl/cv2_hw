# 🧠 Итоговый отчёт по заданию: Алгоритм NMS и дообучение модели детекции

## ✅ Часть 1. Построение алгоритма NMS

- Реализована функция `non_max_suppression` на Python.
- Используется своя функция `IoU`.
- Тестирование на синтетических данных с визуализацией до/после NMS.

---

## ✅ Часть 2. Дообучение модели на `coco128`

- Использована предобученная модель: `yolov8n.pt`
- Обучение на `coco128`:
  - `epochs=10`
  - `imgsz=640`
  - `device=0` (CUDA: RTX 4070 SUPER)
- Сохранены результаты обучения и метрики (`runs/detect/train*/`):
  - `confusion_matrix.png`
  - `F1_curve.png`
  - `PR_curve.png`

---

## ✅ Часть 3. Аугментации изображений и боксов

Использована библиотека `albumentations`. Для каждой аугментации визуально показано:

- 🔄 `HorizontalFlip`
- 🔁 `Rotate`
- ☀️ `RandomBrightnessContrast`
- 🔍 `RandomScale`

### HorizontalFlip

![HorizontalFlip](aug_HorizontalFlip.jpg)

### Rotate

![Rotate](aug_Rotate.jpg)

### Brightness & Contrast

![BrightnessContrast](aug_BrightnessContrast.jpg)

### Random Scale

![RandomScale](aug_RandomScale.jpg)


---

📄 Код задания: `hw2_NMS.ipynb`
