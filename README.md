# AI-Deep-Learning
Deep Learning by Python

### DeepBrick for Keras

#### Dataset
| Name | Description |
|:------|:------|
|`Input data, Labels`|1차원의 입력 데이터 및 라벨|
| `2D Input data` | 2차원의 입력 데이터, 주로 영상 데이터를 의미하며 샘플수, 너비, 높이, 채널수로 구성|

#### Layers
| Name | Description |
|:------|:------|
|`Dense`|모든 입력 뉴런과 출력 뉴런을 연결하는 전결합층|
| `Embedding` | 단어를 의미론적 기하공간에 매핑할 수 있도록 벡터화|
|`Conv1D`|필터를 이용하여 지역적인 특징을 추출|
| `Conv2D` |필터를 이용하여 영상 특징을 추출 |
|`GlobalMaxPooling1D`|여러 개의 벡터 정보 중 가장 큰 벡터를 골라서 반환|
| `MaxPooling1D` |입력벡터에서 특정 구간마다 값을 골라 벡터를 구성한 후 반환 |
|`MaxPooling2D`|영상에서의 사소한 변화가 특징 추출에 크게 영향을 미치지 않도록 함|
| `Flatten` | 2차원의 특징맵을 전결합층으로 전달하기 위해서 1차원 형식으로 변환|
| `LSTM` |Long-Short Term Memory unit의 약자로 순환 신경망 레이어 중 하나|
| `Dropout` |과적합을 방지하기 위해서 학습 시에 지정된 비율만큼 임의의 입력 뉴런(1차원 혹은 2차원)을 제외|

#### Activation Functions
| Name | Description |
|:------|:------|
|`sigmoid`|활성화 함수로 입력되는 값을 0과 1사이의 값으로 출력. 출력값이 특정 임계값(예를 들어 0.5) 이상이면 양성, 이하이면 음성이라고 판별할 수 있기 때문에 이진분류 모델의 출력층에 주로 사용|
| `softmax` |활성화 함수로 입력되는 값을 클래스별로 확률 값이 나오도록 출력. 다중클래스 모델의 출력층에 주로 사용되며, 확률값이 가장 높은 클래스가 모델이 분류한 클래스|
|`tanh`|활성화 함수로 입력되는 값을 -1과 1사이의 값으로 출력. LSTM의 출력 활성화 함수로 사용|
| `relu` |활성화 함수로 주로 은닉층(Conv2D)에 사용 |

