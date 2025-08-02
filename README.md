# Human Activity Recognition Using MPU6050 Sensor Data



This project implements a human activity recognition (HAR) system using data collected from the MPU6050 sensor. The sensor provides six features: three-axis accelerometer (`ax`, `ay`, `az`) and three-axis gyroscope (`gx`, `gy`, `gz`). The system uses a Random Forest classifier to identify human activities based on the sensor inputs.



## Overview



- Preprocesses raw sensor data including label encoding and normalization.

- Trains a supervised machine learning model using the Random Forest algorithm.

- Evaluates model performance on a held-out test set.

- Supports real-time activity prediction based on new sensor input.



## Dataset



The dataset should be in CSV format (`mpu6050\_dataset.csv`) and contain the following columns:

- Features: `ax`, `ay`, `az`, `gx`, `gy`, `gz`

- Target: `label` (categorical activity name)



## Installation and Usage



1. Clone the repository:

git clone https://github.com/musharafhussainabid/har-mpu6050.git

cd har-mpu6050

Ensure that the dataset file mpu6050_dataset.csv is placed in the root directory.



Install required Python packages:




pip install -r requirements.txt

Run the activity recognition script:





python activity\_recognition.py

Input Example



test_data = np.array([

[-0.163107, -0.092484, 10.443980, 2.824668, 1.910485, -4.037339]

])

Output Example



Accuracy: 0.95

Predicted Activity: Walking

(Note: Actual results may vary depending on the dataset.)



Technologies

Python 3



NumPy



Pandas



scikit-learn (Random Forest Classifier, preprocessing, metrics)



File Structure



har-mpu6050/

│

├── activity_recognition.ipynb     

├── requirements.txt            # Python dependencies

└── README.md                   # Project documentation

License

This project is licensed under the MIT License. See the LICENSE file for more details.



Credits

MPU6050 sensor dataset

scikit-learn library


