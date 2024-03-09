
# Overview
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

In this project, we will be using the BirdClef 2022 dataset, which contains metadata for audio recordings. The are two major steps in this paper, first to prepare the data for CNN models using different audio pre-processing techniques. The second step is to train state-of-the-art pre-trained CNN models to classify our obtained dataset. Transfer learning involves using pre-trained Convolutional Neural Networks (CNNs) on one task and adapting them to perform well on another task. This approach conserves resources, as the model can be partially reused, with options ranging from completely retraining the network to retraining only specific components of it that are related to classification. The following are the key aspects of our contribution:

• Utilization of pre-trained Convolutional Neural Networks (CNNs) for sound classification through transfer learning.
• Implementation of techniques for sound representation and feature extraction to input sound descriptions into the retrained CNNs.
• Assessment of the effectiveness of transfer learning on selected CNNs in terms of classification accuracy metric

# Dataset
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Data : https://www.kaggle.com/c/birdclef-2022/data

The training dataset is sourced from the Xeno-canto community and included over 14,800 recordings spanning 152 different bird species. Many of these bird species are found in isolated, hard-to-reach high-elevation habitats, making physical monitoring difficult. Therefore, scientists have turned to using sound recordings to study them. As shown in Figure 1, these bird species exhibit a long-tailed distribution, which makes it challenging to deal with the extreme class imbalance. The goal of this competition is to develop machine learning models that can identify bird species based on their sounds, while addressing real-world challenges such as long-tailed rare birds and weak-noisy labels. The Kaggle competition provides all necessary data. It consists of 39.28 GB worth of 62.9k Ogg Vorbis audio files. The data includes:

• 10-minute long soundscape audio files in the Ogg format, separated into train and test sets.
• Short audio files featuring individual bird calls sourced from xeno-canto.org.
• Metadata in the form of a CSV file for the short audio files, which includes the primary bird species code, recording provider, location (latitude and longitude), date, and associated audio file name.

# Steps
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

   #1- EDA: Exploratory Data Analysis

Bird sounds distribution: Distribution of bird species in the training dataset:
![image](https://github.com/ali-dakhlaoui/Bird-sound-classification/assets/96072199/6a91ca9f-bc88-4ed2-81a2-6da3cfead317)



Attributes in the metadata CSV file:
![image](https://github.com/ali-dakhlaoui/Bird-sound-classification/assets/96072199/ee88f91f-4ce1-4bcb-84bd-a14b8e96199a)




Audio Distribution of the bird sounds:
![image](https://github.com/ali-dakhlaoui/Bird-sound-classification/assets/96072199/78716293-306e-4b88-9dbe-422f711dd472)



