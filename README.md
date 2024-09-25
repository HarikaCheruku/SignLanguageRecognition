Sign Language Recognition 
Overview
This project is a Sign Language Recognition that interprets hand gestures  into alphabets. It uses deep learning and computer vision to detect and recognize hand movements or signs, helping bridge the communication gap for individuals who are hearing or speech-impaired.

The project is built to recognize  American Sign Language (ASL)and can be expanded to support additional languages and gestures.

Features
Real-time recognition: The system captures and interprets signs in real-time using a webcam or video input.
High accuracy: Achieved through advanced deep learning techniques.
Customizable: Easily add new signs or modify the system to support different sign languages.
User-friendly interface: Simple and intuitive interface for ease of use.
Text/Speech Output: Converts recognized signs into text and optionally speech using text-to-speech integration.
Demo

Technologies Used
Python: Core programming language for development.
OpenCV: For capturing and processing video streams.
TensorFlow/Keras: Used to train and deploy the deep learning models.
Numpy, Pandas, Matplotlib: Data processing and visualization.
Project Structure
bash
Copy code
├── Sign Language                # Directory of the project            
│   ├── __pycache__/             # Cache directory
│   ├── .ipynb_checkpoints/      # Jupyter notebook checkpoints       
│   ├── .pytest_cache/           # Pytest cache  
│   ├── .venv/                   # Virtual environment directory
│   ├── .vscode/                 # VSCode configuration files
│   ├── myvenv/                  # Additional virtual environment directory
│   ├── SignImage48x48/          # Directory for sign language images (48x48 resolution)
│   ├── splitdataset48x48/       # Directory for split dataset (48x48 resolution)
│   ├── collectdata.py           # Script to collect sign language data
│   ├── split.py                 # Script to split dataset for training and testing
│   ├── realtimedetection.py     # Script for real-time detection of sign language
│   ├── requirements.txt         # Required Python packages and dependencies
│   ├── signlanguagedetectionmodel48x48.h5  # Pretrained model in H5 format
│   ├── signlanguagedetectionmodel48x48.json # Model architecture in JSON format
└── README.md                    # Project documentation (this file)
Installation
Prerequisites
Python 3.10.7
opencv-contrib-python
numpy
tensorflow
keras
split-folders
Steps
Clone the repository:
git clone https://github.com/HarikaCheruku/SignLanguageRecognition.git
cd sign-language-recognition
Install the required dependencies:
pip install -r requirements.txt
To collect data or to make own dataset
python src/collectdata.py
Split the dataset
python src/split.py
Train the model using google colab and download the trained model
train.ipynb
Download the dataset:
https://drive.google.com/drive/folders/1HuhBquOx49cVn9q2Z9d9DyLBNXSxFmU-?usp=sharing
Download the trained model
Start the real-time recognition system:
python src/realtimedetection.py
python app.py
Contributing
If you would like to contribute to the project, feel free to submit a pull request or open an issue. Please ensure you follow the contribution guidelines.
Future Improvements
Support for additional sign languages such as Indian Sign Language.
Enhance model accuracy and reduce latency.
Mobile app version for ease of use.
