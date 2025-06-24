# Model Architecture

The model consists of several key components:

- TokenAndPositionEmbedding: Handles token and positional embeddings.
- TransformerBlock: A custom transformer block with multi-head attention.
- Causal_Attn_Mask: Implements causal masking to masked future tokens

### Running it in local machine
Installation

```
git clone https://github.com/Shegun93/Decoder-Transformer.git
cd Decoder-Transformer
pip install -r requirements.txt

```
### Running with docker
If you do not have GPU, run the below command
```
docker-compose up
```

if you want to run with GPU, run the below the command
```
docker compose -f docker-compose-gpu.yml up
```
### .env file
Before running the container, enusre you setup your .env file in the root directory

```
JUPYTER_PORT=8890
TENSORBOARD_PORT=6006
```
Jupyter lab should be available in your local browser on the prot you specifified in your env file

## Acknowledgements

- TensorFlow and Keras teams
