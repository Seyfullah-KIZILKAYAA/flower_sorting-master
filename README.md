# Flower Sorting (Çiçek Sınıflandırma) Projesi

Bu proje, yapay zeka ve makine öğrenmesi teknikleri kullanarak çiçek türlerini sınıflandıran kapsamlı bir uygulamadır. Iris veri seti üzerinde eğitilmiş model, çiçek özelliklerine göre türleri doğru bir şekilde tanımlayabilmektedir.

## Proje Hakkında

Bu proje, çiçek görüntülerini analiz ederek çiçek türlerini otomatik olarak tanımlayan bir makine öğrenmesi uygulamasıdır. Iris veri seti kullanılarak, çiçeklerin fiziksel özellikleri (çanak yaprak ve taç yaprak ölçüleri) değerlendirilerek sınıflandırma yapılmaktadır. Scikit-learn kütüphanesi ile geliştirilen model, yüksek doğruluk oranıyla çiçek türlerini belirleme yeteneğine sahiptir.

## Veri Seti

Projede kullanılan Iris veri seti, makine öğrenmesi alanında yaygın olarak kullanılan klasik bir veri setidir. Bu veri seti:

- 150 örnek içerir
- 3 farklı Iris çiçek türü bulunur (Setosa, Versicolor, Virginica)
- Her çiçek için 4 özellik kaydedilmiştir:
  - Çanak yaprak uzunluğu (sepal length)
  - Çanak yaprak genişliği (sepal width)
  - Taç yaprak uzunluğu (petal length)
  - Taç yaprak genişliği (petal width)

## Özellikler

- Çiçek özelliklerini (çanak yaprak uzunluğu, çanak yaprak genişliği, taç yaprak uzunluğu, taç yaprak genişliği) kullanarak hassas sınıflandırma
- Scikit-learn makine öğrenmesi kütüphanesi ile entegrasyon
- Çoklu sınıflandırma algoritmaları (KNN, Karar Ağaçları, SVM, vb.)
- Iris veri seti üzerinde eğitim ve test işlemleri
- Çapraz doğrulama ile model performans değerlendirmesi
- Kullanıcı dostu arayüz
- Görselleştirme araçları ile sonuçların sunumu

![Model Performans Grafiği](https://github.com/seyfullah-kizilkaya/flower_sorting/assets/110238774/e0871832-4872-48bd-b165-3fc8929caeb8)

*Genel olarak, modelin eğitim sürecinde iyi bir performans gösterdiği ve hem eğitim hem de doğrulama doğruluklarının arttığı gözlemlenmiştir. Ancak, doğrulama kaybındaki dalgalanmalar, modelin doğrulama verisine fazla uyum sağlayabileceğini ve bu nedenle dikkatli bir şekilde gözlemlenmesi gerektiğini göstermektedir. Modelin genelleme kabiliyetini arttırmak için ek düzenleme teknikleri (örneğin, erken durdurma, düzenleme) kullanılabilir.*

## Kurulum

1. Bu projeyi klonlayın:
   ```
   git clone https://github.com/Seyfullah-KIZILKAYAA/flower_sorting-master.git
   ```

2. Proje dizinine gidin:
   ```
   cd flower_sorting-master
   ```

3. Gerekli kütüphaneleri yükleyin:
   ```
   pip install scikit-learn numpy pandas matplotlib seaborn
   ```

## Kullanım

1. Ana uygulamayı başlatmak için:
   ```
   python sınıflama.py
   ```

2. Program çalıştığında, çiçek özelliklerini aşağıdaki formatta girerek sınıflandırma yapabilirsiniz:
   - Çanak yaprak uzunluğu (cm)
   - Çanak yaprak genişliği (cm)
   - Taç yaprak uzunluğu (cm)
   - Taç yaprak genişliği (cm)

3. Girilen özelliklere göre, program çiçeğin hangi türe ait olduğunu tahmin edecektir.

## Teknik Detaylar

### Kullanılan Algoritmalar

Proje içerisinde aşağıdaki makine öğrenmesi algoritmaları kullanılmıştır:

- K-En Yakın Komşu (KNN)
- Destek Vektör Makineleri (SVM)
- Karar Ağaçları
- Rastgele Orman

### Model Eğitimi ve Değerlendirme

Model, veri setinin %70'i üzerinde eğitilmiş ve kalan %30'u ile test edilmiştir. Çapraz doğrulama ile model performansı optimize edilmiş ve en iyi hiperparametreler seçilmiştir.

### Performans Metrikleri

- Doğruluk (Accuracy): %95+
- Hassasiyet (Precision)
- Duyarlılık (Recall)
- F1 Skoru

## Teknolojiler

- Python 3.x
- Scikit-learn: Makine öğrenmesi algoritmaları için
- NumPy: Sayısal hesaplamalar için
- Pandas: Veri manipülasyonu için
- Matplotlib ve Seaborn: Veri görselleştirmesi için

## Dosya Yapısı

- `sınıflama.py`: Ana uygulama dosyası, model eğitimi ve tahmin işlemlerini içerir
- `flower.jpg`: Örnek Iris çiçek görüntüsü
- `README.md`: Proje dokümantasyonu
- Veri klasörü: Iris veri seti ve ilgili dosyalar

## Gelecek Geliştirmeler

- Web tabanlı kullanıcı arayüzü
- Gerçek zamanlı görüntü işleme ile çiçek tanıma
- Daha fazla çiçek türünü içeren genişletilmiş veri seti desteği
- Model performansını artırmak için derin öğrenme yaklaşımları

## Katkıda Bulunma

1. Bu depoyu fork edin
2. Feature branch'i oluşturun (`git checkout -b feature/amazing-feature`)
3. Değişikliklerinizi commit edin (`git commit -m 'feat: Add some amazing feature'`)
4. Branch'inize push edin (`git push origin feature/amazing-feature`)
5. Pull Request oluşturun

## Lisans

Bu proje MIT lisansı altında lisanslanmıştır. Detaylar için `LICENSE` dosyasına bakın.

## İletişim

Seyfullah KIZILKAYA - [GitHub](https://github.com/Seyfullah-KIZILKAYAA)

Proje Linki: [https://github.com/Seyfullah-KIZILKAYAA/flower_sorting-master](https://github.com/Seyfullah-KIZILKAYAA/flower_sorting-master)

## Teşekkürler

- Scikit-learn ekibine kapsamlı makine öğrenmesi kütüphanesi için
- Iris veri setini oluşturan ve paylaşan araştırmacılara
- Tüm katkıda bulunanlara ve geri bildirim sağlayanlara
