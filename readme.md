# Deep Learning Applied to COVID-19 Detection in X-Ray Images

## Summary
This repository contains the source code developed during the course of our research project, intended to develop a Computer Aided Diagnosis (CAD) tool for the COVID-19 disease using Chest X-Ray images (CXR) and Deep Learning methods. The code available covers from database processing and manipulation, preprocessing techniques to training, and evaluation, of classification and object detection models. It is recommended to run these notebooks using the [Google Colab](https://colab.research.google.com/) platform.

-----

## Contents
### Folders
- **utils:** contains Python files (.py) with various useful functions used in most notebooks. These functions include metrics, preprocessing operations, GradCam, among others.

- **Cov-Caldas Dataset** contains notebooks associated with data preparation and analysis for Cov-Caldas CXR dataset.

### Files
- **Database Processing - NPY from DICOM:** create a binary file (.npy) containing all the images from a directory structure and DICOM format. Faster load times and saves disk space.

- **Database Processing - Frontal and Lateral Projection Filtering:** training and evaluation of a model to classify CXR based on the projection it was taken from.

- **Database Processing - Lung Segmentation:** training and evaluation of a U-Net model to perform semantic segmentation of the lung region in CXR.

- **COVID-19 Classification with VGG16 and VGG19:** training and evaluation of VGG16 and VGG19 models to classify CXR into positive or negative for COVID-19.

- **COVID-19 Detection in X-Ray Images using Convolutional Neural Networks:** full experimental setup for the paper *[COVID-19 detection in X-ray images using convolutional neural networks][1]* (2021).

- **GGO Localization with Bounding Boxes and YOLOv5:** training and evaluation of the [YOLOv5][2] algorithm to detect Ground Glass Opacities (GGO) in CXR.

- **GGO Segmentation:** training and evaluation of multiple semantic segmentation models to detect Ground Glass Opacities (GGO) in CXR.

-----

## Data sources
In the development of this project we have used multiple databases, most of them are publicly available, but others remain private with the intention be released soon.

A curated version, including the partition into train, validation and test sets, are available via a [Code Ocean Capsule][3]. In particular, the files published correspond to the ones used in the notebook [COVID-19 Detection in X-Ray Images using Convolutional Neural Networks][4].

### Other databases
- BIMCV-COVID19+: https://bimcv.cipf.es/bimcv-projects/bimcv-covid19/.

- BRIXIA: https://brixia.github.io/.

- ML Hannover: https://data.uni-hannover.de/dataset/cov-19-img.

- Cancer Image Archive: https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=70226443.

- Covid Data Save lives: https://www.hmhospitales.com/coronavirus/covid-data-save-lives/english-version.

- IEEE8023: https://github.com/ieee8023/covid-chestxray-dataset.

- Padchest: https://bimcv.cipf.es/bimcv-projects/padchest/ or https://bimcv.cipf.es/bimcv-projects/bimcv-covid19/#1590857662078-c30d2790-05dc.

- BIMCV-COVID-: https://bimcv.cipf.es/bimcv-projects/bimcv-covid19/#1590859488150-148be708-c3f3.

- CheXpert: https://stanfordmlgroup.github.io/competitions/chexpert/.

- RSNA: https://www.kaggle.com/c/rsna-pneumonia-detection-challenge.

- Chest X-Ray Images (Pneumonia): https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia.

-----

## Products
- D. Arias-Garzón et al., “COVID-19 detection in X-ray images using convolutional neural networks,” *Mach. Learn. with Appl.*, vol. 6, p. 100138, Dec. 2021, doi: [10.1016/j.mlwa.2021.100138][1].

```
@article{ARIASGARZON2021100138,
title = {COVID-19 detection in X-ray images using convolutional neural networks},
journal = {Machine Learning with Applications},
volume = {6},
pages = {100138},
year = {2021},
issn = {2666-8270},
doi = {https://doi.org/10.1016/j.mlwa.2021.100138},
url = {https://www.sciencedirect.com/science/article/pii/S2666827021000694},
author = {Daniel Arias-Garzón and Jesús Alejandro Alzate-Grisales and Simon Orozco-Arias and Harold Brayan Arteaga-Arteaga and Mario Alejandro Bravo-Ortiz and Alejandro Mora-Rubio and Jose Manuel Saborit-Torres and Joaquim Ángel Montell Serrano and Maria {de la Iglesia Vayá} and Oscar Cardona-Morales and Reinel Tabares-Soto},
keywords = {COVID-19, Deep learning, Transfer learning, X-ray, Segmentation}
}
```

-----

## Acknowledgment
This work was supported by the Regional Ministry of Health of the Valencia Region, “The Medical Image Bank of the Valencian Community (BIMCV).” Part of the infrastructure used has been co-funded by the European Union through the Operational Program of the European Fund of Regional Development (FEDER) of the Valencian Community 2014-2020.

### Funding
This work was supported by the National Ministery of Technology and Information (Minciencias) Colombia with the identification code 0831-2020.


[1]: <https://doi.org/10.1016/j.mlwa.2021.100138>
[2]: <https://github.com/ultralytics/yolov5>
[3]: <https://codeocean.com/capsule/8595156/tree>
[4]: <COVID-19 Detection in X-Ray Images using Convolutional Neural Networks.ipynb>
