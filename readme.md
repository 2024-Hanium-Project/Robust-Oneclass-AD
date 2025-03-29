# SK-RD4AD: Skip-Connected Reverse Distillation for Robust One-Class Anomaly Detection

SK-RD4AD introduces a novel anomaly detection architecture that integrates **non-corresponding skip connections** into a reverse knowledge distillation framework.  
This design preserves **multi-scale visual features**, addressing deep feature loss in traditional models and enhancing both **anomaly localization** and **detection accuracy**.

---

## 🧠 Architecture

<p align="center">
  <img src="https://github.com/user-attachments/assets/64b2f6de-1ec1-4232-a86c-28a4f5836b3e" width="100%">
</p>

---

## 📊 Benchmark Results

| Dataset     | Metric         | RD4AD | SK-RD4AD |
|-------------|----------------|--------|-----------|
| **MVTec-AD** | Pixel AUROC    | 97.8   | **98.06** |
| **VisA**     | Pixel AUPRO    | 70.9   | **92.1**  |
| **VAD**      | AUROC          | 84.5   | **87.0**  |

> Evaluated on MVTec-AD, Valeo Anomaly Dataset (VAD), and VisA.

---

## 🖼️ Visual Results

<p align="center">
  <img src="https://github.com/user-attachments/assets/b2fe4e4b-6a4c-4c86-8caa-ebef8da92dd8" width="45%">
  <img src="https://github.com/user-attachments/assets/dbbd9d8a-f70a-4a8f-9a9b-49e2f95ed4be" width="45%">
</p>

Anomaly maps clearly highlight defective regions with high accuracy.  
Red/yellow hues indicate high anomaly confidence, overlayed on the original images for interpretability.

---

## 📝 Key Highlights

- **Non-Corresponding Skip Connections**: Enhances deep layer representations with fine-grained details.
- **Robust Generalization**: Performs reliably across various industrial and structural defect types.
- **Built on Reverse Distillation**: Based on the RD4AD backbone, improved for feature preservation.

---

## 📬 Contact

For inquiries or collaborations, contact:  
**Eun-ju Park** — pej0918@ewha.ac.kr
