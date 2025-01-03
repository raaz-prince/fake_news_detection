# Fake News Detection using BERT

This project uses a pretrained BERT transformer model for classifying news as fake or true. The model is trained on a dataset of fake and true news articles and can be used to predict the authenticity of news articles.

## Project Structure

- `Fake.csv`: Contains fake news articles.
- `True.csv`: Contains true news articles.
- `fake_news_model_state_dict.pth`: Contains the state dictionary of the trained model.
- `fake_news_model.pth`: Contains the entire trained model.
- `fakeNewsDetection.ipynb`: Jupyter notebook for training the model.
- `modelEval.ipynb`: Jupyter notebook for evaluating the model.

## Installation

1. Clone the repository:

2. Install the required packages by using command:
   ```sh
      pip install -r requirements.txt
   ```

## Training the Model

1. Open the [fakeNewsDetection.ipynb](http://_vscodecontentref_/6) notebook.
2. Run all the cells to train the model. The notebook will:
   - Load the fake and true news datasets.
   - Preprocess the data and create a custom dataset class.
   - Split the data into training and validation sets.
   - Load the BERT tokenizer and create dataloaders.
   - Define the BERT model for sequence classification.
   - Train the model and save the trained model and its state dictionary.

## Evaluating the Model

1. Open the [modelEval.ipynb](http://_vscodecontentref_/7) notebook.
2. Run all the cells to evaluate the model. The notebook will:
   - Load the BERT tokenizer and the trained model.
   - Define a function to predict the authenticity of news articles.
   - Use the function to predict the authenticity of user-input news articles.

## Usage

To predict the authenticity of a news article, run the [modelEval.ipynb](http://_vscodecontentref_/8) notebook and enter the news article when prompted. The model will output whether the news is ~"true" or "fake".
