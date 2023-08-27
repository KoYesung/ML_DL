# 🤔얼굴 나이 예측 모델 구현하기


<h3>📌 과제 개요</h3>

- IMDB-WIKI의 이미지 데이터셋을 사용하여 연령을 예측하는 모델 구현하
- [데이터셋](https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/)

<h3>👩‍💻 과제 진행 과정</h3>

- 데이터 전처리
  - 파일 이름은 사진의 연도 + 인물의 태어난 연도로 나와있음 -> 나이 디렉토리 생성 및 이동
  - 데이터 이상치 제거 -> 사람이 아닌 경우, 두명 이상인 경우, 마스크를 낀 경우는 제거
  - 나이의 범위는 7 ~ 93으로 제한
- transform 정의(Resize, RandomAffine, RandomHorizontalFlip)
- DataLoader 생성
- 사용모델: CNN(EfficientB4을 사전학습한 모델에서 FC Layer 수정)


<h3>🪄TEST </h3>

- 모델 예측 값과 실제 나이를 TITLE로 표시
- 얼굴이 잘 보이는 사진을 사용
- 약간의 오차가 있지만 예측값과 실제값이 비슷함


![image](https://github.com/KoYesung/ML_DL/assets/131944189/41d34afc-b8c2-4040-abf8-1b3c7f32574d)



[발표자료 바로가기](https://github.com/KoYesung/ML_DL/blob/6c10b2982d8e3abcf02b6dc30e6ed6e93d0989aa/%EC%96%BC%EA%B5%B4%20%EB%82%98%EC%9D%B4%EC%98%88%EC%B8%A1%EB%AA%A8%EB%8D%B8/%EC%97%B0%EB%A0%B9%EC%97%90%EC%B8%A1%EB%AA%A8%EB%8D%B8_%EC%B5%9C%EC%A2%85%EB%B3%B8.pdf)
