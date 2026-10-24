# 21. MediaPipe 환경 구축(선택)

## 개요
Google MediaPipe를 Jetson Nano에 설치합니다.

## 설치 방법
- pip로 설치 (버전 호환성 확인)
- 소스 빌드 (필요시)

`ash
pip3 install mediapipe
`

## 확인
`python
import mediapipe as mp
print(mp.__version__)
`

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
