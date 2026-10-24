# 19. YOLOv5 + TensorRT 가속

## 개요
TensorRT로 모델을 최적화하여 추론 속도를 향상시킵니다.

## 방법
- PyTorch 모델(.pt) → ONNX 변환
- ONNX → TensorRT 엔진(.engine) 변환
- 엔진으로 추론

## 기대효과
Jetson Nano에서 FPS 향상

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
