## 🎥 **Movie Genre Prediction**
This repository contains a Machine Learning-based web application that predicts the Genre of a Movie based on its Plot Summary. The project uses TF-IDF vectorization with Multinomial Naive Bayes for classification. It features a user-friendly interface built with Flask to allow users to input a movie plot and get real-time genre predictions.


## 📋 **Table of Contents**
- [Project Overview](#project-overview)
- [Tech Stack](#tech-stack)
- [How It Works](#how-it-works)
- [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Demo](#demo)
- [License](#license)


## 🏆 **Project Overview**
The Movie Genre Prediction project aims to classify movie plots into genres such as Thriller, Comedy, Drama, Action, Sci-Fi, and more. It is useful for:

- Content creators analyzing trends in movie genres.
- Film enthusiasts exploring new recommendations.
- Data science enthusiasts learning text classification.


## ⚙️ **Tech Stack**
- Frontend: HTML, CSS, Bootstrap
- Backend: Flask (Python)
- Machine Learning:
- Text Vectorization: CountVectorizer (TF-IDF and n-grams)
- Classifier: Multinomial Naive Bayes
- Visualization: Seaborn (confusion matrix)
- Dataset: Custom movie dataset with plot summaries and genres


## 🛠 How It Works
1. Data Preprocessing:
- Cleans the plot summaries by removing special characters and stopwords.
- Applies stemming to normalize the words.
2. Feature Extraction:
- Converts text data into numerical vectors using CountVectorizer with n-grams.
3. Classification:
- Trains a Naive Bayes classifier on the extracted features to predict genres.
4. Web Application:
- Users input a movie plot on the **`index.html`** page.
- Flask processes the input and predicts the genre using the trained model.
- Results are displayed on the **`result.html`** page.


## 🛠 Installation
1. Clone the repository:  
   ```bash
   git clone https://github.com/Saha-na16/Movie-Genre-Prediction.git  
   cd Movie-Genre-Prediction

2. Install dependencies:
   ```bash
   pip freeze > requirements.txt

3. Place your dataset in the project directory (kaggle_movie_train.csv).

4. Run the Flask application:
   ```bash
   python app.py
## 🚀 **Usage**
- Open your browser and navigate to **`http://127.0.0.1:5000`**.
- Enter a movie plot summary in the text area on the homepage.
- Click Predict to get the predicted genre on the results page.


## 📂 **Folder Structure**
1. movie-genre-prediction/
   ```plaintext
   movie-genre-prediction/
   ├── app.py                # Flask application  
   ├── model.pkl             # Trained Naive Bayes model  
   ├── cv.pkl                # Trained CountVectorizer  
   ├── templates/            # HTML files for Flask  
   │   ├── index.html        # Input page  
   │   └── result.html       # Output page  
   ├── static/               # Static assets (CSS, JS, images, etc.)  
   ├── dataset.csv           # Movie dataset (input)  
   ├── preprocess_and_train.py  # Model training and preprocessing script  
   └── README.md             # Project documentation 
## 🌟 Demo
Homepage **`(index.html)`**
Users enter a movie plot summary and click Predict.

Results Page **`(result.html)`**
The predicted genre is displayed.

## 📜 License
This project is licensed under the MIT License - see the [License](LICENSE) file for details.

