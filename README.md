````markdown
# 🎥 Review Phim 🎥

🎬 Ứng dụng web “Review Phim” mạnh mẽ và thân thiện, cho phép bạn dễ dàng dịch và đánh giá phim với giao diện trực quan do Gradio cung cấp.

**Dự án chính:** [ltteamvn/ReviewPhim](https://github.com/ltteamvn/ReviewPhim)
| 💻 Colab Runtime | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1nmdU6vTKRBnjRxHDKudFxdCGbIB4Q3RM?usp=sharing) |

---

## Giao diện web của Review Phim

![Giao diện Review Phim](https://github.com/ltteamvn/ReviewPhim/assets/114810545/0d71fbf4-e9f0-4f8f-944e-8f3f1ea6a019)

---


## Ngôn ngữ hỗ trợ dịch

| Mã ngôn ngữ | Tên ngôn ngữ              |
|-------------|---------------------------|
| en          | Tiếng Anh                 |
| fr          | Tiếng Pháp                |
| de          | Tiếng Đức                 |
| es          | Tiếng Tây Ban Nha         |
| it          | Tiếng Ý                   |
| ja          | Tiếng Nhật                |
| nl          | Tiếng Hà Lan              |
| uk          | Tiếng Ukraina             |
| pt          | Tiếng Bồ Đào Nha          |
| ar          | Tiếng Ả Rập               |
| zh          | Tiếng Trung Giản thể      |
| zh-TW       | Tiếng Trung Phồn thể      |
| cs          | Tiếng Séc                 |
| da          | Tiếng Đan Mạch            |
| fi          | Tiếng Phần Lan            |
| el          | Tiếng Hy Lạp              |
| he          | Tiếng Do Thái             |
| hu          | Tiếng Hungary             |
| ko          | Tiếng Hàn Quốc            |
| fa          | Tiếng Ba Tư (Persian)     |
| pl          | Tiếng Ba Lan              |
| ru          | Tiếng Nga                 |
| tr          | Tiếng Thổ Nhĩ Kỳ          |
| ur          | Tiếng Urdu                |
| hi          | Tiếng Hindi               |
| vi          | Tiếng Việt                |
| id          | Tiếng Indonesia           |
| bn          | Tiếng Bengal              |
| te          | Tiếng Telugu              |
| mr          | Tiếng Marathi             |
| ta          | Tiếng Tamil               |
| jw (jv)     | Tiếng Java                |
| ca          | Tiếng Catalan             |
| ne          | Tiếng Nepali              |
| th          | Tiếng Thái                |
| sv          | Tiếng Thụy Điển           |
| am          | Tiếng Amharic             |
| cy          | Tiếng Wales               |
| hr          | Tiếng Croatia             |
| is          | Tiếng Iceland             |
| ka          | Tiếng Georgia             |
| km          | Tiếng Khmer               |
| sk          | Tiếng Slovakia            |
| sq          | Tiếng Albania             |
| sr          | Tiếng Serbia              |
| az          | Tiếng Azerbaijan          |
| bg          | Tiếng Bulgaria            |
| gl          | Tiếng Galicia             |
| gu          | Tiếng Gujarati            |
| kk          | Tiếng Kazakh              |
| kn          | Tiếng Kannada             |
| lt          | Tiếng Lithuania           |
| lv          | Tiếng Latvia              |
| ml          | Tiếng Malayalam           |
| ro          | Tiếng Romania             |
| si          | Tiếng Sinhala             |
| su          | Tiếng Sunda               |
| et          | Tiếng Estonia             |
| mk          | Tiếng Macedonia           |
| sw          | Tiếng Swahili             |
| af          | Tiếng Afrikaans           |
| bs          | Tiếng Bosnia              |
| la          | Tiếng Latin               |
| my          | Tiếng Miến Điện (Burmese) |
| no          | Tiếng Na Uy               |
| as          | Tiếng Assamese            |
| eu          | Tiếng Basque              |
| ha          | Tiếng Hausa               |
| ht          | Tiếng Creole Haiti        |
| hy          | Tiếng Armenia             |
| lo          | Tiếng Lào                 |
| mg          | Tiếng Malagasy            |
| mn          | Tiếng Mông Cổ             |
| mt          | Tiếng Malta               |
| pa          | Tiếng Punjabi             |
| ps          | Tiếng Pashto              |
| sl          | Tiếng Slovenia            |
| sn          | Tiếng Shona               |
| so          | Tiếng Somali              |
| tg          | Tiếng Tajik               |
| tk          | Tiếng Turkmen             |
| tt          | Tiếng Tatar               |
| uz          | Tiếng Uzbek               |
| yo          | Tiếng Yoruba              |

### Ngôn ngữ không hỗ trợ phiên âm (chỉ dịch văn bản)

| Mã ngôn ngữ | Tên ngôn ngữ |
|-------------|--------------|
| ay          | Aymara       |
| bm          | Bambara      |
| ceb         | Cebuano      |
| ny          | Chichewa     |
| dv          | Divehi       |
| doi         | Dogri        |
| ee          | Ewe          |
| gn          | Guarani      |
| ilo         | Iloko        |
| rw          | Kinyarwanda  |
| kri         | Krio         |
| ku          | Kurdish      |
| ky          | Kirghiz      |
| lg          | Ganda        |
| mai         | Maithili     |
| or          | Oriya        |
| om          | Oromo        |
| qu          | Quechua      |
| sm          | Samoan       |
| ti          | Tigrinya     |
| ts          | Tsonga       |
| ak          | Akan         |
| ug          | Uighur       |

---

## Cài đặt và chạy Review Phim (Linux)

1. **Chuẩn bị**  
   - Cài NVIDIA driver (CUDA 11.8)  
   - Tạo token Hugging Face và chấp nhận license Pyannote  
   - Cài Anaconda/Miniconda và Git

2. **Tạo môi trường Conda**  
   ```bash
   conda create -n reviewphim python=3.10 -y
   conda activate reviewphim
   pip install pip==23.1.2
   conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia
````

3. **Clone và cài đặt**

   ```bash
   git clone https://github.com/ltteamvn/ReviewPhim.git
   cd ReviewPhim
   pip install -r requirements_base.txt
   pip install -r requirements_extra.txt
   pip install onnxruntime-gpu
   conda install -y ffmpeg
   ```

4. **Chạy ứng dụng**

   ```bash
   export HUGGINGFACE_TOKEN="YOUR_HF_TOKEN"
   python app_rvc.py
   ```

   Mở `http://127.0.0.1:7860` trên trình duyệt để truy cập giao diện Review Phim.

5. **Dừng ứng dụng**

   * Nhấn `Ctrl+C` trong terminal
   * `conda deactivate`

6. **Xóa sạch và bắt đầu lại**

   ```bash
   conda deactivate
   conda env remove -n reviewphim
   rm -rf ReviewPhim
   ```

---

## Tham số dòng lệnh

| Tham số             | Mặc định         | Mô tả                                                                                     |
| ------------------- | ---------------- | ----------------------------------------------------------------------------------------- |
| `--theme`           | Taithrah/Minimal | Chọn giao diện (xem [Theme Gallery](https://huggingface.co/spaces/gradio/theme-gallery)). |
| `--language`        | english          | Ngôn ngữ giao diện (ví dụ: vietnamese, french, german, v.v.).                             |
| `--verbosity_level` | info             | Mức độ log: debug, info, warning, error, critical.                                        |
| `--public_url`      |                  | Bật liên kết công khai.                                                                   |
| `--cpu_mode`        |                  | Chạy trên CPU thay vì GPU.                                                                |

Ví dụ:

```bash
python app_rvc.py --theme gradio/soft --language vietnamese
```

---

## Tin tức

* 🔥 **2025/05/18**: Thêm Overlap Reduction, tích hợp OpenAI API cho transcription/translation/TTS, nhiều tùy chọn xuất: phụ đề theo speaker, tách âm thanh, video chỉ có phụ đề…
* 🔥 **2025/03/02**: Giữ nguyên tên file, xử lý playlist YouTube, soft subtitles, batch processing, format MP3/MP4/MKV/WAV/OGG…
* 🔥 **2025/02/22**: Thêm freevc voice imitation, mở rộng GUI translation, burn subtitles, queue đa tác vụ, checkpoint resume…
* 🔥 **2025/01/16**: Hỗ trợ thêm nhiều ngôn ngữ (Thai, Nepali, Catalan…), tích hợp BARK, Coqui XTTS, Piper-TTS, audio separation…
* 🔥 **2024/10/29**: Chỉnh sửa phụ đề dịch, điều chỉnh volume/speed…
* 🔥 **2024/08/03**: Thay đổi mặc định, thư mục downloads view…
* 🔥 **2024/08/02**: Hỗ trợ thêm Ả Rập, Séc, Đan Mạch, Phần Lan, Hy Lạp, Do Thái, v.v.
* 🔥 **2024/07/27**: Sửa lỗi xử lý video/audio.
* 🔥 **2024/07/26**: Giao diện mới, thêm mix options.

---

## Đóng góp

Rất hoan nghênh mọi ý tưởng, bug report hoặc feature request. Vui lòng mở Issue hoặc Pull Request. Xem thêm hướng dẫn đóng góp trong repo.

---

## Tín dụng

Dự án sử dụng nhiều thư viện mã nguồn mở, cảm ơn các tác giả:

* [PyTorch](https://github.com/pytorch/pytorch)
* [yt-dlp](https://github.com/yt-dlp/yt-dlp)
* [Gradio](https://github.com/gradio-app/gradio)
* [edge-tts](https://github.com/rany2/edge-tts)
* [deep-translator](https://github.com/nidhaloff/deep-translator)
* [pyannote-audio](https://github.com/pyannote/pyannote-audio)
* [WhisperX](https://github.com/m-bain/whisperX)
* [faster-whisper](https://github.com/SYSTRAN/faster-whisper)
* [Transformers](https://github.com/huggingface/transformers)
* [FFmpeg](https://github.com/FFmpeg/FFmpeg)
* [Piper](https://github.com/rhasspy/piper)
* [Coqui TTS](https://github.com/coqui-ai/TTS)
* [pypdf](https://github.com/py-pdf/pypdf)
* [OpenVoice](https://github.com/myshell-ai/OpenVoice)

---