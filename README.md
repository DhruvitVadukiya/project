# Shakespeare Text Generator with LSTM

## Project Description
This project uses a Recurrent Neural Network (RNN) with Long Short-Term Memory (LSTM) layers to generate Shakespeare-style text. It is trained on public domain Shakespeare text from Project Gutenberg.

## Technologies Used
- Python
- TensorFlow (Keras)
- NumPy
- Google Colab

## Dataset
- Source: [Shakespeare by Project Gutenberg](https://www.gutenberg.org/files/100/100-0.txt)

## How It Works
1. Loads and cleans the text (lowercases, removes punctuation).
2. Tokenizes and generates word sequences.
3. Trains a 2-layer LSTM neural network.
4. Predicts the next word from a given seed phrase to generate text.

## Sample Outputs

*Seed: "the night is"*  
Generated: the night is his room of the room of the

*Seed: "love is a"*  
Generated: love is a man that will not speak

*Seed: "my heart is"*  
Generated: my heart is the king of the land of

## How to Run
1. Open the notebook in Google Colab.
2. Upload shakespeare.txt if needed.
3. Run all cells to train and generate text.
4. Use generate_text("your seed", num_words) to create new text.
5. Download the trained model using:
```python
model.save("shakespeare_lstm_model.h5")
from google.colab import files
files.download("shakespeare_lstm_model.h5")
