# CleanSweep.AI
A-EYE on SCATTERED GARBAGE! An AI & ML solution to solve some of the basic but most important problems in day to day life.  


Problem Statement:- Scattered scrap detection is a significant problem in many countries around the world. It can lead to a number of negative consequences, including environmental degradation, public health issues and decreased quality of life for residents.
Garbage can accumulate in public spaces, such as streets, parks, and beaches, due to individuals littering or improperly disposing of waste.
In some areas, waste collection systems may be inadequate or inefficient, leading to a build-up of garbage in certain areas.

Objective:- The goal is design an object classification model which segregates garbage and scattered scrap from the given input data from various sources like dashcams, CCTVs installed in roads etc.
The video is processed and the density of garbage is then calculated and the processed through a machine learning algorithm.
If garbage is detected is greater than a certain threshold, then the concerned authorities are intimated with help of an escalation algorithm.

Solution:- The solution to solve the above problem is implementing a Garbage Detection Model using the Single Shot Detector Algorithm whcih is trained on the TACO Dataset. 

System Workflow:-
![Flowchart](https://user-images.githubusercontent.com/80829447/208266806-8d21746e-7aa9-4147-8169-4d3ae4e526b1.png)


# Toolkits used : Intel® AI Analytics Toolkit (AI Kit) - oneDNN (Deep Neural Network Library) and Intel® Distribution of OpenVINO™ Toolkit

Cleansweep.AI uses the openVINO toolkit to optimize the processing of the object detection model to detect the scattared garbage  from the input video . The detected scrab density determines to which authority , the alert message should be sent. The Intel® AI Analytics Toolkit (AI Kit) helps in achieving better results by optimising the models with the help of oneAPI Deep Neural Network Library (oneDNN).
The toolkits have support for a number of pre-trained models such as MobileNetV1,which can achieve accurate and efficient effect in  CLeanSweepAI and help to improve the performance.


![image](https://user-images.githubusercontent.com/92366411/225904033-084ef650-47a9-43de-b0bc-f4fb038eac8d.png)

The Scrab Detection model is executed on the local system wherein an environment is created and Tensorflow is installed through the Intel channel. The AI Analytics Toolkit is used to install and optimize all the libraries which are present in the project.


Steps to run this project:  
STEP 1: Download the models and the weights from the drive link provided below.  
STEP 2: Clone the GitHub repository.  
STEP 3: Create a new Conda environment and install the required libraries present in the requirements.txt through the Intel channel.
STEP 4: Run the code provided below in the terminal of the project folder.

Install the requirements:
```
pip install -r requirements.txt
```

Run the app:
```
streamlit run app.py
```



Collaborators:  
Mani Kanta: https://github.com/Manikanta-7342  
Akhil: https://github.com/Akhil5347  
Shreyas: https://github.com/ShreyasKuntnal
Nishank:https://github.com/NishankKS

