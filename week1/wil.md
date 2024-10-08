# 인공지능 스터디 1주차 WIL
## 1주차 스터디 목표
인공지능 분야에 문외한인 내가 앞으로 배울 내용의 큰 틀이 어떤 것들이 있는지 이해하고 진행과정에 대해 배워보자.
## 1주차 키워드
AI, Learning, Deep Learning Component, Perceptron
### 1.**AI**
- AI>ML>DL (상위개념->하위개념)
* AI
* Artificial Intelligence, 인간의 지능과 연관된 ***인지문제의 해결***
- ML
- Machine Learning, *데이터로부터* ***특징을 학습하는 알고리즘***
* DL
* Deep Learning, *신경망을 기반으로* ***특징을 학습하는 알고리즘***
### 2.**Learning**
#### 학습(머신러닝 기법)
- 지도 학습
- Supervised Learning, 라벨이 있는 데이터를 사용해 입력과 출력 간의 관계를 학습
* 비지도 학습
* Unsupervised Learning, 라벨이 없는 데이터를 사용하여 데이터의 패턴이나 구조를 발견, 학습
- 준지도 학습
- Semi-supervised Learning, 적은 양의 라벨이 있는 데이터와 많은 양의 라벨이 없는 데이터를 함께 사용하여 학습
* 자가지도 학습
* Self-supervised Learning, 라벨이 없는 데이터를 사용하여 모델이 스스로 라벨을 생성하거나 학습
- **라벨(label)**- 데이터에 부여된 정답(출력값) 또는 분류 정보
- ex) 사진에 고양이라는 라벨이 붙어있으면 모델은 이 사진을 고양이라고 학습함.
+ 학습의 주체는 **모델**, 데이터를 학습하여 특정 작업을 수행하는 수학적/알고리즘적 구조이다
### 3.**Deep Learning Component**
#### 1.Data
- 딥러닝 모델이 학습하는데 사용하는 입력 자료
- 데이터의 양과 품질에 따라 모델의 성능이 좌우됨
- 학습 데이터, 검증 데이터, 테스트 데이터
#### 2.Model
- 입력 데이터를 받아 작업을 수행하는 알고리즘
- 여러 층의 *신경망*으로 구성되어 있으며, 각 층은 입력 데이터를 더 복잡한 특징으로 변환
- 모델의 구조(층의 수 등)가 성능과 학습 속도에 영향을 줌
#### 3.Loss Function
- 손실 함수
- 모델의 예측값과 실제값을 비교하여 모델의 학습 수준을 파악하는데 사용하는 함수
### 4.**Perceprton**
- 퍼셉트론
- 이진 분류 모델을 학습하기 위한 지도 학습 기반의 알고리즘
#### (단층)퍼셉트론의 시행
1. 두 클래스의 데이터 포인트를 그래프에 표현(2차원 이상의 차원에서)(=Feature 값을 뽑는다)
2. 선을 랜덤하게 그어보며 두 클래스를 가장 잘 나누는 선을 찾는다.(단층 퍼셉트론)
3. 단층 퍼셉트론으로는 XOR 문제와 같이 선 하나로 문제해결을 하지 못하는 경우가 발생
4. 따라서 층을 늘려 문제를 해결하는 다층 퍼셉트론을 사용
#### 다층 퍼셉트론의 시행
1. 두 그룹을 가장 잘 나누는 decision boundary를 찾아야 함
2. 단층 퍼셉트론과 다르게 다층 퍼셉트론은 비선형적 특성을 가짐
3. 가중치와 편향을 무작위로 설정한 후 데이터 학습을 통해 업데이트함
## 추가 학습
계속해서 등장하는 신경망에 대한 추가 학습을 해봤다.
#### 신경망
- 인공신경망(Artificial Neural Network)과 신경망은 같은 개념을 가리킴
- 입력 데이터와 출력 데이터의 관계를 모델링하고 학습하는 알고리즘
- 신경망의 각 층은 뉴런으로 구성되고, 뉴런 간의 연결에는 가중치와 편향이라는 매개변수가 작용함
- 다층 퍼셉트론도 인공신경망이고, 다른 신경망으로는 합성곱 신경망, 순환 신경망 등이 있음
## 느낀점
아무것도 모른채로 혼자 공부하는 것보다 공부의 방향성을 잡을 수 있다고 생각해 스터디에 참여하기 잘했다고 생각한다. WIL을 처음 작성해보며 앞으로 마크다운 문법을 자유롭게 활용할 수 있도록 연습해야겠다는 생각을 했다.