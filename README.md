# 🧥 Fashion Recommendation System Using CLIP

This project builds a multimodal fashion recommendation system that suggests visually and semantically similar fashion items based on an input image and text description. It uses OpenAI's CLIP model (via Hugging Face) and the [Fashion Product Images Dataset](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset) from Kaggle.

## 🔍 Features

- Query with an image and a text prompt (e.g., *"red summer dress"*)
- Recommends visually and semantically similar items
- Powered by CLIP (Contrastive Language-Image Pretraining)
- Cosine similarity-based ranking
- Works with the first 1000 fashion items for demonstration

## 📁 Dataset

**Fashion Product Images Dataset**  
Kaggle Link: [https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset)

To use the dataset:
1. Download it manually or via Kaggle CLI:
   ```bash
   kaggle datasets download -d paramaggarwal/fashion-product-images-dataset
   unzip fashion-product-images-dataset.zip -d fashion_dataset

## 🧠 Model
Model: openai/clip-vit-base-patch32

Framework: Hugging Face Transformers

Language: Python (PyTorch)


## 🚀 How It Works
- Load and preprocess images and metadata

- Extract CLIP image embeddings from dataset

- Take a query image + text prompt

- Generate a multimodal embedding (image + text)

- Rank all dataset images using cosine similarity

- Display top-N visually/textually similar recommendations

## 🖼 Example
Query: a watch image

Prompt: "red summer dress"

Results: top 5 visually/textually similar recommended watch 

### Built with 💡 by Tasnia Sultana 
