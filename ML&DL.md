[[Linear Algebra]]
[[Analytic Geometry]]

# Classic ML:
#### Алгоритмы кластеризации:
1) [[K-means]]
#### Деревья и как их прунить: 
[[Decision tree]]
#### Бустинги:
1) [[AdaBoost]]
2) [[GBM]]
3) [[Catboost algorithm]]
#### Метрики:
1) [[Recall and Precision]]
2) [[F1]]
3) [[RocAuc]]
4) [[R squared metric]]
# DL
[[Строение нейрона]]
### Активации:
1) линейные (чекай [[Перцептроны]])
2) [[Сигмоидальные]]
3) [[С гиперболическим тангенсом]]
4) [[ReLu]]
5) и его друг [[Softplus]]
6) [[GELU]]
7) [[Softmax]]
### CV:
[[CNN]]
[[Pooling]]
#### Эволюция сверточных сетей
1) [[LeNet]] (самая первая и примитивная)\
2) [[AlexNet]] (чуть сложнее)
3) [[VGG]] Network ( состоит из блоков, каждый из которых состоит из нескольких слоев сверток и макспулинга)
4) [[NiN]]
5) [[GoogLeNet]]
6) [[ResNet]]
7) [[ResNeXt]]
8) [[DenseNet]]
9) [[EfficientNet]]
Эволюция сетей для object detection:
	1) [[R-CNN]]
	2) [[FAST R-CNN]]
	3) [[FASTER R-CNN]]
	4) [[YOLO]]
#### Модели для face recognition:
1) [[FaceNet]]
2) 


### NLP:
#### общее
1) [[Токен]]
2) [[disfluences]]
3) [[word types & word instances]]
4) [[text normalization]]

#### Виды токенизаций:
1) [[Byte-Pair Encoding]]
2) [[Unigram Language Modeling]]
[[Word Normalixation]]
[[Lemmatization]]
[[Stemming]]
[[Sentence Segmentation]]
[[Minimum Edit Distance]]

#### Vector Semantics and Embeddings:
1) [[bag-of-words]]
2) [[tf-idf]]
3) [[word2vec]]
4) [[cosine]]
5) [[PPMI]]
6) [[Positional embedding]]

#### Language Models:
1) [[N-gram model]]:
		1.1)  [[Markov Chain]]
2) [[MLP for NLP]]
3) [[RNN]]
	1) [[LSTM]]
4) [[Transformers]]

Оценка эффективности языковых моделей:
1) [[Extrinsic evaluation]]
2) [[Intrinsic evaluation]]
### Audio Signal Processing

Звук нуждается в предварительной обработке, перед тем, как мы его будем использовать.

[[Sound waves]] - что такое волна
[[DAC&ADC]]  - Преобразование аналога в дискретку
[[Time and frequency-domain audio features]] - фичи, которые можно получить
[[Fourier Transform]] - Босс этой качалки
### Остальное:
#### Состав метрики:
1) [[Функция потерь]]
2) [[Эмпирический риск]]

#### Методы оптимизации:
1) sgd
2) [[sgd with momentum]]
3) [[sgd with nesterov momentum]]
4) [[adagrad]]
5) [[rmsprop]]
6) [[adam]]
7) [[adadelta]]


#### Термины и обозначения дип лернинга: 
1) [[Лютейшая база]] 
2) [[Батч]]
3) [[Эпоха]]

#### Backpropagation:
1) [[Лютейшая база]]
2) [[Два предположения, нужных для функции эмпирического риска]]
3) [[Hadamard product]]
4) [[Четыре базовых уравнения для backpropagation]]


#### Метрики (и им подобные):
1) [[OLS]]
2) [[MLE]]
3) [[Cross Entropy Loss]]
4) [[mAP]]
5) 

#### Энкодинги:
1) [[OneHotEncoding]]
2) [[LabelEncoding]]
3) [[TargetEncoding]]
4) [[CatboostEncoding]]

#### Регуляризация 
1) [[L1&L2]]
2) [[Dropout]]

#### Honorable mentions:
1) [[Bottle Neck]]
2) [[Transfer Learning]]
3) [[Batch Normalization]]
4) [[Normalization and Standardization]]
5) 