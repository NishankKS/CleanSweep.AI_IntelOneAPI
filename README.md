# CleanSweep.AI (powered by Intel oneAPI)
A-EYE on SCATTERED GARBAGE! An AI & ML solution to solve some of the basic but most important problems in day to day life.  


Problem Statement:- Scattered scrap detection is a significant problem in many countries around the world. It can lead to a number of negative consequences, including environmental degradation, public health issues and decreased quality of life for residents.
Garbage can accumulate in public spaces, such as streets, parks, and beaches, due to individuals littering or improperly disposing of waste.
In some areas, waste collection systems may be inadequate or inefficient, leading to a build-up of garbage in certain areas.

Objective:- The goal is design an object classification model which segregates garbage and scattered scrap from the given input data from various sources like dashcams, CCTVs installed in roads etc.
The video is processed and the density of garbage is then calculated and the processed through a machine learning algorithm.
If garbage is detected is greater than a certain threshold, then the concerned authorities are intimated with help of an escalation algorithm.

Solution:- The solution to solve the above problem is implementing a Garbage Detection Model using the Single Shot Detector Algorithm which is trained on the TACO Dataset.  

# Toolkits used : Intel® AI Analytics Toolkit (AI Kit) - oneDNN (Deep Neural Network Library) and Intel® Distribution of OpenVINO™ Toolkit

CleanSweep.AI uses the OpenVINO toolkit to optimize the processing of the object detection model to detect the scattared garbage  from the input video . The density of the detected scrap determines to which authority the alert message should be sent. The Intel® AI Analytics Toolkit (AI Kit) helps in achieving better results by optimising the models with the help of oneAPI Deep Neural Network Library (oneDNN).
The toolkits have support for a number of pre-trained models such as MobileNetV1,which can be used to achieve accurate and efficient results in  CleanSweepAI and help to improve the performance.


![image](https://user-images.githubusercontent.com/92366411/225904033-084ef650-47a9-43de-b0bc-f4fb038eac8d.png)

The Scrap Detection model is executed on the local system wherein an environment is created and Tensorflow is installed through the Intel channel. The AI Analytics Toolkit is used to install and optimize all the libraries which are present in the project.  

## Time Elapsed  


![base](https://user-images.githubusercontent.com/80829447/225950360-10c74071-f839-4135-828c-0f70bcd87f01.jpg)  
Time taken for the project to execute without oneAPI(base environment) : 1.59 seconds

![oneapi](https://user-images.githubusercontent.com/80829447/225950391-897195cb-0e69-47a7-aace-efd4452969f7.jpg)  
Time taken for the project to execute with oneAPI(oneapi environment) : 1.43 seconds  

Hence, we observe a difference of 0.16 seconds which is obtained with the help of oneAPI libraries.  

  
  

## System Workflow:-
![Flowchart](https://user-images.githubusercontent.com/80829447/208266806-8d21746e-7aa9-4147-8169-4d3ae4e526b1.png)


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


