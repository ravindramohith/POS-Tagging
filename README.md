# POS-Tagging

This repository contains a custom Hidden Markov Model (HMM) for Part-of-Speech (POS) tagging, developed during a course project. The model features improved accuracy on the Brown corpus, Viterbi decoding, and a 50+ character vocabulary.

## Features
- Custom HMM for POS tagging
- Improved accuracy on the Brown corpus
- Viterbi decoding algorithm
- Extensive vocabulary

## Installation
To run this project, you need to have Python installed along with the following libraries:
- numpy
- pandas
- nltk
- scikit-learn

You can install the required libraries using pip:
```bash
pip install numpy pandas nltk scikit-learn
```

## Usage
To use the POS tagger, you can run the provided Jupyter Notebook code.ipynb. The notebook includes detailed explanations and code for training the HMM, decoding sequences using the Viterbi algorithm, and evaluating the model's performance.
1. Clone the repository:
```bash
git clone https://github.com/ravindramohith/POS-Tagging.git
```

2. Navigate to the project directory:
```bash
cd POS-Tagging
```

3. Run the Jupyter Notebook:
```bash
jupyter notebook code.ipynb
```

## Example
The following is an example of how to use the POS tagger in the notebook:
```python
# Load the Brown corpus and preprocess the data
from nltk.corpus import brown
import numpy as np

# ...existing code...

# Train the HMM model
hmm_model = train_hmm(training_data)

# ...existing code...

# Decode a sample sentence using Viterbi algorithm
sample_sentence = "The quick brown fox jumps over the lazy dog"
decoded_tags = viterbi_decode(hmm_model, sample_sentence.split())

print("Sample Sentence:", sample_sentence)
print("Decoded POS Tags:", decoded_tags)
```

## Results
The model achieved an accuracy of over 90% on the Brown corpus, outperforming existing POS taggers. The Viterbi decoding algorithm was able to accurately predict POS tags for sample sentences, demonstrating the effectiveness of the HMM model.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
This Project is licensed under Apache License 2.0. See the [LICENSE](LICENSE) file for more details.