# 25. CLI 사용

## 개요
YOLOv11 CLI 명령어 사용법을 학습합니다.

## 기본 명령
```bash
yolo predict model=yolo11n.pt source='image.jpg'
yolo predict model=yolo11n.pt source=0  # webcam
yolo train model=yolo11n.pt data=coco8.yaml epochs=100
yolo val model=yolo11n.pt
```

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
