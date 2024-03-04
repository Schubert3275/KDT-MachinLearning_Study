### 1. 기계학습 프로세스에 대해 간략하게 설명하세요.

> 데이터 수집 -> 데이터 전처리 -> 모델 학습 -> 모델 평가 -> 결과 예측 및 사용

### 2. 기계학습에 사용되는 데이터셋에 대해 설명하세요.

> 학습용 데이터셋 :
>
> > 모델을 학습시키기 위한 데이터셋으로, 해당 데이터셋(Feature)에 대한 결과(Target)가 함께 주어진다.

> 평가용 데이터셋 :
>
> > 모델의 학습 정도를 판단하기 위한 데이터셋으로 학습용 데이터셋과 동일한 형태이나 학습용 데이터셋에 포함되지 않는 데이터셋을 사용한다.

> 결과용 데이터셋 :
>
> > 실제 결과를 출력하기 위한 데이터셋으로 임의의 데이터로 이루어져 결과가 포함되지 않은 데이터셋을 사용한다.

### 3. 지도학습의 특징을 설명하세요.

> 문제(Feature)와 답(Target)이 함께 주어져 학습시킬 때 해당 데이터셋에 대한 결과를 매칭시키는 방식으로 학습을 실시한다.
> 비지도 학습보다 더 단순하고 일반적이지만, 학습을 위해 미리 답을 알고 있어야 할 필요가 있으며 문제와 답을 미리 매칭시켜 분류시킨 데이터를 사용해야 한다.

### 4. 데이터 전처리 중 처음 데이터 수집 후 데이터 정제하는 과정에 진행되는 작업을 설명하세요.

> 데이터 형태 확인 :
>
> > 데이터의 형태와 실제 해당 데이터의 형태를 비교하여 차이나는 부분을 실제에 맞게 수정한다.

> 데이터 결측치 확인 :
>
> > 데이터의 결측치를 확인하여 결측치가 있는 경우 결측치를 제거하거나 평균값, 주변값, 중앙값 등으로 대체한다.

> 데이터 이상치 확인 :
>
> > 데이터의 이상치를 확인하여 이상치가 단순 입력오류일 경우 제거하지만 실제 특이성을 지닌 데이터인 경우 제거할지 아니면 어느 범위까지는 사용할지를 결정한다.

> 데이터 스케일링:
>
> > 데이터의 크기들이 일정하지 않을 경우 데이터들의 크기를 일정하게 만들어 모델의 학습을 돕는다.

### 5. 모델 개념을 설명해 주세요.

> 데이터를 학습시키기 위한 여러가지 수단으로, 다양한 공식에 따라 학습을 진행하는 과정을 함수화시켜 미리 만들어 놓은 것을 말한다.

### 6. 모델의 결과 값이 수치를 예측해주는 기계학습은 무엇인가요?

> 분류형 모델(Classification Model)

### 7. 모델 파라미터는 무엇인가요?

> 모델이 학습한 데이터로부터 얻어지는 파라미터.

### 8. KNN 알고리즘에 대해 설명해 주세요.

> 주어진 데이터에 대한 거리를 측정하여 결과를 도출하는 알고리즘으로, 주어진 데이터와 가장 가까이 있는 K개의 데이터를 찾아 그 중 가장 많이 나오는 결과(분류형)를 예측하거나 해당 데이터의 평균으로 결과(회귀형)를 예측한다.

### 9. 하이퍼 파라미터는 무엇인가요?

> 모델의 성능을 개선시키기 위해 인스턴스 생성 단계에서 변화시키는 파라미터.

### 10. Regression의 성능평가 지표들을 설명하세요.

> recall_score
>
> > 재현율을 표현하는 지표로 정답에 대한 정확도를 측정한다.

> precision_score
>
> > 정밀도를 표현하는 지표로 예측에 대한 정확도를 측정한다.

> f1_score
>
> > 재현율과 정밀도의 조화평균으로 모델의 성능을 측정한다.

### 11. LinearRegression 알고리즘에 대해 설명해 주세요.

> 선형회귀분석 알고리즘으로, 선형회귀분석 공식을 사용하여 가중치와 절편을 구해 데이터를 예측한다.

### 12. Classification의 성능평가 지표들을 설명하세요.

> mean_absolute_error
>
> > 오차의 평균을 구해 정확도를 측정한다.

> mean_squared_error
>
> > 오차의 제곱으로 정확도를 측정한다.

> root_mean_squared_error
>
> > 오차의 제곱에 대한 제곱근으로 정확도를 측정한다.

### 13. 피쳐공학에 대해 설명하세요.

> 주어진 피쳐만으로 올바른 학습이 힘들거나 주어진 피쳐가 지나치게 많아 학습이 힘들 경우 피쳐를 변형시키거나 새로운 피쳐를 만들어 학습을 돕는 방법을 말한다.

### 14. LogisticRegression 알고리즘에 대해 설명해 주세요.

> 시고모이드 곡선을 통해 타겟이 어느 그룹에 속해있는지를 분석하여 결과를 도출해내는 알고리즘을 말한다.
> 이진분류 또는 다중 분류로 결과를 도출해낸다.

### 15. 과대적합/과소적합에 대해 설명해 주세요.

> 과대적합
>
> > 학습용 데이터에 대한 결과는 높지만 테스트용 데이터에 대한 결과는 낮게 나오는 등 두 가지 테스트 결과가 지나치게 상이할 경우를 말한다.

> 과소적합
>
> > 학습용 데이터에 대한 결과와 테스트용 데이터에 대한 결과가 모두 낮을 경우를 말한다.

### 16. 아래 데이터셋을 기반으로 분류/회귀 모델을 완성 후 성능평가까지 구현하세요.

-   : iris.csv 데이터셋
-   조건
    -   : 3 2 분류 개 품종 중 개 선택하여 이진 분류 진행
    -   : 3 1 , 4 회귀 개 품종 중 개 선택 개 피쳐 중 꽃잎의 길이값 예측 회귀

> iris_ML-TEST.ipynb