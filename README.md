# Amazon Sentiment Analysis Project

## Overview

This project focuses on building a **Sentiment Analysis** model for Amazon product reviews using **Deep Learning** with **TensorFlow** and **Keras**. The solution classifies customer reviews into positive or negative sentiments, helping understand customer feedback for products. The project has been deployed using **Gradio**, which provides a user-friendly web interface that not only classifies the sentiment but also generates feedback percentages based on the reviews.

## Key Features

- **Deep Learning Model**: Built using TensorFlow and Keras for sentiment classification.
- **Data Processing**: Preprocessing of Amazon product reviews, including text cleaning, tokenization, padding, and embedding using techniques like Word Embedding (e.g., Word2Vec, GloVe).
- **Feedback Percentage Generator**: A feature that calculates the percentage of positive and negative feedback based on the reviews provided.
- **Gradio Interface**: A fully functional web interface for users to input their product reviews and see real-time sentiment classification results along with the feedback percentage breakdown.
  
## Project Structure

```bash
amazon-sentiment-analysis/
│
├── data/                       # Folder containing Amazon product reviews dataset
├── model/                      # Folder for saving model architecture and weights
├── notebooks/                  # Jupyter notebooks for exploratory data analysis and model training
├── app.py                      # Main Python script for deploying the Gradio interface
├── preprocess.py               # Script for data cleaning and text preprocessing
├── train.py                    # Script to train the TensorFlow Keras model
├── requirements.txt            # List of dependencies
├── README.md                   # Project documentation
└── saved_model/                # Folder for the saved trained model
```

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/amazon-sentiment-analysis.git
   cd amazon-sentiment-analysis
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset:
   - Download the Amazon product reviews dataset and place it inside the `data/` directory.
   
4. Train the model:
   - To train the sentiment analysis model, run the following command:
     ```bash
     python train.py
     ```

5. Run the Gradio interface:
   ```bash
   python app.py
   ```

6. Open the Gradio interface in your browser using the provided URL to start classifying reviews.

## Model Details

- **Architecture**: The sentiment analysis model uses a sequential neural network with LSTM layers to capture the context and sentiment from product reviews.
- **Embedding**: Word embeddings are used to convert text into dense vectors. GloVe embeddings are used for better semantic understanding of words.
- **Performance**: The model achieves good accuracy on the test data, showcasing its ability to predict positive or negative sentiments effectively.

## Gradio Interface

- The web interface allows users to input an Amazon product review and get real-time sentiment analysis.
- Along with the sentiment classification, the interface provides a feedback percentage generator, showing how many reviews are positive or negative.

## Example

1. **Input**: "This product is amazing! The quality is fantastic, and it arrived on time."
   - **Output**: "Positive"
   - **Feedback Percentage**: 90% Positive, 10% Negative

2. **Input**: "Terrible experience. The product broke down after one use."
   - **Output**: "Negative"
   - **Feedback Percentage**: 30% Positive, 70% Negative

## Future Improvements

- Adding more layers or experimenting with different architectures like BERT or GPT-based models.
- Including more classes for sentiment analysis (e.g., neutral or mixed sentiments).
- Expanding the dataset to improve the model's generalization capabilities.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

This project demonstrates the use of **Deep Learning** for text-based sentiment analysis and provides a clean, functional user interface for interacting with the model, making it a valuable tool for analyzing product feedback.
