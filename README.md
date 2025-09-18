# Gerçek Zamanlı Curl Sayacı

Bu proje, MediaPipe Pose kütüphanesini kullanarak web kameranızdan gelen görüntü akışı üzerinde gerçek zamanlı bir curl (pazu bükme) sayacı çalıştırır. Uygulama, dirsek açısını anlık olarak hesaplayarak fitness takibini ve doğru egzersiz formunu destekler.

## ✨ Öne Çıkan Özellikler

- **Dinamik HUD (Heads-Up Display):** Tekrar (REPS) sayısı ve hareketin aşaması (STAGE) bilgilerini, metin uzunluğuna göre otomatik ayarlanabilen, dinamik bir kutu içinde gösterir.
- **Akıllı Sayaç Mekanizması:** Ayarlanabilir açı eşikleri sayesinde (ör. `ANGLE_UP_THR` ve `ANGLE_DOWN_THR`), tekrar sayımını hassas ve güvenilir bir şekilde gerçekleştirir.
- **Kolay Kullanım:** Sol (`"left"`) veya sağ (`"right"`) kol için kolayca yapılandırılabilir.
- **Çözünürlükten Bağımsızlık:** Uygulama, kullanılan kameranın çözünürlüğünden bağımsız olarak tüm görsel bileşenleri (metinler, sayılar) doğru şekilde konumlandırır.
- **Selfie Modu:** Yalnızca tek bir yatay çevirme (`flip`) işlemi ile kullanıcıya ayna efekti sunar ve sol/sağ kol eşlemesini doğru yapar.
- **Görsel Kimlik:** Opsiyonel logo desteği ve özelleştirilebilir imza satırı (ör. `github.com/yarencelikk`) ile projenize kişisel bir dokunuş katabilirsiniz.


---
🙏 Teşekkür ve Kaynak

Bu çalışma, bir YouTube MediaPipe Pose anlatımını referans alarak yazılmıştır.

İlham kaynağı: [[YouTube tutorial linkinizi buraya ekleyin](https://www.youtube.com/watch?v=06TE_U21FK4)]

---
## 🚀 Kurulum

```bash
# (opsiyonel) sanal ortam
python -m venv .venv && .venv\Scripts\activate   # Windows
# source .venv/bin/activate                      # macOS/Linux

pip install opencv-python mediapipe numpy
# Jupyter kullanacaksanız
pip install notebook

