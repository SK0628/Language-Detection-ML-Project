# Language-translator-ML-Project

# 🎙️ Real-Time Multilingual Voice Translator

## 📌 Project Overview
This Jupyter Notebook implements a real-time multilingual voice translation system using open-source Python tools. It allows users to speak in any language, automatically detects the spoken language, translates the speech into English, accepts a typed English reply, and then translates and speaks the reply back in the original language.

---

## 🚀 Features
- 🎤 Start/Stop voice recording
- 🌐 Language detection using Google Translate
- 🔁 English translation and reverse translation
- 🧠 Text-to-speech output for replies
- 🧩 Interactive widgets for user input and control
- 📦 Fully open-source and Jupyter-based

---

## 🛠️ Technologies & Libraries
- Python 3.x
- `SpeechRecognition` – for audio transcription
- `googletrans` – for translation
- `gTTS` – Google Text-to-Speech
- `sounddevice` and `scipy` – for audio recording
- `ipywidgets` – for GUI interface

---

## 🧪 Sample Interaction
| Input Language | User Says           | English Translation | User Reply | Translated Back      |
|----------------|---------------------|----------------------|-------------|-----------------------|
| Hindi          | Aap kaise ho?       | How are you?         | I am good.  | Main achha hoon.     |
| Spanish        | ¿Cómo estás?        | How are you?         | I am good.  | Estoy bien.          |

---

## 🖥️ How to Run
1. Clone the repository or open the `.ipynb` file in Jupyter Notebook.
2. Install the required dependencies:
```bash
pip install SpeechRecognition googletrans==4.0.0-rc1 gTTS sounddevice scipy ipywidgets
```
3. Click **Start Recording**, speak your sentence.
4. Click **Stop Recording**, the system will transcribe and translate.
5. Type your English reply and click **Submit**.
6. Your reply will be translated and spoken back in the original language.

---

## 📊 Performance Summary (Hypothetical)

| Language | Accuracy (%) | Latency (sec) |
|----------|--------------|----------------|
| Hindi    | 92           | 6              |
| Spanish  | 90           | 7              |
| French   | 88           | 7.5            |

---

## 🔮 Future Enhancements
- Streamlit web interface
- Use of official Google Translate or DeepL APIs
- Improved noise reduction and contextual translation
- Deployment on mobile/web platforms

---

## 📜 License
This project is released under the [MIT License](LICENSE).

---

## 👨‍🔬 Author
Developed by Shivam Kansara, 2025.
