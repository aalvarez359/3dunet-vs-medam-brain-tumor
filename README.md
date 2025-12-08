# 3dunet-vs-medam-brain-tumor
Repository for 3D U-Net vs MedSAM2 brain tumor MRI segmentation

Instructions for training, inference and metrics are written at the top of each python notebook. All notebooks were run in Google Colab.

Datasets can be found at here. MSD Task01_BrainTumour: http://medicaldecathlon.com/ and BraTS 2024: https://www.synapse.org/Synapse:syn53708249/wiki/626323

All weights, data split jsons, dataset jsons, and inference metrics can be found https://drive.google.com/drive/folders/1mAqbM9HJ6-J0_SWVOey-MJGGAeZSE3Md?usp=drive_link

Google Drive Directory Guide

weights: Contains all weights needed to replicat inference for each of the datasets and modalities. To run inference using the same weights that I did, make sure the inference script is pointed to the appropriate weight. checkpoint weights are for the highest attained dice score and last weights are for the last epoch's dice score.

dataset_json: Contains the json files containing image information needed to train on the dataset. To run training scripts, make sure model is directed to the appropriate json.

data_split_json: Contains json files that contain the training split for each dataset. To run training scripts using the same exact training spllit that I used, make sure the model is directed to the appropriate data split json file. Otherwise training will create a new random split when training begins.

inference: Contains csv results of each model's inference.  Use these to create table and graph metrics for inference statistics.

metrics: tables created by metric notebooks.

