# Uyku Evrelerinin EEG Verileri ile Derin Öğrenme Yöntemleri Kullanılarak Sınıflandırılması

Bu repo, tek kanallı EEG sinyalleri kullanılarak uyku evrelerinin otomatik sınıflandırılmasını amaçlayan bir derin öğrenme projesine ait kaynak kodları ve dokümantasyonu içermektedir. Çalışma, bir doktora dersi kapsamında hazırlanmış olup, PhysioNet Sleep-EDF veri seti üzerinde iki farklı derin öğrenme mimarisinin karşılaştırmalı analizini içermektedir.

## 📌 Proje Amacı

Bu projenin temel amacı, uyku evresi sınıflandırma probleminde farklı derin öğrenme mimarilerinin performanslarını karşılaştırmak ve mimari seçimlerinin sınıflandırma başarımı üzerindeki etkilerini incelemektir. Bu kapsamda aşağıdaki iki model ele alınmıştır:

- CNN + BiLSTM (hibrit mimari)
- BiGRU (saf tekrarlayan sinir ağı mimarisi)

## 📊 Kullanılan Veri Seti

- **Veri Seti:** Sleep-EDF Expanded
- **Kaynak:** PhysioNet
- **Sinyal Türü:** EEG
- **Kanal:** Fpz–Cz
- **Epoch Uzunluğu:** 30 saniye
- **Sınıflar:**  
  - Uyanıklık (W)  
  - Uyku Evresi 1 (N1)  
  - Uyku Evresi 2 (N2)  
  - Uyku Evresi 3 (N3)  
  - Uyku Evresi 4 (N4)  
  - REM  

Veri seti büyük boyutlu olduğu için bu repo içerisinde paylaşılmamaktadır. Veri, PhysioNet üzerinden otomatik olarak indirilmektedir.

## ⚙️ Kurulum

Projeyi çalıştırmadan önce gerekli Python paketlerinin kurulması gerekmektedir.

```bash
pip install -r requirements.txt
