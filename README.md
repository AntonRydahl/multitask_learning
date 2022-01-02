# Diagnosis Correction Using Domain Knowledge
In this project a multitask classification deep neural network has been trained to predict dermatological diagnoses and visible symptoms. The networks have been trained on the images in the folder <a href="https://github.com/multitask_learning/CSTR/blob/main/images/">images</a>.<br>
Note that this project has been carried out in <a href="https://colab.research.google.com/">Google Colab</a>. Thus the *.ipynb*-files cannot be run directly by cloning this repository. Instead one have to upload the image folder to <a href="https://drive.google.com/">Google Drive</a> and link the folder with the cell containing

```{python}
from google.colab import drive
drive.mount('/content/drive/')
sys.path.insert(0,'/content/drive/MyDrive/INSERT_DIRECTORY_HERE')# Insert folder name here
drive_path= "drive/MyDrive/project/" # Insert folder name here
```

<p align="center"><img src="https://github.com/AntonRydahl/multitask_learning/blob/main/figures/final_classifier.png" alt="drawing" width="500"/></p>

<p align="center"><img src="https://github.com/AntonRydahl/multitask_learning/blob/main/figures/combined_classifier.png" alt="drawing" width="500"/></p>