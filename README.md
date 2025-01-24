# Sentiment Analysis on IMDB Reviews

This repository contains a project focused on performing **sentiment analysis** on the IMDB movie reviews dataset using **Bi-Directional LSTMs** implemented in Python with TensorFlow and Keras.

## Project Overview
Sentiment analysis is a key task in Natural Language Processing (NLP) to classify text as positive, negative, or neutral. This project uses Bi-Directional Long Short-Term Memory (LSTM) networks to effectively capture context from both past and future words, enabling accurate sentiment predictions.

### Key Features
- **Data Preprocessing**:
  - Tokenization, stopword removal, and lemmatization.
  - Conversion of text to sequences using one-hot encoding.
  - Sequence padding to ensure uniform input size for the LSTM model.

- **Model Architecture**:
  - Two Bi-Directional LSTM architectures were trained for comparison.
  - Early stopping to prevent overfitting.
  - Achieved an accuracy of **87.37%** on the validation set.

- **Tools & Technologies**:
  - TensorFlow and Keras for model building.
  - NumPy and Pandas for data preprocessing.
  - Matplotlib for visualizing results.

## Getting Started
### Prerequisites
Make sure you have Python 3.8 or later installed, along with the following libraries:

```bash
pip install tensorflow numpy pandas matplotlib
```

### Running the Notebook
1. Clone this repository:
   ```bash
   git clone https://github.com/naimish75/Sentiment-Analysis-on-IMDB-Reviews.git
   ```
2. Navigate to the folder:
   ```bash
   cd Sentiment-Analysis-on-IMDB-Reviews
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook IMDB_LSTM.ipynb
   ```
4. Run the cells to train and evaluate the model.

## Model Performance
- **Accuracy**: 87.37%
- **Loss**: Visualized through training and validation loss plots.

![Performance Graph](assets/images/imdb-lstm-performance.png)

## File Structure
- `IMDB_LSTM.ipynb`: Main notebook containing the implementation.
- `README.md`: Documentation for the project.
- `assets/images/`: Folder containing visualizations and results.

## Example Results
- **Input**: "The movie was absolutely fantastic, with great acting and a thrilling plot."
- **Output**: Positive

- **Input**: "Terrible film. Waste of time and money."
- **Output**: Negative

## Future Work
- Integrate additional features such as sentiment intensity scores.
- Experiment with pre-trained models like BERT for comparison.
- Deploy the model using a Flask or Streamlit app for real-time predictions.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author
Developed by [Naimish Sharma](https://github.com/naimish75).

Feel free to raise issues or contribute to this repository!
