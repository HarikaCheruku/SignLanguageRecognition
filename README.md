<h1>Sign Language Recognition</h1>

<h2>Overview</h2>
<p>
    This project is a Sign Language Recognition System that interprets hand signs into the alphabet. It uses deep learning and computer vision to detect and recognize hand movements or signs, helping bridge the communication gap for individuals who are hearing or speech-impaired.
</p>
<p>
    The project is built to recognize American Sign Language (ASL) and can be expanded to support additional languages and gestures.
</p>

<h2>Features</h2>
<ul>
    <li><strong>Real-time recognition:</strong> The system captures and interprets signs in real-time using a webcam or video input.</li>
    <li><strong>High accuracy:</strong> Achieved through advanced deep learning techniques.</li>
    <li><strong>Customizable:</strong> Easily add new signs or modify the system to support different sign languages.</li>
    <li><strong>User-friendly interface:</strong> Simple and intuitive interface for ease of use.</li>
    <li><strong>Text/Speech Output:</strong> Converts recognized signs into text and optionally speech using text-to-speech integration.</li>
</ul>

<h2>Technologies Used</h2>
<ul>
    <li>Python: Core programming language for development.</li>
    <li>OpenCV: For capturing and processing video streams.</li>
    <li>TensorFlow/Keras: Used to train and deploy the deep learning models.</li>
    <li>Numpy, Pandas, Matplotlib: Data processing and visualization.</li>
</ul>

<h2>Project Structure</h2>

<h2>Project Structure</h2>

<pre>
Sign Language                  - Directory of the project
├── __pycache__/               - Cache directory
├── .ipynb_checkpoints/        - Jupyter notebook checkpoints
├── .pytest_cache/             - Pytest cache
├── .venv/                     - Virtual environment directory
├── .vscode/                   - VSCode configuration files
├── myvenv/                    - Additional virtual environment directory
├── SignImage48x48/           - Directory for sign language images (48x48 resolution)
├── splitdataset48x48/         - Directory for split dataset (48x48 resolution)
├── collectdata.py             - Script to collect sign language data
├── split.py                   - Script to split dataset for training and testing
├── realtimedetection.py       - Script for real-time detection of sign language
├── requirements.txt           - Required Python packages and dependencies
├── signlanguagedetectionmodel48x48.h5  - Pretrained model in H5 format
├── signlanguagedetectionmodel48x48.json - Model architecture in JSON format
└── README.md                  - Project documentation (this file)
</pre>


<h2>Installation</h2>
<h3>Prerequisites</h3>
<ul>
    <li>Python 3.10.7</li>
    <li>opencv-contrib-python</li>
    <li>numpy</li>
    <li>tensorflow</li>
    <li>keras</li>
    <li>split-folders</li>
</ul>

<h3>Steps</h3>
<ol>
    <li>Clone the repository:
        <pre><code>git clone https://github.com/HarikaCheruku/SignLanguageRecognition
cd sign-language-recognition</code></pre>
    </li>
    <li>Install the required dependencies:
        <pre><code>pip install -r requirements.txt</code></pre>
    </li>
    <li>Collect the data:
        <pre><code>python src/collectdata.py</code></pre>
    </li>
    <li>Split the dataset for training and testing:
        <pre><code>python src/split.py</code></pre>
    </li>
    <li>Train the model:
        <pre><code>train.ipynb</code></pre>
    </li>
    <li>Download the dataset: <a href="https://drive.google.com/drive/folders/1HuhBquOx49cVn9q2Z9d9DyLBNXSxFmU-?usp=sharing">Google Drive Link</a></li>
    <li>Start the real-time recognition system:
        <pre><code>python src/realtimedetection.py</code></pre>
    </li>
</ol>

<h2>Usage</h2>
<p>Once the system is running, ensure your webcam is connected or provide a video feed. The system will capture your gestures and output the recognized sign alphabet.</p>

<h2>Contributing</h2>
<p>If you would like to contribute to the project, feel free to submit a pull request or open an issue. Please ensure you follow the contribution guidelines.</p>

<h2>Future Improvements</h2>
<ul>
    <li>Support for additional sign languages (e.g., British Sign Language, Indian Sign Language).</li>
    <li>Enhance model accuracy and reduce latency.</li>
    <li>Mobile app version for ease of use.</li>
</ul>
