# 26. 물체 감지

## 개요
YOLOv11으로 객체 탐지를 수행합니다.

## 실시간 예제
`ash
yolo predict model=yolo11n.pt source=0 show=True
`

## Python API
`python
from ultralytics import YOLO
model = YOLO('yolo11n.pt')
results = model.predict(source=0, show=True)
`

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
