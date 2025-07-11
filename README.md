# 🧠 Image Sharpening Using Knowledge Distillation

This project presents an efficient, lightweight solution for sharpening blurry images using deep learning and *knowledge distillation. Designed for real-time video conferencing and low-bandwidth scenarios, the approach trains a compact **student model* to mimic a powerful *teacher model*, delivering fast and high-quality image restoration.

---

## 🔍 Problem Statement

In low-bandwidth or motion-intensive environments (like video calls), image quality suffers from blur and compression artifacts. Traditional sharpening filters fail to restore real detail. This project uses deep learning and *teacher-student distillation* to perform *intelligent image sharpening* using fewer resources.

---

## 🏁 Outcomes

| Metric             | Teacher Model | Student Model |
|--------------------|---------------|---------------|
| SSIM vs GT         | *0.7943*    | 0.7119        |
| PSNR vs GT (dB)    | *27.48*     | 25.78         |
| SSIM vs Teacher    | —             | *0.9137*    |
| PSNR vs Teacher    | —             | *34.09*     |

- ✅ *Student model* is over *180× smaller* than the teacher (13K vs 2.5M parameters)
- ✅ Performs comparably while consuming minimal resources
- ✅ Ideal for deployment on edge devices or mobile systems

---

## ⚠ Limitations

- ⚙ *SSIM with ground truth* remains lower for the student model due to its reduced capacity.
- ⏱ *Training time* can be significant even for small models due to high-quality image data.
- 🎯 *Generalization* may vary for real-world low-quality inputs not seen during training.
- 🔄 Requires *pretrained teacher model*, adding complexity in deployment pipeline.

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

## 🤝 Acknowledgment

This project was developed under the *Intel® Unnati Program* by Team Luminous from Saintgits College of Engineering. Special thanks to our mentor Mr. Siju Swamy and all academic and industry collaborators.

---

## 📬 Contact

For queries, reach out to:
- Angela Mary Thomas
- Fahim Shafeek
- Lakshmi Krishna V R
