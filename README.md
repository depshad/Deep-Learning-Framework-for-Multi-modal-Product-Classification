# Deep Learning Framework for Multi-modal Product Classification
Code repository for Rakuten Data Challenge : Multimodal Product Classification and Retrieval. 

Team Transformer's solution : Deep Multi-level Boosted Fusion Learning Framework for Multi-modal Product Classification 
 
Paper Link : https://sigir-ecom.github.io/ecom20DCPapers/SIGIR_eCom20_DC_paper_8.pdf


Data challenge link : https://sigir-ecom.github.io/data-task.html

## Abstract

In this paper, we present our approach for the ’Multimodal Product 
Classification’ task as a part of the 2020 SIGIR Workshop On eCommerce (ECOM20). The specific objective of this task is to build and
submit systems that classify previously unseen products into their
corresponding product type codes. We propose a deep Multi-Modal
Multi-level Boosted Fusion Learning Framework used to categorize
large-scale multi-modal (text and image) product data into product
type codes. Our proposed final methodology achieved a macro F1-
score of 91.94 on the phase 1 test dataset which is the top-scoring
submission and third position on the scoreboard for phase 2 test
dataset with macro F1-score of 90.53.

## Code Usage

### Unimodal Model Training and Prediction Scripts

1. SEResnext50_train_predict.ipynb : Fine tune the pre-trained SEResnext50 model on Rakuten images

2. camembert_train_predict.ipynb : Fine tune the pre-trained Cammebert model on French text; Custom Cammbert model with vector output (used later for feature fusion)

3. flaubert_train_predict.ipynb : Fine tune the pre-trained Flaubert model on French text; Custom Flaubert model with vector output (used later for feature fusion)

### Multimodal Feature Level Fusion
1. multi-modal_concatenate_fusion.ipynb : Concatenate the features extracted and train NN module on top

### Probability Level Fusion
1. Boosted Late-Fusion.ipynb : Train LightGBM model with class probability as input



<p align="center"> Multi-modal Joint Representation Learning </p> 

<p align="center">
  <img src="https://user-images.githubusercontent.com/56831322/89715638-a5ff2280-d9c4-11ea-9ca1-be884c8b9c26.png" />
</p>



<p align="center"> Late Fusion Model </p> 

<p align="center">
  <img src="https://user-images.githubusercontent.com/56831322/89715668-f1193580-d9c4-11ea-8fcd-042e909ee30d.png" />
</p>



