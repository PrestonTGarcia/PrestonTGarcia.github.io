---
title: Contrail Identification
date: 2023-08-09
tags:
  - Image Segmentation
  - Machine Learning
  - Atmospheric Sciences
---

A Kaggle competition tasked with identifying and segmenting condensation trails (contrails) in images of the sky.

<!--more-->

![Contrail Results](contrailresults.png "Contrail Results")

Contrails are line shaped clouds composed of water in the form of ice crystals. These contrails trap heat in the atmosphere, contributing to air pollution, global warming, and altering weather patterns. As a result, efforts are made by researchers within many fields, such as aerodynamics, space, and machine learning, to mitigate the effects of these contrails. The first step of mitigating these effects is to identify the contrails. A competition was held on Kaggle to develop a machine learning model that takes image frames of the sky as input, and outputs a masked version where the contrails are segmented from the sky in the background. Data in this competition included bands of images provieded by NASA and NOAA's [GOES-16 Baseline Imager](https://www.goes-r.gov/spacesegment/abi.html) satellite as described in the [Kaggle competition](https://www.kaggle.com/competitions/google-research-identify-contrails-reduce-global-warming/data)

Competing in this Kaggle competition has given me extensive experience in image segmentation and computer vision. Prior to this project, I had only done image classification projects, however, image segmentation was new to me, and would pose to be a challenge. I had learned the importance of image augmentation techniques such as normalization and cropping with neural networks, as well as some state of the art pretrained segmentation models, such as [UNet](https://github.com/milesial/Pytorch-UNet) and [UNet++](https://github.com/4uiiurz1/pytorch-nested-unet).

Models were evaluated using the dice coefficient on a test set of images consisting of two records. The [public leaderboard](https://www.kaggle.com/competitions/google-research-identify-contrails-reduce-global-warming/leaderboard?tab=public) uses 15% of the test data, and the [private leaderboard](https://www.kaggle.com/competitions/google-research-identify-contrails-reduce-global-warming/leaderboard?) uses 85% of the data. The training for models took more than 4 hours long per run on the Kaggle runtime environment, giving me problems with properly training my models. On the [public leaderboard](https://www.kaggle.com/competitions/google-research-identify-contrails-reduce-global-warming/leaderboard?tab=public) I earned a dice coefficient of 0.62283 and placed 682/954, and on the [private leaderboard](https://www.kaggle.com/competitions/google-research-identify-contrails-reduce-global-warming/leaderboard?) I earned a dice coefficient of 0.62833 and placed 663/954. To improve the models, different types of pretrained models could be used, as well as hyperparameter optimization.
