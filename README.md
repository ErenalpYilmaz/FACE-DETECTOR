# Face Recognition with OpenCV and face\_recognition

Bu proje, Python'da OpenCV ve [face\_recognition](https://github.com/ageitgey/face_recognition) kütüphanesi kullanılarak canlı yüz tanıma sistemi oluşturur. Kamera görüntüsü üzerinden tanıdığınız kişileri tespit eder ve isimleriyle birlikte ekranda gösterir.

## ✨ Özellikler

* Bilinen yüzleri tanıma
* "Unknown" olarak bilinmeyenleri işaretleme
* Gerçek zamanlı (canlı kamera) izleme

## 📚 Gereksinimler

* Python 3.6+
* OpenCV (`cv2`)
* face\_recognition
* dlib (face\_recognition'un bir bağımlılığı)

Kurulum:

```bash
pip install opencv-python
pip install face_recognition
```

> Not: `face_recognition` kurulumu için ek kütüphaneler veya CMake derleyici gerekebilir. [Resmi Yükleme Talimatları](https://github.com/ageitgey/face_recognition#installation)'ı inceleyin.

## 📁 Dosya Yapısı

```
project-folder/
├── face_recognition_script.py
├── Photos/
│   ├── ronaldo.jpg
│   ├── elonMosk.jpg
│   └── erenalp.jpg
```

## 🔧 Nasıl Çalışır?

1. `Photos/` klasöründe tanınmasını istediğiniz kişilerin fotoğraflarını kaydedin.
2. Bu görüntülerden yüz kodlamaları çıkarılır.
3. Kamera açılır ve her karedeki yüzler bilinen yüzlerle karşılaştırılır.
4. Eğer eşleşme varsa, ekranda kişinin ismiyle birlikte yüzü kutulanır.

## 🚀 Çalıştırma

```bash
python main.py
```

Çıkmak için `q` tuşuna basın.

## ⚠️ Uyarılar

* Işık ve kamera kalitesi tanıma doğruluğunda önemlidir.
* Çok benzer görünen yüzlerde (ikizler vb.) hata payı olabilir.
* Yüz kodlamaları ilk bulundukları fotoğraflara göre belirlenir, bu nedenle iyi aydınlatılmış ve net fotoğraflar kullanın.

## 📄 Lisans

Bu proje MIT lisansı altındadır.

---

Hazırlayan: Erenalp Yılmaz
Proje: Canlı Yüz Tanıma Sistemi
