# Model Architecture

The model consists of several key components:

- **TokenAndPositionEmbedding**: Handles token and positional embeddings.
- **TransformerBlock**: Custom Transformer block with multi-head attention.
- **Causal_Attn_Mask**: Implements causal masking for auto-regressive generation.

## Hyperparameters

- **Maximum Sequence Length**: 80 tokens
- **Vocabulary Size**: 10,000
- **Embedding Dimension**: 256
- **Number of Attention Heads**: 2
- **Key Dimension**: 256
- **Feed Forward Dimension**: 256

## Dataset

- **Source**: Wine Magazine Dataset (130k reviews)
  
### Preprocessing:
- Lowercased
- Punctuation handling
- Tokenization

## Training

- **Optimizer**: Adam
- **Loss Function**: Sparse Categorical Crossentropy

### Callbacks:
- Model Checkpointing
- Early Stopping
- TensorBoard Logging
### How to Run the Code
- if you don't have GPU, run the below command

###docker-compose up
## Usage

1. Prepare your dataset
2. Configure hyperparameters
3. Train the model
4. Generate wine descriptions

## Potential Improvements

- Increase model complexity
- Experiment with different hyperparameters
- Implement more sophisticated text generation techniques

## Limitations

- Generated descriptions may not always be coherent.
- Quality depends on training data and model complexity.

## Acknowledgements

- TensorFlow and Keras teams
- Wine Magazine for the dataset
