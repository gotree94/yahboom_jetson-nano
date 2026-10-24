# 30. 방향성 경계 상자 감지

## 개요
OBB (Oriented Bounding Box)로 회전된 객체를 탐지합니다.

## 실행
`ash
yolo predict model=yolo11n-obb.pt source='image.jpg' show=True
`

## 활용
- 항공영상, 도로 표지판 등 회전된 객체

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
