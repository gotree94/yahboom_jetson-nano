# 03. Jupyter Lab 및 JetCam 설치

## 개요
Jupyter Lab 환경에서 JetCam을 사용해 카메라를 쉽게 다루는 방법을 학습합니다.

## JetCam이란?
JetCam은 NVIDIA Jetson에서 카메라를 간편하게 사용하기 위한 Python 라이브러리입니다.

## 설치
`ash
cd ~
git clone https://github.com/NVIDIA-AI-IOT/jetcam
cd jetcam
sudo python3 setup.py install
`

## Jupyter Lab 설치
`ash
pip3 install jupyter jupyterlab
`

## 실행
`ash
jupyter lab --ip=0.0.0.0 --port=8888 --allow-root
`

## JetCam 사용 예시
`python
from jetcam.csi_camera import CSICamera
camera = CSICamera(width=224, height=224)
image = camera.read()
`

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
