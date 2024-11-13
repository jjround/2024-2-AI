# 인공지능 스터디 7주차 WIL
## 7주차 스터디 목표
7주차의 테마인 Object Detection의 주요 개념과 모델의 발전 과정을 알아보자.
## 5주차 키워드
Object Detection(객체 검출), Two-stage Detector, One-stage Detector, Feature Pyramid Network (FPN)
### Object Detection
Object Detection은 이미지 속 객체를 찾아내고, 해당 객체의 위치와 종류를 예측하는 작업임. Classification(분류)과 Localization(위치 파악)을 결합한 형태로 볼 수 있음.
### Two-stage Detector
Two-stage Detector는 객체 검출을 두 단계로 수행하는 모델임. 먼저 객체가 있을 가능성이 높은 영역(Region Proposal)을 찾고, 해당 영역에서 객체를 분류하고 위치를 정확하게 예측함.

- R-CNN: Selective Search 알고리즘을 통해 후보 영역을 찾고, 각 영역을 CNN으로 처리하여 SVM으로 분류하는 방식임. CNN을 여러 번 실행해야 하므로 연산 비용이 높음.
- Fast R-CNN: 이미지 전체를 CNN으로 처리한 후, 필요한 영역에서 특징 맵을 ROI Pooling을 통해 추출하여 분류와 BBox 회귀를 수행함. R-CNN보다 속도가 빨라졌음.
- Faster R-CNN: RPN(Region Proposal Network)을 도입하여 Selective Search 대신 CNN 기반으로 후보 영역을 생성함. Two-stage Detector 모델의 속도와 효율성이 크게 개선됨.
### One-stage Detector
One-stage Detector는 객체 검출과 분류를 동시에 수행하여 연산 속도를 높임. 대표적인 모델은 YOLO (You Only Look Once) 시리즈로, 빠른 속도가 장점이지만 초기 버전에서는 정확도가 다소 낮았음. 이후 YOLO v2, v3 등의 개선된 버전들이 나오며 정확도와 속도가 모두 향상됨.
### Feature Pyramid Network (FPN)
FPN은 다양한 해상도의 특징 맵을 결합하여 서로 다른 크기의 객체를 검출할 수 있도록 함. Convolutional Network에서 얻은 여러 해상도의 특징 맵을 피라미드 형태로 쌓아 다양한 크기의 객체에 대응할 수 있도록 설계됨. 작은 객체와 큰 객체 모두 잘 검출할 수 있게 됨.
## 추가학습
Object Detection 성능을 높이기 위해, **Non-Max Suppression(NMS)** 과 **Intersection over Union(IoU)** 에 대해 추가로 학습할 예정임. 특히 NMS는 겹치는 Bounding Box를 정리하는 중요한 기법임.

## 느낀점
단순 분류보다 객체 검출은 더 복잡한 과제임을 알게 됨. 다양한 모델들이 발전하면서 속도와 정확도 모두 개선되고, 실시간 애플리케이션에 적합한 모델들이 많이 연구되고 있다는 점이 흥미로웠음. 앞으로 객체 검출이 실제 환경에서 어떻게 응용될 수 있을지 기대됨.