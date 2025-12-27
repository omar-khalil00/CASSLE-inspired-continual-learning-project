# Continual Self-Supervised Learning with Distillation (CaSSLe-inspired)

## Overview
This project explores continual self-supervised learning using MAE and RotNet backbones.  
The focus is on studying **knowledge distillation** to reduce forgetting and improve stability across tasks.  

Datasets: CIFAR-100, ImageNet subsets  
Models: RotNet, MAE  
Pretraining: None / ImageNet / Places  

## Acknowledgment
This project is inspired by **Self-Supervised Models are Continual Learners**.  
The core idea of using self-distillation to mitigate catastrophic forgetting motivated this work.

Original paper:  
[Self-Supervised Models are Continual Learners](https://arxiv.org/pdf/2112.04215)

> Note: This is **not an official implementation**. It explores similar ideas using different architectures, datasets, and training setups.

## Method
- Train MAE and RotNet models on continual learning tasks  
- Compare **distillation vs no distillation**  
- Evaluate using **average accuracy** and **forgetting metrics**  
- Analyze the effect of pretraining (ImageNet / Places)  


### Plots

**Accuracy Comparison**  
![Accuracy](results/plots/accuracy_comparison.png)

**Forgetting Comparison**  
![Forgetting](results/plots/forgetting_comparison.png)

## Key Observations
- Distillation consistently reduces forgetting and improves average accuracy.  
- MAE shows stronger improvements than RotNet on CIFAR-100.  
- Pretraining stabilizes learning and boosts performance on ImageNet subsets.  


