# Covid-Classification-and-Severity-Prediction

COVID-19 seems to be an extremely contagious disease and rapid human-to-human transition rate spreading quickly.
It is also associated with high ICU admission resulting in an urgent need for development of fast and accurate detection and diagnosis.
Identifying positive COVID-19 in early stages helps in isolation and breaking the infection chain.

In this project, we have created the classification model and the severity model for the detection of Covid-19 and evaluation of its severity from chest xrays.

## Dataset

### Lung Segmentation Dataset

* [Montgomery](https://data.lhncbc.nlm.nih.gov/public/Tuberculosis-Chest-X-ray-Datasets/Montgomery-County-CXR-Set/MontgomerySet/index.htmlhttps://data.lhncbc.nlm.nih.gov/public/Tuberculosis-Chest-X-ray-Datasets/Montgomery-County-CXR-Set/MontgomerySet/index.html)
* [Shenzhen](https://data.lhncbc.nlm.nih.gov/public/Tuberculosis-Chest-X-ray-Datasets/Shenzhen-Hospital-CXR-Set/index.html)
* [JSRT](http://db.jsrt.or.jp/eng.php)

### Classification Dataset

[Chest Radiography](https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database)

### Severity Dataset

[Brixia](https://brixia.github.io/)


## Architecture

### Classification

<img src="https://github.com/EkanshNishad/Covid-Classification-and-Severity-Prediction/blob/main/images/image8.jpg?raw=true" width="350">

### Severity

<img src="https://github.com/EkanshNishad/Covid-Classification-and-Severity-Prediction/blob/main/images/image9.png?raw=true" width="350">



## Results

### Segmentation Results

Dice Loss: 0.0221
IOU: 0.9790
Recall: 0.9903
Precision: 0.9924

### Classification Results

| Models               | Accuracy |
|----------------------|----------|
| Conv-Capsule Network | 93.98%   |
| Covid-Net            | 93.3%    |
| Xception             | 92.85%   |
| DarkNet              | 87.02%   |
| CoroNet(Xception)    | 89.6%    |

### Severity Results

| Model         | MAE (A, B, C, D, E, F)                          | MSE (A, B, C, D, E, F)                          |
|---------------|-------------------------------------------------|-------------------------------------------------|
| ResNet50      | 0.8509, 0.8513, 0.7953, 0.8434, 0.7910, 0.69    | 0.9678, 0.9804, 0.8938, 0.9164, 0.8575, 0.695   |
| DenseNet 201  | 0.4655, 0.7565, 0.7361, 0.8706, 0.4987, 0.6809  | 0.3351, 0.8612, 0.7463, 0.9684, 0.3874, 0.6442  |
| VGG16         | 0.9252, 0.9481,  0.9328, 0.9704, 0.8948, 0.8834 | 1.0761, 1.1396, 1.1211, 1.1391, 1.0231, 1.0268  |

## Models

Find other models at [link](https://drive.google.com/drive/folders/1iaLxMkzMKdV_FXPhbJW8TN2LVK_GU-oV?usp=sharing)




