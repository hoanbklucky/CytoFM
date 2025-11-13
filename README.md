# CytoFM: The first cytology foundation model

Authors: Vedrana Ivezić, Ashwath Radhachandran, Ekaterina Redekop, Shreeram Athreya, Dongwoo Lee, Vivek Sant, Corey Arnold, William Speier

Accepted to the 10th IEEE Workshop on Computer Vision for Microscopy Image Analysis (CVMI) at CVPR 2025

([full paper](https://arxiv.org/pdf/2504.13402))

### Abstract
Cytology is essential for cancer diagnostics and screening due to its minimally invasive nature. However, the development of robust deep learning models for digital cytology is challenging due to the heterogeneity in staining and preparation methods of samples, differences across organs, and the limited availability of large, diverse, annotated datasets. Developing a task-specific model for every cytology application is impractical and non-cytology-specific foundation models struggle to generalize to tasks in this domain where the emphasis is on cell morphology. To address these challenges, we introduce CytoFM, the first cytology self-supervised foundation model. Using iBOT, a selfsupervised Vision Transformer (ViT) training framework incorporating masked image modeling and self-distillation, we pretrain CytoFM on a diverse collection of cytology datasets to learn robust, transferable representations. We evaluate CytoFM on multiple downstream cytology tasks, including breast cancer classification and cell type identification, using an attention-based multiple instance learning framework. Our results demonstrate that CytoFM performs better on two out of three downstream tasks than existing foundation models pretrained on histopathology (UNI) or natural images (iBOT-Imagenet). Visualizations of learned representations demonstrate our model is able to attend to cytologically relevant features. Despite a small pre-training dataset, CytoFM’s promising results highlight the ability of task-agnostic pre-training approaches to learn robust and generalizable features from cytology data.


### :bangbang: Weights release :bangbang:

Please find the weights used for CytoFM [here](https://drive.google.com/file/d/1iG1OcQTzXNzpjnSXHu79Zs5WqyTznf4a/view?usp=sharing). We have provided a notebook with an example of how to load in weights to the vit_base model adapted from the iBOT github. Setting up the iBOT code is a requirement to run this notebook. Please feel free to open an issue or send an email if there are any questions. 



### Acknowledgement
The code for this project was built using [iBOT: Image BERT Pre-Training with Online Tokenizer](https://github.com/bytedance/ibot). 


