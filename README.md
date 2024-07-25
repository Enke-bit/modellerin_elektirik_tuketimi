# Makine Öğrenme Modellerinin Enerji Tüketimi ve Performans Analizi

Bu proje, çeşitli makine öğrenme modellerinin enerji tüketimini ve performansını analiz etmeyi amaçlamaktadır. Modern bilgisayarlarda makine öğrenme algoritmalarının uygulanması, yüksek hesaplama gücü ve enerji tüketimini beraberinde getirir. Bu çalışma, enerji tüketiminin farklı modeller arasında nasıl değiştiğini ve bu tüketimin model performansına nasıl yansıdığını anlamayı hedeflemektedir.

## İçindekiler

- [Proje Tanımı](#proje-tanımı)
- [Kullanılan Modeller](#kullanılan-modeller)
- [Metodoloji](#metodoloji)
  - [Enerji Tüketimi Hesaplama](#enerji-tüketimi-hesaplama)
  - [Performans Ölçümü](#performans-ölçümü)
- [Sonuçlar](#sonuçlar)
- [Görselleştirmeler](#görselleştirmeler)
- [Kurulum ve Kullanım](#kurulum-ve-kullanım)
- [Yazarlar](#yazarlar)
- [Lisans](#lisans)

## Proje Tanımı

Bu çalışma, çeşitli makine öğrenme modellerinin enerji tüketimini ve performansını değerlendirmek amacıyla gerçekleştirilmiştir. Sürdürülebilirlik perspektifiyle, enerji verimliliğini ve çevresel etkileri minimize etmeyi amaçlayan bir analiz sunulmuştur.

## Kullanılan Modeller

Projede toplam yedi farklı makine öğrenme modeli değerlendirilmiştir:
- **Linear Regression**
- **Random Forest**
- **Gradient Boosting**
- **Support Vector Regressor**
- **K-Nearest Neighbors**
- **Decision Tree**
- **AdaBoost**

## Metodoloji

### Enerji Tüketimi Hesaplama

Enerji tüketimini hesaplamak için `pyJoules` kütüphanesi kullanılmıştır. Bu kütüphane, CPU ve DRAM enerji tüketimini ölçmeyi sağlar. Her modelin eğitim süreci boyunca enerji tüketimi ölçülmüş ve watt-saat (Wh) cinsinden rapor edilmiştir.

### Performans Ölçümü

Modellerin performansı, **Mean Squared Error (MSE)** metriği ile değerlendirilmiştir. MSE, modelin tahmin ettiği değerlerle gerçek değerler arasındaki farkların karelerinin ortalamasını temsil eder. Bu metrik, modelin tahmin doğruluğunu ölçmek için kullanılmıştır.

## Sonuçlar

### Enerji Tüketimi ve Performans

| Model                  | Enerji Tüketimi (Wh) | Mean Squared Error | CPU Kullanımı (%) | Süre (s) |
|------------------------|-----------------------|--------------------|--------------------|----------|
| Linear Regression      | 5.65e-06              | 0.556              | 15.65              | 0.0020   |
| Random Forest          | 0.0163                | 0.255              | 5.35               | 16.88    |
| Gradient Boosting      | 0.0082                | 0.294              | 11.05              | 4.09     |
| Support Vector Regressor | 0.0067              | 1.332              | 4.4                | 8.39     |
| K-Nearest Neighbors    | 3.86e-05              | 1.119              | 6.65               | 0.0321   |
| Decision Tree          | 0.0009                | 0.495              | 21.10              | 0.2341   |
| AdaBoost               | 0.0004                | 0.614              | 4.2                | 0.5092   |

## Görselleştirmeler

Projede çeşitli görselleştirmeler yapılmıştır:

1. **Enerji Tüketimi vs. Model**: Her modelin enerji tüketimini gösteren sütun grafiği.
2. **Süre vs. Model**: Modellerin eğitim sürelerini karşılaştıran sütun grafiği.
3. **Enerji Tüketimi ve MSE ile Scatter Plot**: Enerji tüketimi ve eğitim süresinin Mean Squared Error ile ilişkisinin görselleştirildiği dağılım grafiği.

## Kurulum ve Kullanım

### Gereksinimler

Bu projeyi çalıştırmak için aşağıdaki Python kütüphanelerine ihtiyacınız olacak:
- `numpy`
- `pandas`
- `scikit-learn`
- `pyJoules`
- `matplotlib`
- `seaborn`


###  Kullanım
Projeyi çalıştırmak için aşağıdaki adımları takip edebilirsiniz:

1. Python betiğini çalıştırın.
2. pyJoules kullanarak enerji tüketimi ölçümünü başlatın.
3. Her bir model için eğitim süresini ve enerji tüketimini hesaplayın.
4. Sonuçları görselleştirin.
###  Yazarlar
İbrahim Püsküllü
Lisans
Bu proje MIT Lisansı altında lisanslanmıştır.

### Kurulum

Gereksinimleri yüklemek için aşağıdaki komutu kullanabilirsiniz:

```bash
pip install numpy pandas scikit-learn pyJoules matplotlib seaborn


