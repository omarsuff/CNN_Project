# 🖼️ Automatic Image Captioning using CNN-RNN on Flickr8k Dataset

This project builds an end-to-end **image captioning system** that generates human-like descriptions for images using a deep learning pipeline. It combines **Convolutional Neural Networks (CNNs)** for visual feature extraction and **Recurrent Neural Networks (RNNs)** for natural language caption generation. An intermediate **image classification step** is used to enhance contextual relevance in the captions.

---

## 📁 Dataset

- **Name:** Flickr8k  
- **Description:** Contains 8,091 images with 5 human-written captions per image.  
- **Source:** [Flickr8k Dataset on Kaggle](https://www.kaggle.com/datasets/adityajn105/flickr8k)

| Split | Images | Captions | Purpose                  |
|-------|--------|----------|--------------------------|
| Train | 6,472  | 32,360   | Model training           |
| Val   | 810    | 4,050    | Validation/tuning        |
| Test  | 809    | 4,045    | Final evaluation/scoring |

---

## ⚙️ Preprocessing Steps

1. **Caption Cleaning & Tokenization**
2. **Vocabulary Construction**
3. **Sequence Preparation (input-output pairs)**
4. **Image Feature Extraction using CNN (e.g., VGG16/InceptionV3)**
5. **Train-Test Split**  
   - 60% Training, 20% Validation, 20% Testing  
   - Ensured captions correctly map to images

---

## 🧠 Model Architecture

- **CNN Encoder**: Extracts feature vectors from images (using pre-trained CNNs)
- **Embedding Layer**: Converts words to dense vectors
- **RNN Decoder**: Generates captions word-by-word using LSTM
- **Dense Layer**: Final output layer predicting next word in the sequence

---

## ✅ Features

- Image-to-sequence deep learning pipeline
- Clean and pre-tokenized captions
- Uses CNN for image understanding, RNN for language generation
- Evaluation on custom test split using BLEU scores and qualitative inspection

---

## 🚀 Future Work

- Switch to Transformer-based decoder for improved performance
- Integrate attention mechanisms
- Expand to larger datasets like MSCOCO

---

## 📌 Project Status

✅ Model Training Complete  
✅ Evaluation Performed  
🔄 Real-time Captioning (Future scope)  

---