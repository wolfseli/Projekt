# Slide Image Correction Project

## Project Goal / Motivation
Some time ago, I decided to digitize my family's tens of thousands of old slides. I bought a slide scanner, which can scan slides relatively quickly. The problem is that there are a lot of negative images and images with a red tint in the slides. Also, the slides are not all stored in the same direction. So they all have to be rotated correctly before scanning. Although the scanned images can be rotated directly on the scanner and the negatives can be reversed, this is tedious and takes a relatively long time. With thousands of images, it also takes a long time to correct the images on the computer afterwards. In addition, it would be relatively easy to automate the scanning process if the images did not have to be rotated or reversed during scanning.

## Problem
It would be ideal if the slides could be scanned automatically, without having to rotate the images or invert the colors. The aim is to develop a machine learning model that will automatically go through all the images after scanning, identify whether they are negative or rotated, and correct them. This could save a lot of time. To do this, the model must be trained on a large number of images containing as many different objects as possible. This allows the model to learn how different objects look rotated or correctly oriented, and with negative and non-negative colors and also with a red tint. 

## Solution
The goal is to create a machine learning model that processes scanned images, detects whether they are negative or incorrectly oriented, and then corrects them. This will significantly speed up the digitization process by eliminating the need for manual correction during or after scanning.

## How to use the Project
1. **Clone the repository from GitHub**:
   ```sh
   git clone https://github.com/wolfseli/Projekt

2. **Create a virtual environment:**:  
Use the requirements.txt file to set up your environment. 
The project was created with Python Version 3.10.11.

3. **Necessary images:**:  
All the necessary images are already in the raw and processed folders. If desired, the scraping process and image preparation can be redone using the notebooks "01_data_scraping" and "02_data_preparation".

4. **Retrain the model:**:  
If you want to train the model again, you can use the ‘03_model_training’ notbook.

5. **Training in Google Colab:**:  
The training of the model can also be done in Google Colab. Simply open the respective notebook in Colab. The images for training can be found in the following public folder on Google Drive: https://drive.google.com/drive/folders/1ONtDlwGJiek5IfhCGLCNv8n6g25XeNuO?usp=drive_link. Adjust the link in the notebook accordingly, and then you can execute it.
