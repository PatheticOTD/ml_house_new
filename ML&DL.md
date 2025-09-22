[[Linear Algebra]]
[[Analytic Geometry]]
[[Probability theory and statistics]]
[[Continuous Optimisation]]
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

Методы генерации текста:
1. [[Greedy Search]]
2. [[Beam Search]]
3. [[Top-k sampling]]
4. [[Top-p Sampling]]
5. [[Temperature]]

[[Retrieval-Augmented Generation]]

Аспекты файнюнинга моделей:
1. [[Chat Templates]]
2. [[Supervised Fine-Tuning]]
3. 
### RL

**Политика** (_policy_) — это стратегия поведения агента. Она определяет, какие действия агент будет предпринимать в каждом состоянии. Это центральная часть любой системы обучения с подкреплением.

![[action_space.jpg]]
![[obs_space_recap.jpg]]
![[tasks.png]]
![[pbm_1.jpg]]
![[pbm_2.jpg]]
![[vbm_1.jpg]]
![[vbm_2.jpg]]
![[Pasted image 20250623174821.png]]
##### The two types of value-based methods
Напомню, что это те методы которые оптимизируют саму функцию.
![[Pasted image 20250620182033.png]]
![[Pasted image 20250620181118.png]]
Обе эти функции находятся на картинке выше. в правом нижнем углу.
Первая, это State-Value function. Она просчитывает ожидаемые значения для каждого состояния.
Вторая же, Action-value function, на каждом состоянии она подсчитывает значения, и затем выбирает действие
[[Bellman Equation]] помогает нам оптимизировать процесс нахождения.
Для state value метода уравнения беллмана применяются каждый итеративно до тех пор, пока значения состояний перестанут отличаться на эпсилон. стоит отметить, что терминальные состояния всегда будут иметь нулевой вес.
![[Pasted image 20250623225828.png]]

![[Pasted image 20250625163108.png]]
 
##### Monte Carlo vs Temporal Difference Learning
Это два подхода к обучению моделей. 
[[Monte Carlo learning]] использует весь эпизод для обучения.
[[Temporal Difference]] использует только шаг ($S_{t},A_{t},R_{t+1}, S_{t+1}$) для обучения.
Иногда Очень полезно понять, насколько мы выигрываем или проигрываем, если выберем то или иное действие [[Advantage Function]]
##### Методы осп
1. [[Trust Region Policy Optimizaiton]]
2. [[Proximal Policy Optimization]]
3. 
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
5) [[Autoencoders]]
6) 