# 📰 Multimodal Fake News Detection (Text + Image)

This project implements a **multimodal fake news detection system** that combines **textual (BERT)** and **visual (ResNet)** features to classify news posts as **fake** or **real**.  
We use the **Weibo dataset** (Chinese social media) containing posts with both text and images.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alvira-Parveen/multimodal-fake-news-/blob/main/fake_news_multimodal.ipynb)

---

## 🚀 Features
- Uses **BERT (bert-base-chinese)** for text embeddings.  
- Uses **ResNet-50** for image embeddings.  
- Fusion of text + image features for final classification.  
- Achieves **~93% accuracy and F1-score** on validation data.  
- Trained and tested on **Google Colab (T4 GPU)**.  

---

## 📂 Dataset
- Source: **Weibo Fake News Dataset**  
- Structure after extraction:
weibo/
├── fake_news/
│ └── .../new.json
├── real_news/
│ └── .../new.json


- Each sample contains:
- `text_raw` or `text`: news text  
- `pic_infos`: image links  
- label: `0 = real`, `1 = fake`

---

## ⚙️ Installation
Clone repo and install dependencies:
```bash
git clone https://github.com/<your-username>/multimodal-fake-news.git
cd multimodal-fake-news
pip install -r requirements.txt

---


## 🖥️ Training

Run the Colab notebook:fake_news_multimodal.ipynb

Steps:-
1. Mount dataset (Weibo.zip) from Google Drive.
2. Extract text + image links.
3. Download images.
4. Train BERT + ResNet fusion model.
5. Evaluate on validation set.

---

## 📊 Results
| Metric   | Score |
| -------- | ----- |
| Accuracy | 93.1% |
| F1-Score | 93.0% |

- Balanced performance across both Fake and Real classes.
- Confusion matrix & classification report included in notebook.

---

##📌 Future Improvements
- Try Vision Transformers (ViT) instead of ResNet.
- Use multilingual BERT for broader datasets.
- Explore larger datasets (e.g., GossipCop, PolitiFact).
- Add data augmentation for better generalization.

---

##👩‍💻 Author

**Name**  : ALVIRA PARVEEN  
🔗 [LinkedIn](https://www.linkedin.com/in/alvira-parveen-78022536b)  
🌐 [GitHub](https://github.com/Alvira-Parveen)
