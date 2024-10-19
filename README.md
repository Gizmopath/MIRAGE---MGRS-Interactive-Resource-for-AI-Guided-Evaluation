# MIRAGE---MGRS-Interactive-Resource-for-AI-Guided-Evaluation ![Oasi (1)](https://github.com/user-attachments/assets/0951ea44-7f5d-4d37-b78d-15239116ea6f)
A user-friendly application designed to assist clinicians in predicting the likelihood of Monoclonal Gammopathy of Renal Significance (MGRS) before performing a kidney biopsy. 

## Project Overview

This tool was developed as part of a retrospective cohort study conducted across three medical centers in Italy:

- The Nephropathology Center at IRCCS Fondazione San Gerardo dei Tintori, Monza, University of Milano-Bicocca (UNIMIB)
- The Nephrology Unit at Spedali Civili Hospital, Brescia
- The Nephrology, Dialysis, and Kidney Transplant Unit at IRCCS Azienda Ospedaliero-Universitaria, Bologna

The dataset includes **438 renal biopsy cases** collected between 2018 and 2022, with 43% classified as MGRS based on biopsy results. The model was trained to differentiate between MGRS and non-MGRS cases using clinical variables such as age, serum creatinine, proteinuria, presence of M-spike, Bence-Jones protein, and free light chain (FLC) ratios.

## Key Features

- **ML-Based Classifier**: The model is built using the Extreme Gradient Boosting (XGBoost) algorithm, achieving an accuracy of **0.88** and an AUC-ROC of **0.90** on test data.
- **Predictive Flexibility**: The model can still make predictions even with missing data, making it highly useful for real-world clinical scenarios where complete datasets are not always available.
- **Desktop & Mobile Applications**: A user-friendly interface allows clinicians to easily input patient data and generate predictions. The tool is designed to run on both desktop and mobile devices.

## How to Use

![Figure 4 (1)](https://github.com/user-attachments/assets/a59815c4-80ed-46f7-961e-414906148468)


## MGRS Predictor Research-Only License
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute the Software, subject to the following conditions:

- Research and Non-Commercial Use Only: The Software may only be used for research purposes and non-commercial activities. The Software must not be used for clinical decision-making, patient diagnosis, or treatment. Any commercial use or clinical application of this Software is strictly prohibited.

- Attribution: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

Disclaimer: THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES, OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF, OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
