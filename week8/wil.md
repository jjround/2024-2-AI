# 인공지능 스터디 8주차 WIL
## 8주차 스터디 목표
8주차의 테마인 Attention 메커니즘과 이를 활용한 Vision Transformer(ViT)에 대해 이해해보자
## 8주차 키워드
Attention(어텐션), Self-Attention(자기-어텐션), Multi-Head Attention(다중 헤드 어텐션), Vision Transformer(ViT, 비전 트랜스포머)
### Attention
- Attention 메커니즘의 정의  
Attention은 입력 데이터의 서로 다른 부분들 간의 관련성을 계산하는 메커니즘으로, 중요한 데이터를 강조하고 덜 중요한 데이터를 약화시켜 모델의 성능을 향상시킨다.
Seq2Seq 모델에서 정보 압축 문제와 정보 손실을 해결하기 위해 처음 제안되었으며, 각 단어와 연관성이 높은 부분에 집중하도록 설계되었다.  
- Attention의 주요 구성 요소  
Query (Q): 현재 집중해야 할 대상  
Key (K): 데이터의 각 요소에 대한 표현  
Value (V): Key와 관련된 데이터  
Attention Score: Query와 Key 간의 유사도 점수로, 특정 값에 집중할 정도를 나타냄
#### Self Attention
입력 시퀀스의 각 위치가 동일한 시퀀스 내의 다른 위치에 얼마나 집중해야 하는지 계산하는 메커니즘으로, NLP뿐만 아니라 Computer Vision에서도 사용된다.
### Multi-Head Attention
Attention을 여러 번 병렬적으로 수행하여 다양한 관점에서 정보를 학습할 수 있도록 한다.
### Vision Transformer (ViT)
ViT는 Attention 메커니즘을 Vision 분야에 적용한 모델로, 이미지를 패치 단위로 나누고 Self-Attention을 활용하여 이미지 분류를 수행한다.
ViT의 성능은 Image Classification에서 SoTA(State of the Art)를 기록했으며, 특히 Explainable AI(XAI) 분야에서도 주목받고 있다.
## 추가학습
ViT의 학습 방식에 대해 더 공부해봐야겠다.
## 느낀점
Attention 메커니즘이 Seq2Seq에서 시작해 NLP와 Vision 분야 전반으로 확장된 과정을 배우며 AI 모델의 발전 방향을 이해할 수 있었다. 특히, ViT와 CNN 간의 비교를 통해 모델 선택 시 고려해야 할 점들을 배울 수 있었다.