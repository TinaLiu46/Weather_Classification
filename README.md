# Weather_Classification

## Introduction
This project is intended to categorize input (weather images) into 11 categories. We will use deep learning  - "MONAI Pytorch" to train the images and generate an accurate model.

## Dataset
![Goal2](https://github.com/TinaLiu46/Predicting-Dogecoin-Stock-Performance-using-Twitter-Data/blob/main/Images/goal3.png?raw=true "Title")

## What is MONAI

- open-source foundation being created by Project MONAI
- freely available, community-supported, PyTorch-based framework for deep learning 
- domain-optimized foundational capabilities 

## Model Used
```
model = DenseNet121(
    spatial_dims=2,            
    in_channels=1,
    out_channels=num_class,
).to(device)
```

## Metric 

| precision | recall | f1-score   |
| ------------- | ------------- | ------------- |
| 0.6529  | 0.6410  | 0.6436|

