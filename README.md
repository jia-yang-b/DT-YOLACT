DT-YOLACT
This repo. is the official implementation of "Nuclei Instance Segmentation and Classification in Histopathological Images using a DT-YOLACT" .
Please see the paper.
# DKS-DoubleU-Net

## Overview    
<img width="457" alt="image" src="https://user-images.githubusercontent.com/59470630/222135358-fefe13d4-785f-4079-903a-f6b8b88e8b02.png">
##  PQ bar graphs of different network models under different categories
<img width="361" alt="image" src="https://user-images.githubusercontent.com/59470630/222135722-2d9657e3-79f0-454b-8893-6e3614d8942d.png">
## MPQS in different organizations on different networks
<img width="361" alt="image" src="https://user-images.githubusercontent.com/59470630/222135775-4c03a3c6-166b-4794-a914-72dce0f1d24c.png">


## Run  
1.Requirements:  
* CUDA 9.0+cuDNN 7.1.4 
* Pytorch 1.0.1

train dataset：
*images：yolact/data/coco/train
*lables：yolact/data/coco/annotations/instances_cell_train.json

val dataset：
*images：yolact/data/coco/val
*lables：yolact/data/coco/annotations/instances_cell_val.json

test dataset：
*images：yolact/data/coco/test

2.Training:  
* Prepare the required images and store them in new_data folder, the example format of the training, validation, and testing datasets is in the  "yolact/data/coco" folder.

* Run ``` Python train.py –config=yolact_base_config```  

3.Testing:
* Run ```Python eval.py –trained_model=权重文件(pth) –score_threshold=0.15 –top_k=15 –images=input path:output path```

## Citation  




