# 17. YOLOv5 환경 구축(선택)

## 개요
YOLOv5 저장소를 클론하고 의존성을 설치합니다.

## 설치
`ash
git clone https://github.com/ultralytics/yolov5
cd yolov5
pip3 install -r requirements.txt
`

## 확인
`ash
python3 detect.py --weights yolov5s.pt --source 0
`

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
