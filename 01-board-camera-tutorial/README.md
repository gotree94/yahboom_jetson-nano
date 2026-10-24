# 01. 보드 카메라 튜토리얼

## 개요
Yahboom Jetson Nano 4GB(B01/SUB)에 기본 탑재된 카메라 모듈을 사용하는 방법을 학습합니다.

## 대상 보드
- Yahboom Jetson Nano 4GB (B01)
- Yahboom Jetson Nano 4GB (SUB)

## 준비물
- Jetson Nano 보드
- CSI 카메라 모듈 (Yahboom 호환)
- 15핀 FPC 케이블
- 모니터, 키보드, 마우스

## 카메라 연결
1. Jetson Nano 전원을 끕니다.
2. CSI 카메라 커넥터를 엽니다.
3. FPC 케이블을 금속면이 위/아래 방향에 맞춰 연결합니다.
4. 커넥터를 잠급니다.

## 카메라 확인

```
ls /dev/video*
```

## 테스트 명령어

```
# 간단한 미리보기 (nvgstcapture)
nvgstcapture-1.0
```

또는 GStreamer를 사용한 테스트:

```
gst-launch-1.0 nvarguscamerasrc ! 'video/x-raw(memory:NVMM),width=1280,height=720,framerate=30/1' ! nvvidconv ! nvoverlaysink
```

## 트러블슈팅
- 카메라 인식 안됨: 케이블 방향/접촉 확인
- 화면 안나옴: 디스플레이 연결 확인
- 권한 문제: sudo 권한 필요

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
