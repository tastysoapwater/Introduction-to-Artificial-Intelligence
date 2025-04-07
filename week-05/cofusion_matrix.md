# 혼동 행렬 기반 주요 평가 지표 (Confusion Matrix Metrics)

머신러닝 분류 문제에서 모델의 성능을 평가하기 위해 혼동 행렬(Confusion Matrix)을 사용하며, 
이로부터 다양한 지표를 계산할 수 있다.
##  혼동 행렬 기본 형태

```
               실제 양성 (Positive)   실제 음성 (Negative)
예측 양성          TP (True Positive)     FP (False Positive)
예측 음성          FN (False Negative)    TN (True Negative)
```
---

## 1. Accuracy (정확도)

- 정의: 전체 데이터 중에서 올바르게 예측한 비율
- 공식:
  ```
  Accuracy = (TP + TN) / (TP + TN + FP + FN)
  ```
- 설명: 전체 예측 중 맞춘 비율이므로 직관적인 지표이다.
- 하지만 클래스 불균형이 클 경우 과대 평가될 수 있다.

---

## 2. Precision (정밀도)

- 정의: 양성으로 예측한 것 중에서 실제로 양성인 비율
- 공식:
  ```
  Precision = TP / (TP + FP)
  ```
- 설명: False Positive(실제로는 음성인데 양성이라 예측)를 줄이는 데 초점을 둔다.

---

## 3. Recall / Sensitivity (재현율 / 민감도)

- 정의: 실제 양성 중에서 올바르게 예측한 비율
- 공식:
  ```
  Recall = TP / (TP + FN)
  ```
- 설명: False Negative(실제로는 양성인데 음성으로 예측)를 줄이는 데 집중한다.
---

## 4. F1 Score

- 정의: Precision과 Recall의 조화 평균
- 공식:
  ```
  F1 Score = 2 * (Precision * Recall) / (Precision + Recall)
  ```
- 설명: Precision과 Recall 사이의 균형이 중요할 때 사용한다.
- 두 값이 비슷할 때 F1이 높으며, 둘 중 하나가 낮으면 F1도 낮아진다.

---


