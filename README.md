![image](https://github.com/user-attachments/assets/6451ce57-06dd-41ea-8b37-03f9c17c1af0)


Koku Sınıflandırma ve Doğal Dil İşleme (NLP) Projesi
-------------------------------------------------------------
Proje Hakkında
--
Bu proje, bir koku sensöründen elde edilen verilerin sınıflandırılması ve ardından Doğal Dil İşleme (NLP) teknikleri kullanılarak anlamlı hale getirilmesi üzerine odaklanmaktadır. Amaç, farklı kokuları doğru bir şekilde tanımlayabilen ve sınıflandırabilen bir model oluşturmak ve bu sınıflamaları anlamlı metinlere dönüştürmektir.

![image](https://github.com/user-attachments/assets/e777b2e6-ee28-427b-a298-6c6c62d1e947)

Veri Seti
--
![image](https://github.com/user-attachments/assets/94c33ccc-4fc9-448f-a53f-68313e7f36cb)


Bu projede kullanılan veri seti, bir koku sensöründen toplanan verileri içermektedir. Veri seti, sensörün okuduğu farklı özelliklere karşılık gelen birçok özellik ve farklı koku kategorilerini (örneğin, hava, kahve, kolonya) temsil eden etiketler içermektedir.

Örnek Sayısı: 5,490

Özellik Sayısı: 66

Sınıflar: 3 (Hava, Kahve, Kolonya)


Kullanılan Teknolojiler
--
Python: Genel programlama ve veri işleme için

Pandas: Veri yükleme ve ön işleme için

NumPy: Sayısal işlemler için

Scikit-Learn: Model eğitimi, değerlendirme ve ön işleme için

Matplotlib ve Seaborn: Veri görselleştirme için

Joblib: Model saklama için

Modelleme Süreci
--
Veri Ön İşleme
--

1-Eksik ve Sonsuz Değerlerin İşlenmesi: 
Sonsuz değerler NaN olarak değiştirildi.
NaN değerler veri setindeki maksimum değerle dolduruldu.


2-Veri Ölçekleme:
Modelleri eğitmeden önce veriler StandardScaler ile ölçeklendirildi.

Model Eğitimi
--

Aşağıdaki sınıflandırma modelleri eğitildi ve değerlendirildi:

-Logistic Regression

-K-Nearest Neighbors (K-NN)

-Support Vector Classifier (SVC)

-Random Forest Classifier

-Decision Tree Classifier

-Gradient Boosting Classifier

-AdaBoost Classifier

-MLP Classifier (Multi-Layer Perceptron)

Model Değerlendirmesi
--
Her model şu metrikler kullanılarak değerlendirildi:

-Doğruluk (Accuracy)

-Precision

-Recall

-F1-Score

En iyi performans gösteren model, %100 doğruluk oranıyla K-Nearest Neighbors modeli oldu.

Sonuçlar
--

En İyi Model: K-Nearest Neighbors

Doğruluk (Accuracy): 100%

Precision, Recall, F1-Score: Tüm metriklerde her sınıf için 1.00 skor elde edildi.

Bu sonuçlar, K-NN modelinin sensör verilerini sınıflandırmada son derece etkili olduğunu göstermektedir. Ancak, sonuçların genelleştirilebilirliğini sağlamak için farklı veri setleri üzerinde de doğrulama yapılması önerilir.

Nasıl Kullanılır?
--
Gereksinimler
--


-Python 3.7+

-Gerekli kütüphaneler (bkz. requirements.txt)

Kurulum
--
1-Depoyu klonlayın: `git clone https://github.com/mehmetozmenn/Astrosit.git`

2-Proje dizinine gidin: `cd Astrosit`

3-Gerekli kütüphaneleri yükleyin: `pip install -r requirements.txt`

Modeli Çalıştırma
--

1-Verilerinizi beklenen formata hazırlayın.

2-Model eğitim scriptini çalıştırın: `python train_model.py`

3-Eğitilen modeli kullanarak tahmin yapın: `from predict import predict` `result = predict(input_data)` `print(result)`

Gelecek Çalışmalar
--
**-Veri setini genişletmek:** Daha fazla koku ve örnek ekleyerek genelleştirilebilirliği artırmak.

**-Derin öğrenme modellerini denemek:** CNN veya LSTM gibi daha karmaşık veriler için potansiyel olarak daha iyi performans gösterebilecek modelleri denemek.

**-NLP tekniklerini geliştirmek:** Kokuların daha anlamlı ve bağlam farkındalığı yüksek açıklamalarını üretmek.

Katkıda Bulunma
--

Katkılarınızı bekliyoruz! Herhangi bir öneriniz veya iyileştirme fikriniz varsa, lütfen bir Pull Request gönderin veya bir Issue açın.

Lisans
--

Bu proje MIT Lisansı ile lisanslanmıştır. Daha fazla bilgi için LICENSE dosyasına bakın.

