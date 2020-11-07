# Deep Learning Framework for Multi-modal Product Classification
Code repository for Rakuten Data Challenge : Multimodal Product Classification and Retrieval. 

Team Transformer's solution : Deep Multi-level Boosted Fusion Learning Framework for Multi-modal Product Classification 


Data challenge link : https://sigir-ecom.github.io/data-task.html


<p align="center">
  <img src="https://user-images.githubusercontent.com/56831322/89715638-a5ff2280-d9c4-11ea-9ca1-be884c8b9c26.png" />
</p>

<p align="center"> Multi-modal Joint Representation Learning </p> 



<p align="center">
  <img src="https://user-images.githubusercontent.com/56831322/89715668-f1193580-d9c4-11ea-8fcd-042e909ee30d.png" />
</p>

<p align="center"> Late Fusion Model </p> 


### Notebooks

#### Unimodal Model Training and Prediction Scripts

SEResnext50_train_predict.ipynb : Fine tune the pre-trained SEResnext50 model on Rakuten images

camembert_train_predict.ipynb : Fine tune the pre-trained Cammebert model on French text; Custom Cammbert model with vector output (used later for feature fusion)

flaubert_train_predict.ipynb : Fine tune the pre-trained Flaubert model on French text; Custom Flaubert model with vector output (used later for feature fusion)

