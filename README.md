# Named Entity Recognition (NER) with LSTM

This repository contains an implementation of a Named Entity Recognition (NER) model using LSTM layers in TensorFlow. The project processes text data to classify tokens into entity categories, handling sequence labeling tasks efficiently.

## Features

- **Text Preprocessing**: Loads text and labels, tokenizes sentences, and builds vocabularies.
- **Custom Label Vectorization**: Transforms entity labels into vectors with padding handling.
- **LSTM Model**: Implements a custom LSTM-based model with embedding layers for sequence labeling.
- **Masked Loss and Accuracy**: Ignores padding values in loss and accuracy calculations.
- **Model Training and Testing**: Trains the NER model on labeled data and evaluates performance.

## Files

1. **`NER_LSTM_Implementation.ipynb`**: Python script implementing the NER model pipeline.
2. **Dataset Files**:
   - `train_sentences.txt` and `train_labels.txt`: Training data.
   - `val_sentences.txt` and `val_labels.txt`: Validation data.
   - `test_sentences.txt` and `test_labels.txt`: Test data.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AbdulrahmanAhmed20072/NER-LSTM-Model.git
   ```
2. Install the required Python packages:
   ```bash
   pip install numpy pandas tensorflow
   ```

## Usage

1. Load the training, validation, and test datasets.
2. Preprocess sentences and labels, vectorizing them for model input.
3. Train the LSTM-based NER model using the provided pipeline.
4. Use the trained model to predict entity tags for input sentences.

Run the script:
```bash
python NER_LSTM_Implementation.ipynb
```

## Outputs

- Trained NER model with saved weights (`weights.keras`).
- Predicted entity tags for test sentences.
- Evaluation metrics, including masked accuracy, to measure performance.

## Example

Input Sentence:
```
OpenAI and Google are great companies to work for in US.
```

Predicted Tags:
```
ORG ORG O O O O O LOC
```
