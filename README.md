# EESEC 440 English for EEE on DL
## I. Artificial Neural Networks

Artificial neural networks (ANN) are extremely powerful structures that are capable of relating input-output data with utmost complexity. The increment in computational power provided by the new generation Graphical Processing Units (GPU) in the last decade enabled ANN to solve many engineering problems in various fields of study (e.g., Computer Vision, speech recognition, Natural Language Processing, power transfer [1], etc). There are different flavors of ANN designed for different applications depending on the needs. Multi-layer Perceptron (MLP) is one of the most preferred type of network commonly employed in regression and classification problems, which are two major functions of a ANN.

**A. Multi-layer Perceptron (MLP)**

We will study MLP elaborately throughout the course. Regression and classification examples, both supervised learning. Please see Fig. 1 for an example MLP network structure.

![122469761-fb816400-cfc5-11eb-876d-3af765f73169](https://user-images.githubusercontent.com/83131484/122642597-f6322f80-d113-11eb-9ba4-e6076fbc2a5b.png)
Fig. 1: A multi input single output MLP.

**Exclusive OR (XOR) Problem**

![122469163-4babf680-cfc5-11eb-86a0-534f9aef5e9b](https://user-images.githubusercontent.com/83131484/122642628-0ba75980-d114-11eb-8171-53b6f0373216.jpg)
Fig. 2: A MLP network is going to learn XOR problem.
![122468881-f374f480-cfc4-11eb-923a-8d33ee8667cf](https://user-images.githubusercontent.com/83131484/122642676-50cb8b80-d114-11eb-9666-c9e04681e339.jpg)
Fig. 3: For the XOR problem, we use a MLP with one hidden layer consisting of sixteen neurons.

![122468930-038cd400-cfc5-11eb-9a71-c9c050e5ad3d](https://user-images.githubusercontent.com/83131484/122642685-604ad480-d114-11eb-8fef-a1a0bf8da0db.jpg)
Fig. 4: Error back-propogation algorithm (e.g., Gradient Descent) is used to update the network parameters.

**Çok Katmanlı bir Yapay Sinir Ağının Ayarlabilen Parametre (Ağırlık) Sayısı**

![122468881-f374f480-cfc4-11eb-923a-8d33ee8667cf](https://user-images.githubusercontent.com/83131484/122642700-735da480-d114-11eb-906b-f34ba32e0df0.jpg)
Fig. 5: A MLP network with one input, three neurons in the hidden layer and single output. This network has 2 : 3 : 1 configuration. Yukarıda Fig. 5'de gösterilen yapay sinir ağının konfigurasyonu 2 : 3 : 1 olup, giriş katmanında iki, gizli katmanında üç ve çıkış katmanında bir nöron bulundurmaktadır (yuvarlaklar nöronları temsil ediyor). Şekilde ayarlanabilen parametre sayısı 13 olarak gözüküyor: w1, w2, w3, w4, w5, w6, w7, w8, w9, w10, w11, w12, w13. Verilen konfigürasyona göre ayarlanabilen parametre (ağırlık) sayısını hem elimizle çizerek, hem de formülize ederek kısa yoldan hesaplayabiliriz. Formülü siz de biraz düşünürseniz kendiniz çıkarabilirsiniz. Giriş, çıkış ve bir gizli katmandan oluşan bir yapay sinir ağındaki toplam ayarlanabilen parametre (ağırlık - weight) sayısını bulan formül şöyle:

n = (n1 x n2 + n2) + (n2 x n3 + n3)

Burada n1 giriş katmanındaki nöron sayısı, n2 gizli katmandaki nöron sayısı ve n3 çıkış katmanındaki nöron sayısı olurken n ise toplam ayarlanabilen parametre yani ağırlık (weight - w) sayısı. Yukardaki formülde uygun terimler ortak parantez alınırsa, formül aşağıdaki halini alır:

n = n2(n1 + 1) + n3(n2 + 1)

Fig. 5'de verilen 2 : 3 : 1 konfigürasyonlu ağı formülde test edecek olursak n = 3(2 + 1) + 1(3 + 1) = 3 x 3 + 1 x 4 = 13 değerini onaylamış oluruz.
![122469282-71d19680-cfc5-11eb-87c1-1a834005ce0d](https://user-images.githubusercontent.com/83131484/122642716-7f496680-d114-11eb-8e05-5627efd82b25.jpg)

**2 Boyutlu Sınıflandırma Problemi**
![122469353-86159380-cfc5-11eb-9ec1-92afdc84ff88](https://user-images.githubusercontent.com/83131484/122642729-8e301900-d114-11eb-9fbe-5b751bc50fa3.jpg)
Fig. 6: 2 boyutlu sınıflandırma probleminde en başta karşılaşılan bazı adımlar.

**En Küçük Kareler (Least Squares)**
![122469391-93328280-cfc5-11eb-8e56-4cb25022fbc8](https://user-images.githubusercontent.com/83131484/122642742-a011bc00-d114-11eb-89d8-9f67f8535b4b.png)
Fig. 7: Bir boyutlu optimizasyon (veya regresyon) probleminin görselleştirilmiş hali.
**B. Convolutional Neural Network (CNN)**
We might study classification example on images in the last weeks of the course. Cats-dogs image repository on Kaggle. We will follow the tutorial given in [2]. Please see Figures 8 and 9 for classification of cat and dog images via CNN.
<img width="1153" alt="122469484-afceba80-cfc5-11eb-9a4a-70c842359fcc" src="https://user-images.githubusercontent.com/83131484/122642771-ba4b9a00-d114-11eb-8f13-958f093b19f0.png">
Fig. 8: Classification of cat & dog images via CNN.
![122469518-b826f580-cfc5-11eb-9f65-dd3137e880c8](https://user-images.githubusercontent.com/83131484/122642777-c20b3e80-d114-11eb-8142-6c5ef30a9682.gif)
Fig. 9: Cats and dogs classification with deep learning.
