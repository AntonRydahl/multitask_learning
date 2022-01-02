# Diagnosis Correction Using Domain Knowledge
In this project a multitask classification deep neural network has been trained to predict dermatological diagnoses and visible symptoms. The networks have been trained on the images of patients and the predictions have been compared to expert classifications of the images.<br>
Note that this project has been carried out in <a href="https://colab.research.google.com/">Google Colab</a>. Thus the *.ipynb*-files cannot be run directly by cloning this repository. Instead one have to upload the image folder to <a href="https://drive.google.com/">Google Drive</a> and link the folder with the cell containing

```python
from google.colab import drive
drive.mount('/content/drive/')
sys.path.insert(0,'/content/drive/MyDrive/INSERT_DIRECTORY_HERE') # Insert folder name here
drive_path= "drive/MyDrive/project/" # Insert folder name here
```
## Multitask Learning Model
The multitask learning model with connected output layers can be found in the notebook <a href="https://github.com/AntonRydahl/multitask_learning/blob/main/Final_Network_No_Connection.ipynb">Final_Network_No_Connection.ipynb</a>. The following figure illustrates how the two feed forward neural networks have been connected.
<p align="center"><img src="https://github.com/AntonRydahl/multitask_learning/blob/main/figures/combined_classifier.png" alt="drawing" width="500"/></p>

## Multitask Learning Model with Connected Output Layers
The multitask learning model build on top of the pretrained ResNet-18 can be found in the notebook <a href="https://github.com/AntonRydahl/multitask_learning/blob/main/Final_Network_Connection.ipynb">Final_Network_Connection.ipynb</a>. The network is illustrated by the following figure.
<p align="center"><img src="https://github.com/AntonRydahl/multitask_learning/blob/main/figures/final_classifier.png" alt="drawing" width="500"/></p>

## Single Task Classification Models
In order to compare the quality of the multitask models we also developed two regular deep neural networks for classification of diagnosis and chraracteristics (symptoms) respectively. They can be found in the folder <a href="https://github.com/AntonRydahl/multitask_learning/tree/main/singletask_models">singletask_models</a>.

## Note on Data
The images and data sets for this project are private and you will therefore not be able to run the notebooks. 