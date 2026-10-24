# 04. TensorFlow 설치(선택)

## 개요
Jetson Nano에서 TensorFlow를 설치하는 방법을 다룹니다. (선택 과정)

## 권장 버전
JetPack 버전에 맞는 TensorFlow wheel을 사용해야 합니다.

## 설치 방법 (일반적)
NVIDIA에서 제공하는 Jetson용 TensorFlow 패키지를 사용하는 것이 가장 안정적입니다.

`ash
# 예시 (버전에 따라 상이)
pip3 install --extra-index-url https://developer.download.nvidia.com/compute/redist/jp/v461 tensorflow==2.7.0+nv22.1
`

## 확인
`python
import tensorflow as tf
print(tf.__version__)
`

## 주의사항
- 메모리 제한으로 인해 설치/학습 시 주의 필요
- 가능하면 가벼운 모델 사용 권장

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
