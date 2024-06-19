"""
# Indonesian Spam Detection Using Indo-BART and TF-IDF with SVM

## Overview

This project focuses on detecting spam in Indonesian text using a combination of Indo-BART and TF-IDF with a Support Vector Machine (SVM). Indo-BART is used for generating features from the text, and TF-IDF is used for text vectorization. These features are then used to train an SVM classifier to distinguish between spam and non-spam messages.

Additionally, a word cloud is used to identify and remove extra abbreviations and Indonesian stopwords to improve the model's accuracy.

## Team Members

- Elvano Jethro Mogi Pardede - 2502025403
- Rasyad Muhammad Ramdhanazuri - 2501992305
- Theophilus Nathan Tanudjaja - 2502007514
- Wicakra Hanly Tanudjaja - 2502032964

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Training](#training)
- [Evaluation](#evaluation)
- [Contributing](#contributing)
- [License](#license)

## Installation

To get started, clone this repository and install the required dependencies.

```bash
git clone https://github.com/yourusername/indonesian-spam-detection.git
cd indonesian-spam-detection
pip install -r requirements.txt
