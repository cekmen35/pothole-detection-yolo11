
# Pothole Detection with YOLO11

YOLO11s ile yol çukuru tespiti. Veri seti: Kaggle "Pothole Detection" (665 görüntü, PASCAL VOC).

## Test Sonuçları
| Precision | Recall | mAP50 | mAP50-95 |
|---|---|---|---|
| 0.799 | 0.717 | 0.802 | 0.491 |

![results](results.png)
![PR](PR_curve.png)
![confusion](confusion_matrix.png)

## Kullanım
```python
from ultralytics import YOLO
model = YOLO("best.pt")
model.predict("resim.jpg", save=True)
```

## Not
Veri seti repoya dahil değildir, Kaggle'dan indirilmelidir.# pothole-detection-yolo11
