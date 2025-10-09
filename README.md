# Sentiment Analysis for Hatred Speech Detection

A comprehensive deep learning project comparing different neural network architectures for sentiment analysis on Twitter data, focusing on detecting hateful vs non-hateful content and classifying sentiment polarity.

## 📋 Project Overview

This project implements and compares four different deep learning models for sentiment analysis:

- **BERT** (Bidirectional Encoder Representations from Transformers)
- **RNN** (Recurrent Neural Network)
- **LSTM** (Long Short-Term Memory)
- **Deep CNN** (Convolutional Neural Network)

The models classify tweets into three sentiment categories: **positive**, **negative**, and **neutral**.

## 🎯 Objectives

- Compare the performance of different deep learning architectures for sentiment analysis
- Implement robust text preprocessing pipeline for social media data
- Evaluate models on Twitter dataset with focus on hate speech detection
- Provide insights into model selection for different use cases

## 📊 Dataset

- **Source**: Twitter Sentiment Analysis Hatred Speech Dataset
- **Training samples**: 31,962 examples
- **Test samples**: 17,197 examples
- **Features**: Tweet ID, Tweet text, Label
- **Classes**: 3 sentiment categories (positive, negative, neutral)

## 🔧 Technologies Used

- **Python 3.x**
- **Deep Learning Frameworks**:
  - TensorFlow/Keras (for RNN, LSTM, CNN)
  - PyTorch (for BERT)
  - Transformers (Hugging Face)
- **Data Processing**:
  - pandas, numpy
  - NLTK (tokenization, lemmatization)
  - scikit-learn (preprocessing, metrics)
- **Text Processing**:
  - contractions (contraction expansion)
  - emoji (emoji handling)
  - vaderSentiment (sentiment labeling)

## 🚀 Getting Started

### Prerequisites

```bash
pip install torch tensorflow transformers
pip install pandas numpy matplotlib scikit-learn
pip install nltk emoji contractions vaderSentiment
pip install kagglehub tqdm
```

### Installation

1. Clone the repository:

```bash
git clone https://github.com/maybeitsai/sentiment-analysis-hatred-speech.git
cd sentiment-analysis-hatred-speech
```

2. Install required packages:

```bash
pip install -r requirements.txt
```

3. Run the Jupyter notebook:

```bash
jupyter notebook sentiment_analysis_hatred_speech.ipynb
```

## 📁 Project Structure

```
sentiment-analysis-hatred-speech/
│
├── sentiment_analysis_hatred_speech.ipynb  # Main notebook with complete analysis
├── README.md                               # Project documentation
└── requirements.txt                        # Python dependencies
```

## 🔄 Methodology

### 1. Data Understanding

- Exploratory data analysis of tweet characteristics
- Class distribution analysis
- Text length and token analysis

### 2. Data Preparation

- **Text Cleaning**: Remove URLs, mentions, hashtags, special characters
- **Contraction Expansion**: Convert contractions to full forms
- **Emoji Processing**: Convert emojis to text descriptions
- **Slang Normalization**: Standardize informal language
- **Lemmatization**: Reduce words to base forms
- **Stopword Removal**: Remove non-informative words

### 3. Data Labeling

- Use VADER sentiment analyzer for automatic sentiment labeling
- Balance dataset with 6,000 samples per sentiment class

### 4. Model Implementation

- **Traditional Models**: RNN, LSTM, Deep CNN with embedding layers
- **Transformer Model**: Fine-tuned BERT for sequence classification
- **Evaluation**: Accuracy, Precision, Recall, F1-score

## 📈 Results

| Model        | Architecture  | Key Strengths                                    |
| ------------ | ------------- | ------------------------------------------------ |
| **BERT**     | Transformer   | Highest accuracy, contextual understanding       |
| **LSTM**     | Recurrent     | Good sequential processing, handles dependencies |
| **Deep CNN** | Convolutional | Fast inference, captures local patterns          |
| **RNN**      | Recurrent     | Baseline performance, simple architecture        |

_Detailed results and performance metrics are available in the notebook._

## 🎯 Use Cases

- **Content Moderation**: Automatically detect and flag hateful content
- **Social Media Monitoring**: Track sentiment trends in real-time
- **Brand Analysis**: Monitor public sentiment about products/services
- **Research**: Academic studies on online behavior and sentiment

## 🔮 Future Enhancements

- [ ] Implement ensemble methods combining multiple models
- [ ] Add attention mechanisms to RNN/LSTM models
- [ ] Deploy best model as REST API service
- [ ] Extend to multilingual sentiment analysis
- [ ] Real-time streaming analysis integration

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📧 Contact

**Project Maintainer**: Bu Lina  
**Repository**: [sentiment-analysis-hatred-speech](https://github.com/maybeitsai/sentiment-analysis-hatred-speech)

---

⭐ If you found this project helpful, please give it a star!
