<h1 align="center">Some Representative Anomaly Detection Datasets</h1>


<p align="center">
  <a href="#overview">Overview</a> •
  <a href="#datasets">Datasets</a> •
  <a href="#format">Format</a> •
  <a href="#acknowledgements">Acknowledgements</a> •
  <a href="#contact">Contact</a> 
</p>


<a name="overview"></a>
## 📌 Overview 

A collection of anomaly detection datasets, including 5 industrial datasets (**MVTec, VisA, BTAD, MPDD, BeltAD**) and 3 medical datasets (**BrainMRI, LiverCT, BUSI**). They are reorganized under a unified format to support standardized evaluation and reproducible benchmarking in FSAD studies.




<a name = "datasets"></a>
## 📂  Datasets 

<div style="font-size: 11px">

| Domain     | Dataset  | Our Link                                      | Official Link                                 | Type               | Modalities             | Classes | Res. Min | Res. Max | Train Normal | Test Normal | Test Anomaly |
| ---------- | -------- | --------------------------------------------- | --------------------------------------------- | ------------------ | ---------------------- | ------- | -------- | -------- | ------------ | ----------- | ------------ |
| Industrial | MVTec    | [Download](https://pan.quark.cn/s/e891e23fc0e4?pwd=unwi)                                 | [Official Website](https://www.mvtec.com/company/research/datasets/mvtec-ad)                         | Object & Texture   | Photography            | 15      | 700      | 1024     | 3629         | 467         | 1258         |
| Industrial | VisA     | [Download](https://pan.quark.cn/s/8ef7d5657a59?pwd=tm8L)                                 | [Official Website](https://github.com/amazon-science/spot-diff?tab=readme-ov-file#data-download)                         | Object             | Photography            | 12      | 960      | 1562     | 8629         | 962         | 1200         |
| Industrial | BTAD     | [Download](https://pan.quark.cn/s/f5292a1e473d?pwd=FbSY)                                 | [Official Website](http://avires.dimi.uniud.it/papers/btad/btad.zip)                         | Object & Texture   | Photography            | 3       | 600      | 1600     | 1799         | 451         | 290          |
| Industrial | MPDD     | [Download](https://pan.quark.cn/s/47490e894ea9?pwd=gPEA)                                 | [Official Website](https://vutbr-my.sharepoint.com/personal/xjezek16_vutbr_cz/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fxjezek16%5Fvutbr%5Fcz%2FDocuments%2FMPDD&ga=1)                         | Object             | Photography            | 6       | 1024     | 1024     | 888          | 176         | 282          |
| Industrial | BeltAD   | [Download](https://pan.quark.cn/s/07f695d9978e?)                                 | [Official Website](https://github.com/fayeH2/BeltAD)                         | Object             | Photography            | 1       | 1024     | 1024     | 502          | 35          | 550          |
| Medical    | BrainMRI | [Download](https://pan.quark.cn/s/6e245279a177?pwd=EqgP)                                 | [Official Website](http://braintumorsegmentation.org/)                         | Brain              | Radiology (MRI)        | 1       | 240      | 240      | 7500         | 679         | 3119         |
| Medical    | LiverCT  | [Download](https://pan.quark.cn/s/480c395cd2f3?pwd=U6Z2)                                 | [Official Website](https://github.com/DorisBao/BMAD)                         | Liver              | Radiology (CT)         | 1       | 512      | 512      | 1542         | 926         | 733          |
| Medical    | BUSI     | [Download](https://pan.quark.cn/s/1ef43c79796a?pwd=Jt6q)                                 | [Official Website](https://scholar.cu.edu.eg/?q=afahmy/pages/dataset)                         | Breast             | Radiology (Ultrasound) | 1       | 190      | 1048     | 133          | 133         | 697          |

---

</div>


<a name= "format"></a>
## 📁 Format

All reorganized datasets in this repository follow the **same unified directory format**, as illustrated below:

```
datasetName/
└── category/
    ├── train/
    │   └── good/
    │       ├── xxx.png
    │       └── ...
    ├── test/
    │   ├── good/
    │   │   └── ...
    │   ├── AnomalyType1/
    │   ├── AnomalyType2/
    │   └── ...
    └── ground_truth/
        ├── good/
        ├── AnomalyType1/
        ├── AnomalyType2/
        └── ...
```

### 📢 Directory Rules

* **train**: only contains normal samples, no anomaly images are included.

* **test**: contains both normal samples and various types of anomaly samples.

* **ground_truth**: provides pixel-level annotation masks for anomaly samples in the corresponding test folder.

---


<a name= "acknowledgements"></a>
## ⭐ Acknowledgements

We sincerely thank the original dataset creators and the open-source community for making these valuable resources available.

--- 

<a name= "contact"></a>
## 📧 Contact

For questions or suggestions: [jianghong@std.uestc.edu.cn](mailto:jianghong@std.uestc.edu.cn)
