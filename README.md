# E-mail / SMS spam Classifier
This repository contains an NLP-based Email Spam Classifier that detects whether an email or sms is spam or not spam. The project includes data cleaning, exploratory data analysis (EDA), model building, model enhancement, prediction, and deployment to a server.

Live web app - [click here](https://email-sms-spam-classifier-11.onrender.com/)

# Table of Contents
- Project Overview
- Technologies Used
- Setup and Installation
- Dataset
- Exploratory Data Analysis (EDA)
- Model Building
- Model Evaluation
- Deployment
- Usage
- Contributing
- License

# Project Overview
This project aims to classify emails as either spam or ham (not spam) using Natural Language Processing (NLP) techniques. The model is trained on a dataset of labeled emails, and deployed as a web app on [render](https://email-sms-spam-classifier-11.onrender.com/) for real-time classification.

# Technologies Used
- Python 3.9
- NLTK for text preprocessing
- Scikit-learn for model building
- Streamlit for deployment
- Gunicorn as the server gateway

# Setup and Installation
- Clone the repository:
git clone https://github.com/your-username/email-spam-classifier.git
cd email-spam-classifier

- Create a virtual environment and install dependencies:
python -m venv myenv
source myenv/bin/activate  # On Windows, use `myenv\Scripts\activate`
pip install -r requirements.txt

- Run the Streamlit app:
streamlit run app.py

# Dataset
The dataset used consists of labeled emails with spam and ham tags. Basic cleaning steps like removing stop words, punctuation, and stemming were applied.

# Exploratory Data Analysis (EDA)
- Visualizations and insights were drawn from the data to understand patterns of spam emails.
- There is imbalance between spam and ham data counts
- Word clouds, frequency distributions, and length of emails were analyzed.

# Model Building
The following models were evaluated:
Gaussian naive bayes
Multinomial naive bayes
bernouli naive bayes
Random Forest Classifier

Bag of words & TfidfVectorizer was used to transform text data into feature vectors.

# Model Evaluation
- Accuracy, precision, recall, and F1-score were calculated to evaluate the models.
- Applied scaling and voting classifier to know the best performing model
- The best-performing model was random forest classifier with Tfidf vectorizer(accuracy 97% and precission 1)

 # Deployment
The project is deployed using:
- Streamlit for building the web interface.
- Gunicorn as the server gateway.

# Usage
To classify an email:
- Input the email text into the web app.
- The app will return whether the email is spam or Not spam.

- # Feel free to submit issues and pull requests. For major changes, please open an issue first to discuss what you would like to change.

# License
This project is licensed under the MIT License.
