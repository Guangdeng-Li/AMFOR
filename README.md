# AMFOR: Adaptive Multi-Granularity Fusion and Occlusion Reconstruction for Person Re-Identification 📚

<div align="center">

[![Paper](https://img.shields.io/badge/Paper-IEEE%20TMM-blue)](https://ieeexplore.ieee.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8+-orange.svg)](https://python.org)

**🎉 Accepted by IEEE Transactions on Multimedia 🎉**

</div>

---

## 📖 Abstract

Occluded person re-identification (ReID) poses substantial challenges in computer vision, primarily due to incomplete information and occlusion interference. Although Transformer architectures have become dominant in ReID due to their strong feature modeling capabilities, their lack of an adaptive weight allocation mechanism for multi-granularity feature processing limits their ability to extract generalizable and robust features. Recently, Masked Image Modeling (MIM) has demonstrated considerable promise in visual tasks, but its integration into ReID models remains underexplored. 

This paper presents **AMFOR** (Adaptive Multi-granularity feature Fusion and Occlusion Reconstruction), a novel framework combining MIM and Transformer architectures. AMFOR consists of three key components: AMFFEncoder, HPR-Decoder, and Teacher-Student Decoder. The AMFFEncoder enables adaptive fusion of multi-granularity features through learnable queries, allowing interaction between text-visual features and visual features extracted from multiple Transformer layers. The HPR-Decoder conceptualizes occluded regions in pedestrian images as reconstructable patches, guiding the encoder to extract more discriminative features through reconstruction. Additionally, the self-distillation teacher-student decoder is employed to refine pedestrian part features, further optimized by the proposed AMGDLoss. 

**This paper represents the first successful implementation of the MIM mechanism in person ReID models.** Empirical evaluations on five benchmark datasets, covering both occluded (Occluded-DukeMTMC, Occluded-REID, and PDukeMTMC-reID) and complete (Market-1501 and DukeMTMCreID) scenarios, demonstrate that AMFOR outperforms existing state-of-the-art methods in person ReID.

---

## 🏗️ Framework Overview

<div align="center">
<img src="figs/1.jpg" alt="AMFOR Introduction" width="800">
<p><em>Figure 1: Overview of the AMFOR framework for occluded person re-identification</em></p>
</div>

### 🔧 AMFOR Architecture

<div align="center">
<img src="figs/2.jpg" alt="AMFOR Framework" width="800">
<p><em>Figure 2: Detailed architecture of the AMFOR framework</em></p>
</div>

### 🧩 Key Components

#### AMFF-Encoder

<div align="center">
<img src="figs/3.jpg" alt="AMFF-Encoder" width="500">
<p><em>Figure 3: Adaptive Multi-granularity Feature Fusion Encoder</em></p>
</div>

#### HPR-Decoder

<div align="center">
<img src="figs/4.jpg" alt="HPR-Decoder" width="500">
<p><em>Figure 4: Human Part Reconstruction Decoder</em></p>
</div>

#### AMGDLoss

<div align="center">
<img src="figs/5.jpg" alt="AMGDLoss" width="600">
<p><em>Figure 5: Adaptive Multi-Granularity Distillation Loss</em></p>
</div>

---

## 📰 News 🔥

- **[2025.07]** 🎉 **Paper accepted by IEEE Transactions on Multimedia!**
- **[2025.01]** 📊 Update benchmark results
- **[2025.01]** 💻 Code will be released soon!

## 📊 Experimental Results

### 🏆 Benchmark Performance (mAP/Rank-1)

<div align="center">

| **Method** | **Occluded-Duke** | **Occluded-REID** | **P-Duke-MTMC** | **Market-1501** | **DukeMTMC-ReID** |
| :--------------: | :---------------------: | :---------------------: | :--------------------: | :--------------------: | :---------------------: |
| **AMFOR** | **72.1/81.7** ⭐ | **84.1/88.8** ⭐ | **87.4/94.2** ⭐ | **94.0/97.4** ⭐ | **89.0/94.5** ⭐ |

</div>

> 🎯 **Key Achievements:**
>
> - **State-of-the-art performance** across all five benchmark datasets
> - **Superior results** on both occluded and complete person ReID scenarios
> - **First successful integration** of MIM mechanism in person ReID

---

## 📋 TODO List

- [ ] 🚀 Release training code
- [ ] 🤖 Release pretrained models
- [ ] 📚 Add detailed documentation
- [ ] 🎥 Add demo videos
- [ ] 🔧 Provide installation guide
- [ ] 📖 Add technical paper link

---

## 🚀 Quick Start

### Prerequisites
```bash
Python >= 3.8
PyTorch >= 1.8.0
CUDA >= 11.0
```

### Installation
```bash
# Clone the repository
git clone https://github.com/your-username/AMFOR.git
cd AMFOR

# Install dependencies (coming soon)
pip install -r requirements.txt
```

### Usage
```bash
# Training (coming soon)
python train.py --config configs/amfor.yaml

# Evaluation (coming soon)
python test.py --config configs/amfor.yaml --checkpoint path/to/model.pth
```

---

## 🤝 Citation

If you find this work useful for your research, please consider citing:

```bibtex
@article{amfor2025,
  title={AMFOR: Adaptive Multi-Granularity Fusion and Occlusion Reconstruction for Person Re-Identification},
  author={Your Name and Co-authors},
  journal={IEEE Transactions on Multimedia},
  year={2025},
  publisher={IEEE}
}
```

---

## 📞 Contact

For questions and feedback, please contact:
- 📧 Email: [your.email@university.edu](mailto:your.email@university.edu)
- 🐛 Issues: [GitHub Issues](https://github.com/your-username/AMFOR/issues)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">

**⭐ If you find this project helpful, please give it a star! ⭐**

</div>
