[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wT71nrpQ)
# Colorouring grayscale photos
The main objective of this project is to automatically add colour on greyscale images. Note that the type of model which has been used is a Convolutional Neural Network Encoder- Decoder. Main task: Image Reconstruction.

The starting point for this project has been taken from: https://github.com/emilwallner/Coloring-greyscale-images

It is a must to underline that the basic architecture of all the models implemented consists on a basic CNN Endode- Decode architecture. Variations of the model will  be implemented on different alternatives to the baseline model; find these on the models folder.

Datasets used to train the models:
- https://github.com/2014mchidamb/DeepColorization/tree/master/face_images
- https://gist.github.com/mkocabas/a6177fc00315403d31572e17700d7fd9

Note that both of the datasets provided above contain colored images.

# Structure of the repository
The proposed solutions are implemented on different notebooks on the folder called models.

**Models folder**

In this folder all the implemented and proposed models will be implemented. For each model a different subfolder will be assigned. In all the subfolders at least the notebook with the implementation of the model and the corresponding README.md file will be found, apart from that additional files might be also found corresponding to the model.

## Getting started

In order to execute the models related to the dataset of the **face images** and **COCO image dataset** go to its corresponding README.md file and click on the google collab extention in order to run it. It must be pointed out that the data for the face images dataset must be first downloaded locally as it will have to be uploaded to the google collab enviroment.

<img width="946" alt="Screen Shot 2023-05-29 at 10 12 01 PM" src="https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/b88e76c5-bd65-47c0-94ef-19a90be96417">

In case you want to install the enviroment.

1. Clone our repository locally through you terminal.

```console
git clone https://github.com/DCC-UAB/dlnn-project_ia-group_03.git
```

2. Create a new conda enviroment.

```console
conda env create --file coloring_greyscale.yml
```

3. Activate the enviroment

```console
conda activate coloring_greyscale
```

4. Execute

```console
jupyter-notebook <name_of_notebook>.ipynb
```

*If certain libraries seems not to be installed, it must be done manually.*

## Note

The best performing models are the following:

1. CNN Encoder Decoder SE Block with face images
2. CNN Encoder Decoder SE Block with COCO dataset

## Contributors
- Members: Joan Samper, Alex Roldan, Adrián García
- Contacts: 1631430@uab.cat, 1636579@uab.cat, 1634605@uab.cat

Xarxes Neuronals i Aprenentatge Profund
Grau de Artificial Intelligence, UAB, 2023
