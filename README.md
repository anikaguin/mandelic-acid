# mandelic-acid

---

### **👥 Team Members**

| Name | GitHub Handle | Contribution |
| ----- | ----- | ----- |
| Emily Prasad | @emilyp6 | Helped with increasing accuracy and contributed to team collaboration |
| Zoe Bailey | @zoebailey | Worked on model training and contributed to team collaborartion |
| Anika Guin | @anikaguin | Worked on github set up and readme and contributed to team collaboration |
| Sara Phondge | @sarap03 | Helped with implementing model and contributed to team collaborartion |

---

## **🎯 Project Highlights**

**Example:**

* Built a \[insert model type\] using \[techniques used\] to solve \[Kaggle competition task\]
* Achieved an F1 score of \[insert score\] and a ranking of \[insert ranking out of participating teams\] on the final Kaggle Leaderboard
* Used \[explainability tool\] to interpret model decisions
* Implemented \[data preprocessing method\] to optimize results within compute constraints

🔗 [Equitable AI for Dermatology | Kaggle Competition Page](https://www.kaggle.com/competitions/bttai-ajl-2025/overview)

---

## **🏗️ Project Overview**

**Describe:**

* The Algorithmic Justice League is an organization that helps combat social implications and the harms of artificial intelligence. Their mission is to make people aware of the impacts of AI and build the voice of the most imacted communities. AI has been a part in healthcare, but many challenges still persist in regards to accurate predictions and fair representation of communities. AI can perform poorer for people with dark skintones because of a lack of diverse datasets. The goal of this competition is to bridge that gap by using a divserse dataset to classify differennt skin conditions on different colored skins.  
* The objective of the challenge is to train a model that can classify 21 different skin conditions. We have been given datasets with numerous images that depict various skin conditions. These datasets have a diverse set of skintones to maintain a fair representation of skin conditions. Our goal is to develop a model that can accurately predict different skin conditions. Our model will be evaluated with a separate testing dataset and will be scored based on a weighted average F1 score metric. 
* This project will address a major problem with using AI in healthcare. Often times, a lack of fair representation in datasets create biased models. These models can result in inaccurate predictions for skin conditions in patients. Our goal is to bridge the gap by creating a model that can predict different skin conditions by using a diverse dataset. This is significant as it will reduce bias and make AI more reliable in healthcare. 

---

## **📊 Data Exploration**

In this project, we worked with a curated subset of the Fitzpatrick17k dataset provided through Kaggle, which contains approximately 4,500 labeled clinical images across 21 dermatological conditions. These images span a range of skin tones based on the Fitzpatrick Skin Tone (FST) scale, which is represented in two columns: fitzpatrick_scale (self-reported) and fitzpatrick_centaur (machine-annotated by Centaur Labs).

**🧠 Exploration & Preprocessing**

Our exploration focused on understanding the class distribution, skin tone representation, and data quality. Key steps included:
* Analyzing class imbalance across the 21 skin conditions
* Examining representation across different FST levels (1–6)
* Inspecting image quality and verifying metadata
* Identifying missing or anomalous values (e.g., FST scores of -1 or 0)

We visualized sample images per class and skin tone group to assess variability and potential bias. These insights informed our data preprocessing and augmentation strategy.


**Potential visualizations to include:**

* Plots, charts, heatmaps, feature visualizations, sample dataset images

---
