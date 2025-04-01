# Research on Improving One-Class Anomaly Detection for Robustness

> 💻 **Developed through an ICT Vision AI Project**
> 
> 🎉 Our model was accepted at **CVPR 2025 Workshop**
> 
> 📌 **Official Implementation code: [SK-RD4AD](https://github.com/pej0918/SK-RD4AD)**

This research focuses on improving the robustness and localization ability of one-class anomaly detection models by introducing **non-corresponding skip connections** into a **reverse distillation framework**.

To address the limitations of deep-layer feature loss in conventional reverse distillation frameworks, we propose a novel skip-connected design that enhances **multi-scale feature preservation** and **localization accuracy**.

---

## 🧠 Architecture

![image](https://github.com/user-attachments/assets/51916259-a0a4-4d39-aaa0-ee170d87cfe6)

---

## 📊 Benchmark Results

| Dataset     | Metric         | RD4AD | SK-RD4AD |
|-------------|----------------|--------|-----------|
| **MVTec-AD** | Pixel AUROC    | 97.8   | **98.06** |
| **VisA**     | Pixel AUPRO    | 70.9   | **92.1**  |
| **VAD**      | AUROC          | 84.5   | **87.0**  |

> Evaluated on MVTec-AD, Valeo Anomaly Dataset (VAD), and VisA.
---

## 📈 Result Analysis

Our experiments demonstrate that **SK-RD4AD significantly improves anomaly localization**, particularly in datasets with complex textures (e.g., VisA) or subtle defects (e.g., VAD).  
The introduction of **non-corresponding skip connections** enables better flow of spatial detail into deeper layers, allowing the model to detect fine-grained anomalies more precisely.

- On **VisA**, the Pixel AUPRO improved by **+21.2**, showing enhanced ability to localize structural anomalies in PCB data.
- On **VAD**, the model showed better generalization across real-world driving scenarios, achieving **+2.5 AUROC** gain.
- Even on **MVTec**, where performance is already strong, the model shows consistent gains, indicating stability.

These results validate the hypothesis that **feature loss in deep layers** is a core limitation in prior work, and that **skip-connected reverse distillation** can effectively address this issue.

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

## 🎥 Demo Video (Korean ver.)

[![Watch the demo](https://img.youtube.com/vi/RgY_UKld6DM/0.jpg)](https://www.youtube.com/watch?v=RgY_UKld6DM)
