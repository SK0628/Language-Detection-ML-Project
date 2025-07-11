
# Real-Time Multilingual Language Identification Using MFCCs & Ensemble Learning

This project explores an efficient approach for **real-time multilingual language identification (LID)** 
using **MFCC (Mel-Frequency Cepstral Coefficient) features** and **ensemble learning models**. The focus is 
on designing and evaluating compact and accurate models that are feasible for **deployment on edge devices**, 
with low-latency inference and reduced resource consumption.

---

## 🔍 Overview

- **Dataset**: 149,370 speech clips (5s) across 6 languages.
- **Feature Extraction**: 13 static MFCCs extracted using Librosa.
- **Models Evaluated**:
  - Random Forest (100 trees)
  - Gradient Boosting (100 estimators)
  - Logistic Regression (max_iter=1000)
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score.
- **Inference Platform**: Raspberry Pi 4 to validate real-time feasibility.

---

## 🧠 Key Insights

- **Random Forest** achieved the best balance of accuracy (93%) and inference time (7ms).
- **Gradient Boosting** was robust to class imbalance but slower.
- **Logistic Regression** was fastest (3ms latency) but had the lowest accuracy.
- Top 5 MFCCs dominated language discrimination.

---

## 🛠️ Deployment Strategy

- Model quantization and pruning for resource-limited environments.
- Pipeline optimization for batch inference on ARM microcontrollers.
- Over-The-Air (OTA) updates for continuous learning in real-time systems.

---

## 📚 References (APA Format)

- Nie, Y., Zhao, J., Zhang, W. Q., & Bai, J. (2022). *BERT-LID: Leveraging BERT to Improve Spoken Language Identification*. arXiv preprint arXiv:2203.00328.
- Wong, A., Famouri, M., Pavlova, M., & Surana, S. (2020). *TinySpeech: Attention Condensers for Deep Speech Recognition Neural Networks on Edge Devices*. arXiv preprint arXiv:2008.04245.
- Lin, Z. Q., Chung, A. G., & Wong, A. (2018). *EdgeSpeechNets: Highly Efficient Deep Neural Networks for Speech Recognition on the Edge*. arXiv preprint arXiv:1810.08559.
- Khouas, A. R., Bouadjenek, M. R., Hacid, H., & Aryal, S. (2024). *Training Machine Learning Models at the Edge: A Survey*. arXiv preprint arXiv:2403.02619.
- Chakravarty, A. (2024). *Deep Learning Models in Speech Recognition: Measuring GPU Energy Consumption, Impact of Noise and Model Quantization for Edge Deployment*. Texas A&M University.
- Feng, C., Lin, Y., Zhuo, S., Su, C., Ramakrishnan, R. K., Yuan, Z., & Zhang, X. (2025). *Edge-ASR: Towards Low-Bit Quantization of Automatic Speech Recognition Models*. arXiv preprint arXiv:2507.07877.

---

## 📦 Files Included

- `Expanded_Real-Time_Language_ID_MFCC.docx`: Full academic paper (~1800 words, APA formatted).
- `Updated_Language_Detect_Presentation.pptx`: PowerPoint summarizing the project with new references.
- `Code.ipynb`: Jupyter Notebook
- `README.md`: This documentation file.

---

## 🧩 Future Work

- Integrate Whisper/Moonshine quantized models for multilingual LID.
- Benchmark against real-world conversational datasets.
- Expand to streaming audio input with live adaptive learning.
