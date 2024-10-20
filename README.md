# Natural Disaster Prediction with Machine Learning (Ongoing)

**Mentor:** Purnendu Karmakar  
**Team Size:** 3  

## Overview
This project aims to build machine learning models capable of predicting various natural disasters using classification algorithms. The models have achieved over 85% accuracy in predictions. The project involves in-depth data analysis and feature extraction to enhance the performance of the models.

## Key Skills
- **Python**: Used for developing machine learning models and data manipulation.
- **Data Classification**: Implemented classification algorithms for natural disaster prediction.
- **Feature Extraction**: Extracted key features from datasets to optimize model performance.
- **CNN (Convolutional Neural Networks)**: Used for advanced pattern recognition and prediction in natural disaster data.

## Setup Instructions

### 1. Clone the Repository
First, clone the repository from GitHub.

```bash
git clone https://github.com/Bhakti-Jain/BTP-Project.git
cd BTP_Project
```

### 2. Install Dependencies
Make sure you have Python 3.8+ installed. The project uses a virtual environment in the imageclassification/ folder, activate it and install the required dependencies manually.
Activate the virtual environment:

- For Windows (Command Prompt):
```bash
imageclassification\Scripts\activate.bat
```
- For Windows (PowerShell):
```bash
imageclassification\Scripts\Activate.ps1
```
- For Linux/Mac:
```bash
source imageclassification/Scripts/activate
```

### 3. Prepare the Data
Place your input images in the data/ directory. The data should follow the folder structure based on natural disaster types like earthquake, land slide, and wild_fire.
Example folder structure:

data/

├── earthquake/

│   ├── image1.jpg

│   └── image2.jpg

├── land slide/

│   ├── image1.jpg

│   └── image2.jpg

├── wild_fire/

│   ├── image1.jpg

│   └── image2.jpg

### 4. Running the Classifier
To classify new images, use the following command. Make sure to specify the correct path to the image you want to classify:
```bash
python Disaster_Classifier.keras --image <path_to_image>
```
This will output the predicted disaster type for the given image.

### 5. Training the Model (Optional)
If you wish to retrain the model using new data, ensure your new data is placed in the appropriate subdirectories within the data/ folder. You can run the training command as follows:
```bash
python Disaster_Classifier.keras --data_dir ./data/
```
This will retrain the model based on the images and their corresponding disaster types in the data/ directory.

### 6. Evaluating the Model
To evaluate the model on a validation dataset, run:
```bash
python Disaster_Classifier.keras --data_dir ./data/
```
This will print out accuracy and other metrics for the current model.

### Model files
Pretrained models are stored in the models/ directory, such as disasterclassifier.h5. The .keras files like Disaster_Classifier.keras and my_model.keras can be used for loading, training, or fine-tuning models.

## Achievements
- **Model Accuracy**: Achieved over 85% accuracy in predicting various natural disasters.
- **Data Handling**: Conducted thorough data analysis and feature extraction on datasets containing over 900 entries to optimize the performance of the models.

## Future Work
Further optimizations and extensions to the model are ongoing to improve accuracy and incorporate more disaster types.

---

This project is being continuously developed and enhanced as part of a collaborative effort with a team of three members.
