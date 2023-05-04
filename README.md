# Prediction of HR status of breast cancer by weakly supervised deep learning model based on mammography images

![workflow - 副本-01](https://user-images.githubusercontent.com/97509376/236117355-94ecad88-2bfb-4840-891f-dbebae8393df.png)


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


