# Unsupervised_Machine_Learning_Projects
This repository includes unsupervised machine learning projects 
# Denetimsiz Öğrenme ve Kümeleme Analizleri (Unsupervised Learning & Clustering)

Bu depo, farklı veri setleri üzerinde **Denetimsiz Öğrenme (Unsupervised Learning)** algoritmalarının uygulanmasını, performans karşılaştırmalarını ve detaylı veri analizi süreçlerini içerir.

Proje kapsamında **K-Means**, **K-Medoids** ve **Hiyerarşik Kümeleme** algoritmaları kullanılarak veri setleri analiz edilmiş ve sonuçlar çeşitli validasyon metrikleri ile doğrulanmıştır.

##  Proje İçeriği ve Algoritmalar

Bu çalışma aşağıdaki temel kümeleme algoritmalarını ve tekniklerini kapsar:

### 1. Kullanılan Algoritmalar
* **K-Means Clustering:** Veri setini K adet kümeye ayıran merkez tabanlı kümeleme.
* **K-Medoids (PAM):** Gürültülü verilere (outliers) karşı daha dirençli olan, merkez olarak gerçek veri noktalarını kullanan yaklaşım.
* **Hiyerarşik Kümeleme (Hierarchical Clustering):** Veriler arasındaki hiyerarşik ilişkiyi dendrogram üzerinden analiz eden yaklaşım (Agglomerative).

### 2. Küme Doğrulama (Cluster Validation)
Model başarısını ölçmek için aşağıdaki metrikler kullanılmıştır:
* **Elbow Metodu (Dirsek Yöntemi):** Optimal K sayısının belirlenmesi.
* **Silhouette Skoru:** Kümelerin ne kadar iyi ayrıştığının ve kendi içinde ne kadar tutarlı olduğunun analizi.
* **Dendrogram Analizi:** Hiyerarşik yapıdaki ideal kesim noktasının tespiti.

### 3. Uzaklık Ölçüleri (Distance Metrics)
Algoritmaların performansını etkileyen farklı uzaklık ölçüleri test edilmiştir:
* **Euclidean Distance (Öklid):** Kuş uçuşu mesafe.
* **Manhattan Distance:** Izgara (grid) tabanlı mesafe (özellikle K-Medoids ile).
* **Cosine Similarity:** Vektörler arası açısal benzerlik.

## 🛠 Veri Ön İşleme (Data Preprocessing)
Modellerin başarısını artırmak için ham veri üzerinde aşağıdaki işlemler uygulanmıştır:
* **Eksik Veri Analizi:** (Missing Value Imputation)
* **Ölçeklendirme (Scaling):** Verilerin birbirine baskın gelmemesi için `StandardScaler` ve `MinMaxScaler` kullanımı.
* **Gürültü Temizleme (Outlier Detection):** Aykırı değerlerin tespiti ve yönetimi.

