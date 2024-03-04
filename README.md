# Toxic Word Classifier

This repository contains code for training and deploying two models to classify toxic words within sentences. The first model utilizes an BiLSTM-CRF architecture, while the second model is a fine-tuned transformer using the HuggingFace library. Both models operate at the token level, providing accurate detection of toxic language.

## Requirements

- Python 3.x
- PyTorch
- HuggingFace Transformers library (for transformer model)


## Usage

1. **Training:**
   - For the BiLSTM-CRF model, the code for training it is in the ```models/toxicity_token_classifier_BiLSTM_CRF.ipynb``` notebook.
   - For the Transfomer model, the code for training it is in the ```models/toxicity_token_classifier_Transformer.ipynb``` notebook. I have used [Microsoft's mpnet](https://huggingface.co/microsoft/mpnet-base) model as the pretrained model, and fine-tuned it for this specific task.

2. **Inference:**
   - You can use the BiLSTM-CRF model as it is explained in its training notebook.
   - You can use the Transfomer model by going to [my hub at HuggingFace.co](https://huggingface.co/Sinanmz/toxicity_token_classifier). Also, you can load it via the transformers library.