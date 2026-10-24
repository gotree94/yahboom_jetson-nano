# 31. 모델 변환

## 개요
YOLOv11 모델을 Jetson에 최적화된 형식으로 변환합니다.

## 변환 경로
- PyTorch (.pt) → ONNX
- ONNX → TensorRT (.engine)

## CLI 예시
```bash
yolo export model=yolo11n.pt format=onnx
# TensorRT 변환은 trtexec 또는 ultralytics export format=engine 사용
yolo export model=yolo11n.pt format=engine device=0
```

## 주의사항
- Jetson Nano 메모리 제약 고려
- batch size, half precision 설정 확인

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
