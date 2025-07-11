# 🧠 Image Sharpening Using Knowledge Distillation

This project presents an efficient, lightweight solution for sharpening blurry images using deep learning and *knowledge distillation. Designed for real-time video conferencing and low-bandwidth scenarios, the approach trains a compact **student model* to mimic a powerful *teacher model*, delivering fast and high-quality image restoration.

---

## 🔍 Problem Statement

In low-bandwidth or motion-intensive environments (like video calls), image quality suffers from blur and compression artifacts. Traditional sharpening filters fail to restore real detail. This project uses deep learning and *teacher-student distillation* to perform *intelligent image sharpening* using fewer resources.

---

## 🏁 Outcomes

The project produced strong results in terms of structural similarity and reconstruction quality:

- The Teacher Model achieved a Structural Similarity Index Measure (SSIM) of 0.7943 compared to the ground truth images.
- The Student Model, although significantly smaller, reached an SSIM of 0.7119 against the ground truth.
- In terms of Peak Signal-to-Noise Ratio (PSNR), the Teacher Model scored 27.48 dB, while the Student Model scored  25.78 dB , both evaluated against the ground truth.
- When comparing the Student Model’s output to the Teacher Model’s output, the SSIM was 0.9137, indicating the student effectively mimicked the teacher’s behavior.
- The PSNR between the Student Model and the  Teacher Model  was 34.09 dB, showing high visual fidelity between the two.

These results confirm the success of knowledge distillation in training a lightweight model that retains high performance with significantly reduced computational cost.
---

## ⚠ Limitations

- ⚙ *SSIM with ground truth* remains lower for the student model due to its reduced capacity.
- ⏱ *Training time* can be significant even for small models due to high-quality image data.
- 🎯 *Generalization* may vary for real-world low-quality inputs not seen during training.

---

## 🔭 Future Scope

- 🚀 *Improve student performance* via attention mechanisms or residual distillation
- 📱 Deploy on *mobile and edge devices* with real-time benchmarks
- 🧪 Extend to *video frame sharpening* with temporal consistency
- 💡 Incorporate *perceptual loss* or GAN-based enhancements for better visual quality

---

## 🛠 Tech Stack

- *PyTorch* for model design and training
- *SSIM* & *PSNR* for evaluation
- *DIV2K* dataset for high-resolution image pairs
- *Knowledge Distillation* using MSE + L1 loss and intermediate feature mimicry
---


## 🤝 Acknowledgment

This project was developed under the *Intel® Unnati Program* by Team Luminous from Saintgits College of Engineering. Special thanks to our mentor Mr. Siju Swamy and all academic and industry collaborators.

---

## 📬 Contact

For queries, reach out to:
- Angela Mary Thomas
- Fahim Shafeek
- Lakshmi Krishna V R
