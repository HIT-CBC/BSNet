# Improving diagnosis and treatment efficiency based on multimodal data with distinguishing HR+ breast cancer
Hormone receptor (HR+) breast cancer (BC) accounts for a high proportion of patients with BC. Clinically, the heterogeneity of HR+ BC increases the difficulty of treatment options. Therefore, screening of HR+ BC from other patients with breast tumors and subgroup definitions are important for effective treatment. Here, we developed a sequential multimodal analysis framework called BSNet-CMBR for the diagnosis and subgrouping of HR+ BC. BSNet-CMBR included a weakly supervised deep learning model BSNet and a “MF genes” selection method CMBR for diagnosis and subgrouping in HR+ BC. BSNet was trained on 2321 multi-view mammography cases (9284 images) and was validated on the external heterogeneous cohort with average AUCs > 0.9 on the external validation set. The CMBR was proposed to classify and identify subgroups based on DNA methylation and scRNA-sequencing data. HR+/positive epidermal growth factor receptor-2 (HER2+) and HR+/negative epidermal growth factor receptor-2 (HER2-) were divided into two and three subgroups, which showed significant differences in DNA methylation levels, immune cell infiltration, immune checkpoints, immune cell cracking activity (CYT), tumor inflammation signature (TIS), and quantified pathological features. The BSNet-CMBR described high-dimensional mammographic and molecular features in HR+ BC subgroups, which helped inform individualized treatment decisions and early management options.

##
![workflow-01](https://user-images.githubusercontent.com/97509376/190979943-e8cd2370-0f77-4173-876d-620adeb5693f.png)


## Getting Started
Python3, pytorch>=1.8.0,torchvision>=0.7.0 are required for the current codebase
```
pip3 install torch==1.8.2+cu102 torchvision==0.9.2+cu102 torchaudio===0.8.2 -f https://download.pytorch.org/whl/lts/1.8/torch_lts.html
```
## Data preparation

The mammography images are placed according to the following categories
```
------Patient 1
         ------Patient 1_L_CC.png
         ------Patient 1_R_CC.png
         ------Patient 1_L_MLO.png
         ------Patient 1_R_MLO.png
------Patient 2
         ------Patient 2_L_CC.png
         ------Patient 2_R_CC.png
         ------Patient 2_L_MLO.png
         ------Patient 2_R_MLO.png
         
------Patient 3
         ------Patient 3_L_CC.png
         ------Patient 3_R_CC.png
         ------Patient 3_L_MLO.png
         ------Patient 3_R_MLO.png
...         

```

## Demo


* Train model:`bash ./run.sh`
* validate BSNet model:  `python test.py`  

## R code

Folders 1, 2, 3, and 4 are R code and data

* Folder 1 is the data preprocessing code and related data

* Folder 2 is the feature selection code and related data

* Folder 3 is the code and related data for the module selection

* Folder 4 is the clustering and typing code and related data
