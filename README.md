# Face Mask Detection Using YOLOv11

## Deskripsi
Proyek Computer Vision untuk mendeteksi penggunaan masker menggunakan model YOLOv11.

## Dataset
Dataset menggunakan Face Mask Detection Dataset format YOLO.

## Fitur
- Deteksi wajah menggunakan masker
- Deteksi wajah tanpa masker
- Prediksi gambar
- Training model YOLOv11

## Instalasi

```bash
pip install ultralytics
```

## Training

```python
from ultralytics import YOLO

model = YOLO("yolo11n.pt")

model.train(
    data="dataset/data.yaml",
    epochs=20,
    imgsz=640
)
```

## Prediksi

```python
model.predict("test.jpg")
```

## Hasil

Model terbaik disimpan pada

```
runs/detect/train/weights/best.pt
```

## Author

Naufal Zahid Musyaffa
