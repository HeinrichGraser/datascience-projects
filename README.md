# datascience-projects
## 1. Heartattack data

<b> Based on a kaggle dataset </b>: https://www.kaggle.com/rashikrahmanpritom/heart-attack-analysis-prediction-dataset <br>
<b> Data </b>: <br>
    <BLOCKQUOTE>
    Age : Age of the patient <br>
    Sex : Sex of the patient <br>
    exang: exercise induced angina (1 = yes; 0 = no) <br>
    ca: number of major vessels (0-3) <br>
    cp: Chest Pain type chest pain type <br>
        <BLOCKQUOTE>
        Value 1: typical angina <br>
        Value 2: atypical angina <br>
        Value 3: non-anginal pain <br>
        Value 4: asymptomatic <br>
        </BLOCKQUOTE>
    trtbps: resting blood pressure (in mm Hg) <br>
    chol: cholestoral in mg/dl fetched via BMI sensor <br>
    fbs: (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false) <br>
    rest_ecg: resting electrocardiographic results <br>
        <BLOCKQUOTE>
        Value 0: normal <br>
        Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV) <br>
        Value 2: showing probable or definite left ventricular hypertrophy by Estes' criteria <br>
        </BLOCKQUOTE>
    thalach: maximum heart rate achieved <br>
    output: 0= less chance of heart attack 1= more chance of heart attack <br>
    </BLOCKQUOTE>

<b> Goal </b>: Train a classifier to predict which patient probably had a hearattack.  <br>
<b> Approach </b>: I evaluated different classifiers to see, which of them yields the best classification results. Furthermore, to find out why the best performing classifier worked as it did, the python libraries eli5 and pdpbox where used.

