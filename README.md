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

* Built a Convolutional Neural Network model using EfficientNetB0 to predict different skin conditions using a diverse set of images and data.
* Achieved an F1 score of 0.14490 and a ranking of 53/74 on the final Kaggle Leaderboard
* Used SHAP to interpret model decisions which helped us understand the importance of feature selection and model predictions
* Implemented Data augmentation and class weighting to optimize results within compute constraints

🔗 [Equitable AI for Dermatology | Kaggle Competition Page](https://www.kaggle.com/competitions/bttai-ajl-2025/overview)

---

## **👩🏽‍💻 Setup & Execution**

* To clone the repository, you need to execute the command: git clone https://github.com/anikaguin/mandelic-acid.git
* Install dependencies using the terminal. Tere are a list of imports in the first cell. 
* Create a virtual environment to install any dependencies. You can use: python -m venv venv
* The datasets are available in the github repository. You can move it to any folder. 
* You can run the script by typing python <filenmae>.py

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

---

## **🧠 Model Development**

**Describe (as applicable):**

* We used Convolutional Neural Network model with transfer learning based on EfficientNetB0 architecture. This allows us to yous weights determined by pre-trained models that have been trained in a larger dataset. We chose EfficientNetB0 because it works well with images and our data consisted largely on images of skin diseases. We used global Average Pooling to reduce the dimesnions and used dense layers with ReLU to add non-linearity. Then we used a final dense layer to classify the images with the labels of the skin diesease. 
* We used EfficientNetB0 as a base layer. Thus the pretrained model already learned useful features from a larget dataset. We chose the batch size to be 32 which is common practice. We also initially had a learning rate of 0.0005 and we reduced it as a part of the fine tuning process. To prevent overfitting, we added dropout layers.
* We split thet data up so that 80% was in training and 20% was in tetsing. For the training data, we used ImageDataGenerator to rescale the images. The evaluation metics was accuracy. We also used the F1 score to evaluate accuracy. The performance was not too accurate but we were able to increase the score through data fine tuning. 

---

## **📈 Results & Key Findings**

**Describe (as applicable):**

* Our model did not perform too well. The accuracy was low but we were able to get it slightly higher than the initiial score due to hyperparameter fine tuning. 
* We were ranked 53/74 teams
* Our score was 0.14490

---

## **🖼️ Impact Narrative**
1. What steps did you take to address [model fairness](https://haas.berkeley.edu/wp-content/uploads/What-is-fairness_-EGAL2.pdf)? (e.g., leveraging data augmentation techniques to account for training dataset imbalances; using a validation set to assess model performance across different skin tones)
* Data augmentation techniques were applied to the images to address fairness. We rescaled the images to make our data more diverse. A validation set was also used to ensure that the model is predicting properly.
3. What broader impact could your work have?
* The borader impact of this work is to use machine learning to reduce bias in predictions. This ensures fairness in areas such as the medical field. This also helps in accessibility and inclusivity. It is also an ethical way to use AI and machine learning. 

---

## **🚀 Next Steps & Future Improvements**

**Address the following:**

* Some limitations include limited image resolutionn. We could have resize the images to make them bigger so that they could capture more details. We could have also done more data augmentation to reduce the chances of overfitting.
* With more time and resources, we would have tried alternate models to predict the skin conditions. We would have hypertuned the models and compared the different model results. 
* We should have had higher resolution images to see if it would have any impact on the model. We could have also increased the size of the dataset to see if it will make the model more accurate. 

---




