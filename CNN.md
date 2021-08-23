# CNN
### CNN은?
* CNN은 Convolutional Neural Networks의 약자로 데이터로부터 자동으로 특징을 학습하는 모델입니다.
* 이미지 인식과 분류에서 탁월한 성능을 냅니다.
### CNN의 구조
![cnn_banner](https://user-images.githubusercontent.com/81547954/130415601-4287d92e-32b6-44f4-947f-4ea0e3485924.png)
## Convolution
### Convolution은 필터로 합성곱 연산을 수행하여 Feature map을 만듭니다.<br>밑의 그림은 2차원 데이터를 1개의 필터로 합성곱 연산을 수행하는 과정입니다
![Convolution_schematic](https://user-images.githubusercontent.com/81547954/130422944-21df84f9-9374-490e-93e7-686d61f958a7.gif)
## Kernel
### Kernel은 필터입니다 이 필터로 이미지의 특징을 뽑아냅니다.<br>필터는 지정간 간격으로 끝까지 이동하면서 전체입력데이터와 합성곱하여 Feature map을 만듭니다.<br><img width="600" alt="conv" src="https://user-images.githubusercontent.com/81547954/130424358-9d9c3640-1b50-4ec7-87d4-179520b7551d.png">
* 필터가 이동하는 간격을 Stride라고 합니다. strid를 1로 설정하면 필터가 1씩 이동하고 strid를 2로 설정하면 필터가 2씩 이동합니다.
### 입력데이터가 여러 채널을 갖을 경우 체널별로 피처 맵을 만듭니다. 그리고 각체널의 피처 맵을 합산하여<br>최종 피처 맵으로 변환합니다.<br><img width="600" alt="conv2" src="https://user-images.githubusercontent.com/81547954/130431295-b1d2184b-1d1f-4786-9af4-dbff7ad6b484.jpg">
## Padding
### 합성곱 연산을 하여 얻은 특성 맵은 입력 맵보다 크기가 작아져 버리는 특성을 가지고 있기 때문에 크기가<br> 줄어듬을 막기 위해 지정된 개수의 폭만큼 테두리를 추가하는것이 패딩(Padding)을 사용합니다.<br>![conv10](https://user-images.githubusercontent.com/81547954/130433943-e8d7b645-0e8a-479e-8a0d-98970486b066.png)
* 값을 0으로 채우는 제로 패딩을 주로 사용합니다.
## Pooling
### Pooling은 convolution한 결과인 출력데이터를 입력으로 받아 크기를 줄이거나 특정 부분을 강조하기위해<br>샘플링하는 과정입니다. 
* feature map에서 특정영역을 형성한뒤 해당 영역에서 가장 큰 수를 도출해내는 것을 max pooling이라고 합니다.
### Convolution과 Padding으로 늘린 데이터를 줄이기 위해서 max pooling을 이용하여 feature들을 뚜렷하게 합니다.<br><img width="400" alt="c123" src="https://user-images.githubusercontent.com/81547954/130438066-1368cadd-6c41-48f8-b16c-0cf9cfd910b0.png">

#### 출처: https://velog.io/@dltjrdud37/CNNConvolutional-Neural-Network<br>https://www.kakaobrain.com/blog/9<br>http://taewan.kim/post/cnn/<br>https://89douner.tistory.com/57
#### gif출처 : http://deeplearning.stanford.edu/wiki/index.php/Feature_extraction_using_convolution
