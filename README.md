# WasteClassifier

**WasteClassifier**, evsel ve geri dönüştürülebilir atıkları görüntü işleme yoluyla ayırt eden bir sınıflandırma modelidir. Bu proje, çevre bilincini artırmak ve atık yönetimini otomatikleştirmek amacıyla geliştirilmiştir.

Günümüzde artan tüketim alışkanlıklarıyla birlikte atık miktarı da ciddi oranda artmıştır. Atıkların doğru şekilde ayrıştırılması, geri dönüşümün verimli çalışabilmesi açısından kritik öneme sahiptir. Biz de bu probleme yönelik bir çözüm geliştirdik: Görüntülerden atık türünü sınıflandırabilen bir yapay zeka modeli.

---

## 🎯 Projenin Amacı

- Atıkların **otomatik olarak sınıflandırılması** ile geri dönüşüm sistemlerine destek sağlamak  
- **Gerçek dünya koşullarına uygun** örneklerle eğitilmiş bir model geliştirmek  
- Veri artırma ve transfer öğrenme tekniklerini kullanarak **yüksek doğruluk oranına** ulaşmak  

---

## 📁 Veri Kümesi

Veri kümesi `images/` klasöründe yer almaktadır.


---

## 🧠 Yöntem

- **Model:** MobileNetV3 Small (transfer learning ile)
- **Veri Artırma:** Renk bozulması, döndürme, ölçekleme, bulanıklık
- **Dönüşümler:** Normalize, Resize (256x256)
- **Performans Ölçütleri:** Accuracy, Confusion Matrix, Classification Report

Eğitim verisi %60, doğrulama %20, test %20 oranında bölünmüştür. Eğitim sürecinde hem eğitim hem de doğrulama verileri üzerinde kayıplar ve doğruluklar izlenmiştir.


---

## 🔧 Gereksinimler

```bash
pip install torch torchvision matplotlib scikit-learn pillow
```

---

## 🚀 Kullanım

```bash
git clone https://github.com/kullaniciadi/WasteClassifier.git
cd WasteClassifier

jupyter notebook "recyclable and household waste classification.ipynb"
```

Notebook içindeki adımları takip ederek veriyi yükleyebilir, modeli eğitebilir ve test edebilirsiniz.


---

