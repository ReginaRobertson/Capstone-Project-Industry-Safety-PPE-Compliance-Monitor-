PPE COMPLIANCE MONITORING USING MOBILENETV2 TRANSFER LEARNING

Project Overview

This PPE Compliance Monitoring System is a computer vision application developed to automatically determine whether a construction worker is wearing a safety helmet. The system uses Convolutional Neural Networks (CNNs) and transfer learning with MobileNetV2 to classify images as either Compliant (Helmet) or Non-Compliant (No Helmet).

Problem Statement

The construction and mining industries experience frequent workplace accidents and injuries due to workers failing to wear required Personal Protective Equipment (PPE), particularly safety helmets. Current monitoring methods rely heavily on manual inspections conducted by safety officers, which are time-consuming, inconsistent, and unable to provide continuous surveillance across large worksites. As a result, PPE violations may go undetected, increasing the risk of accidents and injuries. Therefore, there is a need for an automated, accurate and real-time system that can identify whether workers are complying with helmet safety requirements. This project addresses this problem by developing a computer vision-based PPE Compliance Monitoring System that automatically classifies workers as compliant or non-compliant using image data and deep learning techniques.

Objectives
1.	To develop a binary image classification model for helmet compliance detection.
2.	To compare a CNN trained from scratch with a transfer learning approach.
3.	To deploy the best-performing model in a user-friendly interface.
4.	To evaluate model performance using standard classification metrics.

   
Table 1: Main Results
Model	Test Accuracy

CNN from Scratch	90.3%

Improved CNN	92.5%

MobileNetV2 Transfer Learning	98.5%

Source: Authors’ construct based on data from Kaggle

From table 1 above, the MobileNetV2 significantly outperforms both CNN variants, achieving 98.5% test accuracy of 8.2% higher than the baseline CNN (90.3%) and 6.0% higher than the improved CNN with oversampling (91.8%). For this PPE helmet detection project, transfer learning with MobileNetV2 is the clear choice over building a CNN from scratch.


User Interface Overview
The PPE Compliance Monitor was deployed using Streamlit to provide a simple and user-friendly interface for safety officers and site managers. The application consists of a navigation panel on the left side with sections including Home, Prediction, History and About. The home page provides an overview of the system, its purpose and key features, while also displaying model statistics such as the achieved accuracy of 98.5% and the MobileNetV2 architecture used.
The prediction page allows users to upload an image of a worker for analysis. Once an image is uploaded, the system processes it using the trained MobileNetV2 model and displays a compliance verdict along with a confidence score. The history page stores previous predictions for review, while the about page provides information about the project and its objectives.

Running the Application
1.	Install project dependencies. 
2.	Launch the Streamlit application. 
3.	Navigate to the Prediction page. 
4.	Upload an image of a worker. 
5.	The model analyzes the image and returns a compliance prediction with a confidence score. 
6.	View previous predictions in the History section if required. 
Example Output
•	COMPLIANT – Helmet Detected (98.5% Confidence) 
•	NON-COMPLIANT – Helmet Not Detected (96.2% Confidence) 
This section ties nicely to the screenshot of your interface and demonstrates that the deployment requirement of the project was successfully completed.

 <img width="1035" height="509" alt="image" src="https://github.com/user-attachments/assets/9b131e2c-0f07-4f3f-8956-82b7633fc422" />

