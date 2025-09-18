# Real-Time Curl Counter (MediaPipe Pose)

Web kameranızdan gelen akışla **dirsek açısını** hesaplar, **REPS** (tekrar) ve **STAGE** (up/down) bilgisini gerçek zamanlı gösterir.  
Bu repo, YouTube’daki temel MediaPipe Pose anlatımından esinlenerek **baştan yazılmış** ve şu eklemelerle genişletilmiştir:

- ✅ **Tek flip** ile selfie görünüm ve doğru LEFT/RIGHT eşlemesi  
- ✅ Çözünürlükten bağımsız **dinamik HUD** (REPS/STAGE kutusu 10, 100… olduğunda taşmaz)  
- ✅ Sol/sağ kol seçimi (`SIDE = "left" | "right"`)  
- ✅ Ayarlanabilir eşikler (`ANGLE_UP_THR`, `ANGLE_DOWN_THR`)  
- ✅ İmza satırı (örn. `github.com/yarencelikk`) ve opsiyonel **logo** desteği

---
🙏 Teşekkür ve Kaynak

Bu çalışma, bir YouTube MediaPipe Pose anlatımını referans alarak baştan yazılmış ve aşağıdaki iyileştirmelerle genişletilmiştir:

Dinamik HUD (REPS/STAGE)

Flip güvenli metin yerleşimi (çözünürlük bağımsız)

Sol/sağ kol seçimi ve ayarlanabilir eşikler

Kaynak bağlantısı (varsa) ekleyin:
Inspired by: [[YouTube tutorial linkinizi buraya ekleyin](https://www.youtube.com/watch?v=06TE_U21FK4)]

---
## 🚀 Kurulum

```bash
# (opsiyonel) sanal ortam
python -m venv .venv && .venv\Scripts\activate   # Windows
# source .venv/bin/activate                      # macOS/Linux

pip install opencv-python mediapipe numpy
# Jupyter kullanacaksanız
pip install notebook

