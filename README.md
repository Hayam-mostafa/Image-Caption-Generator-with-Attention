# Image-Caption-Generator-with-Attention


## Project Idea: 
This project demonstrates how to build an **Image Captioning** system that automatically generates a descriptive sentence for any given image.  
It combines **Computer Vision** and **Natural Language Processing (NLP)** by using a **VGG16 CNN** to extract visual features, then a sequence model (**LSTM**) generates the caption word by word, with an **Attention Layer** to improve focus on important parts of the image during caption generation.


## How It Works:

  1. **Image Features**  
     Each image is passed through a **pre-trained VGG16** network (trained on ImageNet) to extract deep visual features that represent the image content.
  
  2. **Text Sequences**  
     Captions are cleaned, tokenized, and converted into numerical sequences with consistent length for training.
  
  3. **Sequence Generator**  
     An **LSTM** network uses the image features along with the previously generated words to predict the next word in the caption.
  
  4. **Attention Layer**  
     At each step, the attention mechanism helps the model decide which parts of the image to focus on, improving caption accuracy.
  
  5. **Training & Inference**  
     The model is trained on the **Flickr8k** dataset, which contains thousands of images with multiple human-written captions.  
     After training, the system can generate new captions for unseen images.


## Tools & Libraries:

  - **Python** — development language
  - **TensorFlow / Keras** — deep learning framework for building and training the model
  - **numpy** — numerical operations
  - **nltk** — text cleaning and tokenization
  - **matplotlib** — for visualizing samples and training progress


## Dataset:

  - **Flickr8k** — includes 8,000 images, each with five human-written captions


## Project Goal:

The main goal of this project is to show how computer vision and NLP techniques can work together in a single deep learning pipeline.  
It demonstrates how pre-trained networks (**VGG16**), sequence generation (**LSTM**), and attention mechanisms can be combined to produce relevant, human-like image descriptions — a practical example of encoder-decoder architectures in modern AI.

