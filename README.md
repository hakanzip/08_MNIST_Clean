# MNIST - Görsel Veri Analizi Projesi

Bu proje, el yazısı ile yazılmış 0-9 arasındaki rakamların yer aldığı MNIST veri seti üzerinde görsel veri analizi yapmak amacıyla hazırlanmıştır - Piksel yoğunluğu, boyut indirgeme ve ortalama görsel üretimi gibi yöntemlerle rakamların yapısal özellikleri incelenmiştir

## Veri Seti

Kaynak: https://www.kaggle.com/datasets/oddrationale/mnist-in-csv?utm_source=chatgpt.com  
Kullanılan dosya: MNIST (gömülü sklearn veri seti olarak veya ayrı .csv/.png formatında)

## Proje Aşamaları

1. Veri Analizi ve Görselleştirme (EDA - Exploratory Data Analysis)  
   Sınıf dağılımı, ortalama görüntüler ve aktif piksel sayısı gibi temel analizler gerçekleştirildi  
   Rakamların yapısal özellikleri görseller üzerinden istatistiksel olarak değerlendirildi  

2. Görsel Temsil ve Ortalama Hesaplamaları  
   Her rakam sınıfı için ortalama görüntüler hesaplandı  
   Ortalama görseller üzerinden sınıflar arası benzerlik ve çizim farklılıkları analiz edildi  

3. Boyut İndirgeme (Dimensionality Reduction)  
   Yüksek boyutlu (784 özellikli) görüntü verileri t-SNE ve UMAP kullanılarak 2B ve 3B uzaya indirildi  
   Sınıfların küme yapıları görselleştirildi, iç içe geçen veya ayrışan bölgeler incelendi  

4. Piksel Yoğunluk ve Karmaşıklık Analizi  
   Her görseldeki aktif (0 olmayan) piksel sayısı hesaplandı  
   Violin plot ile sınıflar arasında çizim karmaşıklığı karşılaştırıldı  

5. Sonuçların Görselleştirilmesi ve Yorumlanması  
   Tüm görselleştirmeler grafikler aracılığıyla sunuldu  
   Veri kümesinin yapısı hakkında sezgisel çıkarımlar yapıldı ve sonuçlar yorumlandı  

## Kullanılan Kütüphaneler

pandas  
numpy  
matplotlib  
seaborn  
scikit-learn

## Proje Yapısı

mnist/  
├── notebook/  
│   └── mnist.ipynb  
├── images/  
│   ├── 22.png  
│   ├── tsne.png  
│   ├── tsne3D.png  
│   ├── umap.png  
│   ├── aktif_piksel_sayısı.png  
│   ├── ortalama_gorsel.png  
│   └── nihai_çıktı.png  
├── README.md  
├── requirements.txt  
└── .gitignore

## Notlar

Bu proje, görsel veri analizi üzerinden modelleme öncesi keşifsel veri analizi sürecini kapsamaktadır - Boyut indirgeme, ortalama görsel üretimi ve piksel yoğunluğu gibi yapılar üzerinden MNIST veri seti incelenmiştir - Görsel temsiller aracılığıyla sınıf yapısı, karmaşıklık ve benzerlikler analiz edilmiştir - Tüm işlemler veri bilimi prensiplerine uygun şekilde sıralı ve yorumlanabilir adımlarla gerçekleştirilmiştir

# 08_MNIST