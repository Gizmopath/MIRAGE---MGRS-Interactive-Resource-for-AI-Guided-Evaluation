# MIRAGE---MGRS-Interactive-Resource-for-AI-Guided-Evaluation ![Oasi (1)](https://github.com/user-attachments/assets/0951ea44-7f5d-4d37-b78d-15239116ea6f)
A user-friendly application designed to assist clinicians in predicting the likelihood of Monoclonal Gammopathy of Renal Significance (MGRS) before performing a kidney biopsy. 

## Project Overview

This tool was developed as part of a retrospective multicentric cohort study conducted across three medical centers in Italy.
The dataset includes **438 renal biopsy cases** collected between 2018 and 2022, with 43% classified as MGRS based on biopsy results. The model was trained to differentiate between MGRS and non-MGRS cases using clinical variables such as age, serum creatinine, proteinuria, presence of M-spike, Bence-Jones protein, and free light chain (FLC) ratios.

## Key Features

- **ML-Based Classifier**: The model is built using the Extreme Gradient Boosting (XGBoost) algorithm, achieving an accuracy of **0.88** and an AUC-ROC of **0.90** on test data.
- **Predictive Flexibility**: The model can still make predictions even with missing data, making it highly useful for real-world clinical scenarios where complete datasets are not always available.
- **Desktop & Mobile Applications**: A user-friendly interface allows clinicians to easily input patient data and generate predictions. The tool is designed to run on both desktop and mobile devices.

## How to use MIRAGE on Android mobile devices
MIRAGE, as a mobile application, was designed for Android devices using Android Studio, with Kotlin as the programming language. Notably, the target API level for which the application is designed to run is 34 (Android version 14), while the minimum API it supports level is 24 (Android version 7.0); covering approximately 97.4% of Android devices. You can check the Android version of your Android device directly thought the device settings: Go to Settings > About phone (or About device) > Software > Find the Android version.

To install MIRAGE on Android mobile devices from an .APK file, follow these steps:
  1. Enable unknown sources on your mobile device: **Go to Settings** > **Secutity** > 
     **Install unkown app** > Enable permission for the app you are using to open the 
     .APK file
  2. Download the .APK file to your Android device
  3. Navigate to the folder where you saved the .APK file > Tap the .APK file >   
     **Install**

## How to use MIRAGE on your computer desktop 
MIRAGE, as a desktop application, is compatible with Windows 10 and it was developed using the open-source Python's Pyinstaller library. It is standalone, thus it does not require a separate Python installation on the target machine. 

To use MIRAGE on your computer desktop, follow these steps:
  1. download the .exe file to a Windows 10 OS device
  2. lauch it directly by double-clicking

## MIRAGE: instructions for use
Whether you have installed the application on a mobile device or are using it via a desktop computer, its extremely intuitive and simple operation is the same. Once the application is open, you simply need to enter some basic clinical data (_age_, _serum creatinine at biopsy_, _proteinuria_, _amount of FLC kappa_, and _amount of FLC lambda_) and select one of the available options for the following fields: _sex_ (_female_, _male_), _Bence Jones_ (_yes_, _no_), _M-spike_ (_yes_, _no_), _type of FLC_ (_lambda_, _kappa_), and _type of heavy chain_ (_IgA_, _IgG_, _IgD_, _IgM_). Note that when both _Bence Jones_ and _M-spike_ (_yes_, _no_) are set to _no_, the fields _type of FLC_ and _type of heavy chain_ will automatically disappear, as they would be not applicable. 
The use of an Extreme Gradient Boosting algorithm enables predictions even in the absence of some input data, which benefits end-users in routine practice by allowing MGRS risk estimation even when input data is incomplete. However, based on the design of the prediction model, the only fields that do not allow missing values are _sex_ and _M-spike_. If these fields are left empty, the system displays a warning and does not allow proceeding with the prediction calculation.

After entering the clinical data, pressing the _Predict_ button will allow the system to process the data and return, in real-time, the patient’s classification (MGRS vs. non-MGRS) along with the confidence level of the prediction.







![Figure 4 (1)](https://github.com/user-attachments/assets/a59815c4-80ed-46f7-961e-414906148468)


## MGRS Predictor Research-Only License
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute the Software, subject to the following conditions:

- Research and Non-Commercial Use Only: The Software may only be used for research purposes and non-commercial activities. The Software must not be used for clinical decision-making, patient diagnosis, or treatment. Any commercial use or clinical application of this Software is strictly prohibited.

- Attribution: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

Disclaimer: THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES, OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF, OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
