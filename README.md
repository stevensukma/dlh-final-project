# Multi-Label Generalized Zero Shot Learning for the Classification of Ocular Diseases.

This repository is the final project for UIUC CS598: Deep Learning for Healthcare.

The aim is to extend the implementation of `Multi-Label Generalized Zero Shot Learning for the Classification of Disease in Chest Radiographs` (Hayat et al. 2021) on `ODIR-5K` datasets [link](https://odir2019.grand-challenge.org/dataset/)

## Requirements

To install requirements:

```setup
pip install -r requirements.txt
```

Dataset can be obtained from kaggle [link](https://www.kaggle.com/datasets/andrewmvd/ocular-disease-recognition-odir5k)

## Training

The example of training implementation of the network can be found on the jupyter notebook cell

```
trainer.train()
```

## Evaluation

The example of evaluation implementation of the network can be found on the jupyter notebook cell

```
trainer.test()
```

The target metrics is the AUROC of all classes in the dataset.

## Pre-trained Models

Pre-trained weight of the best epoch can be found in the checkpoints folder.

The mentioned weights are trained for 20 epochs using Nvidia L4 GPU on google collab environment.

## Results

Our model achieves the following performance on :

### [Image Classification on ImageNet](https://paperswithcode.com/sota/image-classification-on-imagenet)

| Class                            | Status | AUROC |
| -------------------------------- | ------ | ----- |
| Normal                           | Seen   | 0.71  |
| Diabetes                         | Seen   | 0.75  |
| Glaucoma                         | Seen   | 0.79  |
| Cataract                         | Seen   | 0.89  |
| Age-Related Macular Degeneration | Unseen | 0.43  |
| Hypertension                     | Seen   | 0.728 |
| Pathological Myopia              | Seen   | 0.94  |
| Other                            | Seen   | 0.61  |
