Title: Mapping and Classification of Field Margin Vegetation using High Resolution Satellite Imagery and Deep Learning Models in a Tropical Landscape
Authors: Satya Prakash1,2*, Michael Wachendorf1, Sunil Nautiyal2, Jayan Wijesingha1
Affiliation: 1Section of Grassland Science and Renewable Plant Resources, Faculty of Organic Agricultural Sciences, University of Kassel, Steinstraße 19, D-37213 Witzenhausen Germany
2Centre for Ecological Economics and Natural Resource, Institute for Social and Economic Change, Bengaluru, India

Background:
This repository contains the Python scripts used to delineate and classify field margin vegetation (FMV) in a tropical landscape. The workflow uses WorldView-3 multispectral imagery and deep-learning segmentation models, including U-Net and DeepLabV3+.
This workflow first delineated FMV from the surrounding landscape and then classifies the detected vegetation into woody and non-woody FMV.

Associated publication:
These scripts accompany the following research article:
Prakash, S., et al. (2026). Mapping and Classification of Field Margin Vegetation using High Resolution Satellite Imagery and Deep Learning Models in a Tropical Landscape.
DOI: To be added after publication.

Workflow:
1. Prepare and normalize WorldView-3 imagery and FMV sample.
2. Generate image chips and corresponding reference masks.
3. Apply data augmentation.
4. Train the binary FMV segmentation model.
5. Predict FMV masks.
6. Apply the predicted FMV mask to the classification workflow.
7. Classify FMV as woody or non-woody.
8. Evaluate the models and generate full-area predictions.

Worldview-3 band specifications:
The WorldView-3 imagery contains eight multispectral bands:
Spatial resolution 1.24m
1. Coastal blue
2. Blue
3. Green
4. Yellow
5. Red
6. Red edge
7. Near-infrared 1
8. Near-infrared 2

Software requirements:
The scripts were developed using Python 3.8.10 (Jupyter lab) and require:
- TensorFlow
- NumPy
- Rasterio
- GeoPandas
- scikit-learn
- scikit-image
- Matplotlib
- Pandas

Data availability:
The WorldView-3 imagery used in this study was obtained under a commercial data licence and therefore cannot be redistributed through this repository.
Users wishing to reproduce the complete workflow must obtain suitable high-resolution satellite imagery independently and update the input paths and configuration parameters accordingly.
The repository provides the processing, model-training, prediction, and evaluation scripts. Any example data, reference annotations, trained model weights, or derived products are shared only where permitted by the applicable data licence.

Citation:
If you use this code, please cite the associated publication and this
repository.

A formal citation will be provided after publication of the article.

For any query:
Satya Prakash 
Section of Grassland Science and Renewable Plant Resources
University of Kassel  
Email: satya.prakash@uni-kassel.de; satyaprakash724.sp@gmail.com
