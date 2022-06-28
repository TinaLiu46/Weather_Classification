# Weather_Classification

# Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [MONAI](#what-is-monai)
4. [Model Used](#model-used)
5. [Metric](#metric)
6. [Conclusion](#conclusion)

## Introduction
This project is intended to categorize input (weather images) into 11 categories. We will use deep learning  - "MONAI Pytorch" to train the images and generate an accurate model.

## Dataset
- Data Size : 636.73 MiB (~7000 Images)
- Features: 11 Categories (dew, fogsmog, frost, glaze, hail, lightning, rain, rainbow, rime, sandstorm, snow)
- Data Type: Images

![Goal2](https://github.com/TinaLiu46/Weather_Classification/blob/main/Images/data.png?raw=true "Title")

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


## Conclusion
By implementing deep learning method to train the images, we are able to categorize the weather into 11 categoris. We believe this model is applicable in many feilds since weather classification is becoming more and more important in the industry. 
