

## 🚦 Traffic Sign Recognition with Attention-Based CNNs

Hey! This is a deep learning project I worked on for my Advanced Image Processing course. The goal was to classify traffic signs using CNNs and improve accuracy by adding attention mechanisms.

I tested three different models:  
- A base CNN with **Simple Attention**  
- CNN with **Squeeze-and-Excitation (SE)** Attention  
- CNN with **CBAM (Convolutional Block Attention Module)**

All models were trained on the [GTSRB](https://benchmark.ini.rub.de/gtsrb_news.html) dataset which has 43 different types of German traffic signs.

---

### 🧠 What’s the idea?

CNNs are already pretty good at image classification, but sometimes they struggle to focus on the most important regions (like the actual sign, not the background). That’s where attention modules help — they guide the model to "look" at the right spots.

I used the same CNN structure for all models and just swapped the attention part to see which one works best.

---

### 📊 Quick Results

| Model         | Validation Accuracy | Test Accuracy | Mistakes |
|---------------|---------------------|---------------|----------|
| Simple        | 96.5%               | 95.8%         | 187      |
| SE Attention  | 96.8%               | 96.3%         | 162      |
| CBAM          | **97.2%**           | **96.7%**     | **144**  |

CBAM gave the best results overall — especially on tricky images like faded or tilted signs.



### 🙌 Thanks

Special thanks to Prof. Liu, Jingyu for teaching the Advanced Image Processing course and guiding us through the concepts of CNNs and attention mechanisms. This project was completed as part of the coursework under their supervision.

