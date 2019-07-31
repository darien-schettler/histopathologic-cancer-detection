# histopathologic-cancer-detection
EDA and baseline machine learning model prediction for histopathologic cancer detection challenge via Kaggle
# A Jupyter Notebook For Investigating and Creating Baseline Models For Histopathologic Cancer Detection

As the title suggests. This is a jupyter notebook that utilizes basic machine learning and data exploration techniques to both explore, and create a baseline model for, the dataset/competition *'Histopathologic Cancer Detection'*. <br>The following is the information from Kaggle:<br><br>

```
Create an algorithm to identify metastatic cancer in small image patches taken from larger digital pathology scans. The data for this competition is a slightly modified version of the PatchCamelyon (PCam) benchmark dataset (the original PCam dataset contains duplicate images due to its probabilistic sampling, however, the version presented on Kaggle does not contain duplicates).

PCam is highly interesting for both its size, simplicity to get started on, and approachability. In the authors' words:

[PCam] packs the clinically-relevant task of metastasis detection into a straight-forward binary image classification task, akin to CIFAR-10 and MNIST. Models can easily be trained on a single GPU in a couple hours, and achieve competitive scores in the Camelyon16 tasks of tumor detection and whole-slide image diagnosis. Furthermore, the balance between task-difficulty and tractability makes it a prime suspect for fundamental machine learning research on topics as active learning, model uncertainty, and explainability.
```

## Getting Started

```
1. Clone this repository
2. Create an environment (and activate it) and install the requirements.txt file
3. Download the dataset from [here](https://github.com/basveeling/pcam)
4. To match how I stored my data. Create a Data folder and nest within it input, output, and other folders (and populate accordingly)
5. Launch jupyter
6. Open the file from the cloned repositry
7. Enjoy
```

*NOTE: The data via the link is provided under the CC0 License, following the license of Camelyon16.*


## Prerequisites

```
absl-py==0.7.1
astor==0.8.0
cycler==0.10.0
gast==0.2.2
google-pasta==0.1.7
grpcio==1.22.0
h5py==2.9.0
joblib==0.13.2
Keras==2.2.4
Keras-Applications==1.0.8
Keras-Preprocessing==1.1.0
kiwisolver==1.1.0
Markdown==3.1.1
matplotlib==3.1.1
numpy==1.17.0
pandas==0.25.0
protobuf==3.9.0
pyparsing==2.4.2
python-dateutil==2.8.0
pytz==2019.1
PyYAML==5.1.1
scikit-learn==0.21.3
scipy==1.3.0
seaborn==0.9.0
six==1.12.0
sklearn==0.0
tensorboard==1.14.0
tensorflow==1.14.0
tensorflow-estimator==1.14.0
termcolor==1.1.0
Werkzeug==0.15.5
wrapt==1.11.2
```

## Installation
**NOTE: all shell commands are via the windows command line... you can find alternatives for linux fairly easily**

1. Clone this repository and navigate into it within the command line

2. Create and activate an environment (if you wish)<br>
` python -m venv env `<br>
` env\scripts\activate `<br>
` python -m pip install --upgrade pip `<br>

3. Execute the following commands to install all the requiremets<br>
` pip install -r requirements.txt`<br>

4. Join this competition to be able to download the dataset (or find it directly via NOAA) and create the following folder structure<br>
```
histopathologic-cancer-detection
|---- requirements.txt
|
|---- histopathologic-cancer-detection-eda.ipynb
|---- histopathologic-cancer-detection-model.ipynb
|
|---- data
|\
| \
|  \
|   |---- train_labels.csv
|   |---- inline-images
|   |   |---- cancer_1.png
|   |   |---- cancer_2.png
|   |   '---- cancer_3.png
|   |---- train
|   |   |---- xyz.png
|   |   |---- xyz.png
|   |   '---- xyz.png
|   |---- val
|   |   |---- xyz.png
|   |   |---- xyz.png
|   |   '---- xyz.png
|   |---- test
|   |   |---- xyz.png
|   |   |---- xyz.png
|   |   '---- xyz.png
|  /
| /
|/
|---- README.md
|---- LICENSE.md
|---- CONTRIBUTING.md
```
4. To open the jupyter environment run the following<br>
` jupyter notebook --port=8888`<br>

5. Navigate to the cloned directory and open the .ipynb file<br><br>
***See deployment for notes on how to deploy the project on a live system.***

## Deployment

To deploy this on a system and leave it running, you will need to attach the jupyter instance to a seperate 'screen' in the terminal/cmd prompt. There are different ways of doing this but you should be able to find the appropriate documentation easily. <br>
As this is a learning tool, there is no further information regarding deployment via docker, etc.

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests.

## Authors

**Darien Schettler** -- [Portfolio](http://darienschettler.ca/) -- [Github](https://github.com/darien-schettler)


## Licensing

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
