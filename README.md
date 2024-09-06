# Amazon Sentiment Analysis Using NLP and LSTM

This repository contains a sentiment analysis project that evaluates Amazon product reviews using Long Short-Term Memory (LSTM) networks. The project leverages Natural Language Processing (NLP) techniques to classify reviews into positive or negative sentiments and is deployed as a web application using Flask.

## Project Overview

The goal of this project is to analyze and classify the sentiment of Amazon product reviews using LSTM, a type of Recurrent Neural Network (RNN) designed to handle sequential data. The system processes text reviews to predict their sentiment, providing valuable insights into customer opinions and feedback.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Deployment](#deployment)
- [Results](#results)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Sentiment Classification:** Classifies Amazon reviews as positive or negative.
- **LSTM Model:** Utilizes an LSTM network for accurate sentiment prediction.
- **Web Interface:** Flask-based web application for user interaction.

## Technologies Used

- **Python:** Programming language used for development.
- **TensorFlow:** Framework used to build and train the LSTM model.
- **Flask:** Web framework used for deploying the application.
- **Pandas:** Data manipulation library for preprocessing data.
- **NumPy:** Library for numerical operations.
- **NLTK:** Natural Language Toolkit for text processing.

## Installation

To set up the project locally, follow these steps:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/akudnaver/amazon-sentiment-analysis.git
   cd amazon-sentiment-analysis
   ```

2. **Create and Activate a Virtual Environment:**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Prepare the Data:**
   - Download the dataset (Amazon reviews) and place it in the `data/` directory.

2. **Train the Model:**

   ```bash
   python train_model.py
   ```

3. **Run the Flask Application:**

   ```bash
   python app.py
   ```

4. **Access the Web Interface:**
   - Open a web browser and navigate to `http://localhost:5000` to use the sentiment analysis web app.

## Deployment

The web application can be deployed on a cloud platform like Heroku or AWS. Follow these steps for Heroku deployment:

1. **Create a `Procfile` in the root directory:**

   ```txt
   web: python app.py
   ```

2. **Commit Your Changes:**

   ```bash
   git add .
   git commit -m "Prepare for deployment"
   ```

3. **Push to Heroku:**

   ```bash
   heroku create
   git push heroku main
   ```

4. **Open Your Deployed Application:**

   ```bash
   heroku open
   ```

## Results

The LSTM model achieves an accuracy of X% on the test dataset, demonstrating its effectiveness in classifying sentiment from Amazon reviews. Detailed metrics and performance evaluations are available in the `results/` directory.

## Screenshots

Here are some screenshots of the web application:

- **Homepage:**
  ![Homepage Screenshot](screenshots/homepage.png)

- **Sentiment Analysis Result:**
  ![Result Screenshot](screenshots/result.png)

## Contributing

Contributions are welcome! If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Create a new Pull Request.

