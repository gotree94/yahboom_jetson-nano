# 07. 이미지 분류 추론

## 개요
이미지 분류(Image Classification)를 실습합니다.

## 개념
입력 이미지를 미리 정의된 클래스 중 하나로 분류합니다.

## 실행 예시
```bash
imagenet --model=models/googlenet --input_blob=input_0 --output_blob=output_0 \
  images/cat.jpg output.jpg
```

## 응용
- 웹캠 실시간 분류
- 커스텀 이미지 분류

## 참고
- 원본 튜토리얼: https://www.yahboom.net/study/jetson-nano/6818
