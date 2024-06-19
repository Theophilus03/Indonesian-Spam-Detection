Indonesian Spam Detection Using Indo-BART and TF-IDF with SVM
Overview
This project focuses on detecting spam in Indonesian text using a combination of Indo-BART and TF-IDF with a Support Vector Machine (SVM). Indo-BART is used for generating features from the text, and TF-IDF is used for text vectorization. These features are then used to train an SVM classifier to distinguish between spam and non-spam messages.

Team Members
Elvano Jethro Mogi Pardede - 2502025403
Rasyad Muhammad Ramdhanazuri - 2501992305
Theophilus Nathan Tanudjaja - 2502007514
Wicakra Hanly Tanudjaja - 2502032964
Table of Contents
Installation
Usage
Data
Training
Evaluation
Contributing
License
Installation
To get started, clone this repository and install the required dependencies.

bash
Copy code
git clone https://github.com/yourusername/indonesian-spam-detection.git
cd indonesian-spam-detection
pip install -r requirements.txt
Usage
Preprocessing Data
Before training the model, you need to preprocess the data. Run the following script to clean and preprocess the text data:

bash
Copy code
python preprocess_data.py --input data/raw_data.csv --output data/cleaned_data.csv
Training the Model
To train the spam detection model using Indo-BART and TF-IDF with SVM, execute the following script:

bash
Copy code
python train_model.py --input data/cleaned_data.csv --model_output models/spam_detector.pkl
Predicting with the Model
Once the model is trained, you can use it to predict whether new texts are spam or not:

bash
Copy code
python predict.py --model models/spam_detector.pkl --input data/new_texts.csv --output results/predictions.csv
Data
The data used in this project should be in CSV format with at least two columns: text and label. The text column contains the message text, and the label column contains the corresponding labels (spam or non-spam).

Example of data format:

text	label
"Selamat! Anda menang!"	spam
"Apakah Anda sibuk?"	ham
Training
The training process involves the following steps:

Load Data: Load the cleaned text data.
Feature Extraction: Use Indo-BART for feature extraction and TF-IDF for text vectorization.
Model Training: Train an SVM classifier using the extracted features.
Save Model: Save the trained model to a file for later use.
Evaluation
Evaluate the model using standard metrics such as accuracy, precision, recall, and F1-score. Run the evaluation script as follows:

bash
Copy code
python evaluate_model.py --model models/spam_detector.pkl --test_data data/test_data.csv
Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

License
This project is licensed under the MIT License. See the LICENSE file for more details.

