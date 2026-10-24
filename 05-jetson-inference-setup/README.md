# 05. Jetson-inference 환경 구축(선택)

## 개요
jetson-inference는 NVIDIA에서 제공하는 딥러닝 추론 예제/라이브러리입니다.

## 저장소 클론
```bash
git clone --recursive https://github.com/dusty-nv/jetson-inference
cd jetson-inference
```

## 빌드
```b
mkdir build
cd build
cmake ../
make -j4
sudo make install
sudo ldconfig
```

## 모델 다운로드
빌드 과정 또는 스크립트를 통해 사전학습 모델을 다운로드합니다.

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
