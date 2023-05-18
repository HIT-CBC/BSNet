# Prediction of HR status of breast cancer by weakly supervised deep learning model based on mammography images
Hormone receptor (HR) molecular status is commonly used clinical subtype information and is the foundation of precise treatment. However, subtyping diagnosis of breast cancer requires pathological biopsy, which may alter tumor morphology. Therefore, in this work, we intended to achieve non-invasive breast cancer diagnosis and provide HR status information through mammography screening. We used the multi-view of unlabeled mammography images to develop a weakly supervised deep learning framework BSNet with superior performance and implemented a webserver, which provided convenience for the subtype diagnosis of breast cancer.

![workflow - 副本-01-01](https://github.com/HIT-CBC/BSNet/assets/97509376/54411c7c-3a89-4ae3-84cf-5c0aed77fd00)

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


