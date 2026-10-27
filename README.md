# Custom GPT Trainer

*Train a small GPT on your own text in Google Colab, using nanoGPT.*

Andrej Karpathy'nin [nanoGPT](https://github.com/karpathy/nanoGPT) kodunu kullanarak kendi metin veri setlerinizle özel bir GPT modeli eğitmenizi sağlar.

## 🚀 Özellikler
- **Hızlı Kurulum:** Google Colab üzerinde tek tıklamayla eğitim ortamı hazırlama.
- **Özel Veri Seti:** Kendi `veri-seti.txt` dosyanızla karakter veya Tiktoken tabanlı eğitim.
- **GPU Optimizasyonu:** T4 GPU desteği ile verimli eğitim süreçleri.
- **Üretim (Sampling):** Eğitilen modelden anlık metin çıktıları oluşturma.

## 🛠️ Kurulum ve Kullanım

1.  **Depoyu Klonlayın:**
    ```bash
    git clone https://github.com/YouthX-Research/custom-gpt-trainer.git
    cd custom-gpt-trainer
    ```

2.  **Veri Setini Hazırlayın:**
    Eğitmek istediğiniz metin verilerini `veri-seti.txt` adıyla ana dizine yerleştirin.

3.  **Notebook'u Çalıştırın:**
    `custom_gpt_trainer_.ipynb` dosyasını Google Colab'da açın. Notebook şunları otomatik olarak yapar:
    - Gerekli bağımlılıkları (`torch`, `tqdm`, `numpy`, `tiktoken`) kurar.
    - `nanoGPT` çekirdek kodlarını çeker.
    - Veriyi işlemden geçirerek `.bin` formatına dönüştürür.
    - Belirlediğiniz hiper-parametrelerle eğitimi başlatır.

4.  **Metin Üretme:**
    Eğitim bittiğinde, notebook içindeki örnekleme hücresini çalıştırarak modelinizden metin üretebilirsiniz.

## ⚙️ Hiper-Parametreler
Eğitim sürecini notebook içindeki `cfg` bloğundan özelleştirebilirsiniz:
- `n_layer`: 4-8 (Katman sayısı)
- `n_head`: 4-8 (Dikkat kafası sayısı)
- `n_embd`: 256-512 (Embedding boyutu)
- `max_iters`: Eğitim adım sayısı

## 👥 İletişim ve Katkı
- **Geliştirici:** VastSea0
- **E-posta:** [vastseaoffical0@outlook.com](mailto:vastseaoffical0@outlook.com)
- **GitHub:** [@VastSea0](https://github.com/VastSea0)

## Lisans

Bu repodaki notebook [GPL-3.0](LICENSE) ile lisanslıdır. Notebook'un indirdiği nanoGPT kodu kendi MIT lisansına tabidir.

[YouthX Research](https://github.com/YouthX-Research) projesidir.
