# 18. YOLOv5 실시간 감지

## 개요
웹캠/CSI 카메라로 실시간 객체 탐지를 수행합니다.

## 실행
```bash
python3 detect.py --weights yolov5s.pt --source 0  # USB
python3 detect.py --weights yolov5s.pt --source /dev/video0
```

## 성능 최적화
- 작은 모델(yolov5n/s) 사용
- 해상도 조정

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
