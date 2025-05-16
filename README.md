# SRViT: Self-Supervised Relation-Aware Vision Transformer for Hyperspectral Unmixing

**Note:** SRViT codes are intended for academic communication only and may not be used commercially.

## Architectures and Systems
* SRViT can run under X86 and ARM architectures.\
* Two demos were tested x
* MacOS(M1/M2) will report some errors.
#---------------------------------------------------------------------------------------------\
├── Readme.md\
├── Environment: Python 3.8 and PyTorch 2.0 + cuDNN 11.8\
├── Demo\
│   ├── demo_synthetic_data.py\
│   └── demo_real_data.py\
│── Main Codes                      
│   ├── GSViT.py # Framework of SEViT\
│   ├── gsvit_emb.py                  
│   └── gsvit_tnt.py\
├── Auxiliary Codes                      
│   ├── utils.py\
│   ├── dataPro.py  
│   ├── plots.py\
│   └── vca.py\
├── Test data: real and synthetic data sets.\
│   ├── data_real/real.mat (Real data)\
│   └── synthetic_data.py\
│         ├── USGS_Library (Endmembers are given by randomly selecting library spectra.)\
│         └── data_synthetic/synthetic.mat (Synthetic data)\
└── Results files

## Specification
* 'synthetic_data' is a data generator that can generate different data sets by setting endmemers, 
window size, and SNR.
* For our synthetic_data, it's size, purity, SNR are adjustable for users' needs.
* 'demo_synthetic_data.py' uses a synthetic hyperspectral data.
* 'demo_real_data.py' use a challenging real hyperspectral data (samson data).


## Acknowledgment
Some codes in the SEViT file referred to the following works.\
[1] TNT: Transformer in Transformer, NeurIPS 2021.\
[2] DeepTrans-HSU: Hyperspectral Unmixing Using Transformer Network, IEEE TGRS 2022\
[3] ContraNorm: A Contrastive Learning Perspective on Oversmoothing and Beyond, ICLR 2023\
[4] Incorporating convolution designs into visual transformers, ICCV 2021\
[5] Masked autoencoders are scalable vision learners, CVPR 2022.
Many thanks to the authors of these remarkable works.

## Authors
- Yuanchao Su (suych3@xust.edu.cn)
- Lianru Gao (gaolr@aircas.ac.cn)
- Antonio Plaza 
- Mengying Jiang 
- Xu Sun 
- Guang Yang

## Date
March 2023
