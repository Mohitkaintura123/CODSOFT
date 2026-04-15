# LSTM Research Paper Text Generator

## Overview
This project implements a **Character-Level LSTM Language Model** trained on machine learning research papers to generate scientific-style text.

The system automatically collects **trending research papers**, downloads their PDFs from **arXiv**, extracts the text, and builds a dataset used to train the model. The trained LSTM can then generate **research-style paragraphs** similar to academic writing.

This project demonstrates the use of **deep learning for natural language generation using real research paper data**.

---

## Data Sources

The dataset used in this project was created automatically from publicly available research papers.

Data was collected from:

• Hugging Face Trending Papers  
https://huggingface.co/papers  

• arXiv Research Papers  
https://arxiv.org  

The Hugging Face trending page provides links to recent research papers, which are then downloaded as PDFs from arXiv.

The text is extracted from these PDFs and combined into a dataset file.

---

## Dataset

The dataset was built using approximately **50 research papers** downloaded from arXiv.

After extracting text from the PDFs, the combined dataset is saved as:

paper.txt

Dataset statistics:

• ~27,000+ words  
• Research content from multiple machine learning papers  
• Cleaned text used for training the language model  

---

## Project Pipeline

Trending ML Papers (HuggingFace)
        ↓
arXiv Paper Links
        ↓
PDF Download
        ↓
Text Extraction
        ↓
Dataset Creation (paper.txt)
        ↓
Character-Level LSTM Training
        ↓
Scientific Text Generation
        ↓
Gradio Interface

---

## Model Architecture

The model is a **Character-Level LSTM network** implemented using TensorFlow/Keras.

Embedding Layer  
↓  
LSTM (256 units)  
↓  
Dropout  
↓  
LSTM (256 units)  
↓  
Dropout  
↓  
Dense Softmax Output Layer  

Training parameters:

• Sequence length: 100 characters  
• Step size: 3  
• Batch size: 256  
• Optimizer: Adam  
• Loss: Sparse Categorical Crossentropy  

Early stopping is used to prevent overfitting.

---

## Training

The model learns patterns in the dataset by predicting the **next character in a sequence**.

Training uses the dataset stored in:

paper.txt

Training is performed using **TensorFlow/Keras** and can be run on **Google Colab GPU**.

---

## Text Generation

After training, the model can generate text using a seed prompt.

Example prompt:

The machine learning model learns representations

Example generated output:

the model demonstrates improved performance in large scale
experiments while maintaining spatial consistency across
dynamic environments.

Temperature parameter controls creativity:

0.2 → Conservative output  
0.5 → Balanced output  
0.8 → Creative output  
1.0 → Highly creative output  

---

## Interactive Interface

The project includes a **Gradio interface** that allows users to generate research-style text interactively.

Users can:

• Enter a prompt  
• Adjust temperature  
• Select output length  
• Generate text instantly  

---

## Technologies Used

Python  
TensorFlow / Keras  
NumPy  
PyPDF  
Requests  
Matplotlib  
Gradio  

---

## Future Improvements

• Train on larger datasets (100k+ words)  
• Use word-level language models  
• Experiment with Transformer models  
• Improve dataset cleaning  
• Deploy as a web application  

---

## Author Mohit kaintura 

Machine Learning Project  
LSTM-based Scientific Text Generator
