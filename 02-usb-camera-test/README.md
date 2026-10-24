# 02. USB 외장 카메라 테스트

## 개요
USB 웹캠을 Jetson Nano에 연결하여 테스트하는 방법을 학습합니다.

## 준비물
- USB 웹캠 (UVC 호환 권장)
- Jetson Nano

## 카메라 확인

```bash
lsusb
v4l2-ctl --list-devices
```

## 테스트

```bash
# Cheese 등 GUI 도구
cheese
```

GStreamer 사용:

```bash
gst-launch-1.0 v4l2src device=/dev/video0 ! videoconvert ! xvimagesink
```

Python + OpenCV:

```python
import cv2
cap = cv2.VideoCapture(0)
while True:
    ret, frame = cap.read()
    if not ret: break
    cv2.imshow('USB Cam', frame)
    if cv2.waitKey(1) & 0xFF == ord('q'): break
cap.release()
cv2.destroyAllWindows()
```

## 주의사항
- 해상도/프레임레이트 호환성 확인
- 일부 USB 카메라는 추가 설정 필요

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
