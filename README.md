# datascience-projects
## 1. Heartattack data

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Blausen_0463_HeartAttack.png/675px-Blausen_0463_HeartAttack.png" width="250" height="400" alt="Heart picture"> 
<b> Based on a kaggle dataset </b>: https://www.kaggle.com/rashikrahmanpritom/heart-attack-analysis-prediction-dataset <br>
<b> Data </b>: <br>
    <BLOCKQUOTE>
    Age: Age of the patient <br>
    Sex: Sex of the patient <br>
    exang: exercise induced angina (1 = yes; 0 = no) <br>
    ca: number of major vessels (0-3) (renamed to count_blood_vessels) <br>
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
    output: 0= heartattack; 1= no heartattack <br>
    </BLOCKQUOTE>

<b> Goal </b>: Train a classifier to predict which patient probably had a hearattack.  <br>
<b> Approach </b>: I evaluated different classifiers to see, which of them yields the best classification results. Furthermore, to find out why the best performing classifier worked as it did, the python libraries eli5 and pdpbox where used. <br>
<b> Result </b>: The dataset is best classified by a logistic regression with an average accuracy of 0.854138 (test_size = 0.2, cv = 10, no grid search). Counterintuively, not high blood pressure, high blood sugar or high cholesterine values, but the attribute count_blood_vessels hast the highest impact onto the classification.




# datascience-projects
## 2. Stroke data

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/49/MCA_Territory_Infarct.svg/491px-MCA_Territory_Infarct.svg.png" width="250" height="400" alt="Heart picture"> 
<b> Also based on a kaggle dataset </b>: https://www.kaggle.com/fedesoriano/stroke-prediction-dataset <br>
<b> Data </b>: <br>
    <BLOCKQUOTE>
    id: id
    gender: gender of patient
    age: age of patient
    hyptertension: chronically increased blood pressure (1/0)
    heart_disease: patient has heart disease (1/0)
    ever_married: patient was/is married (Yes/No)
    work_type: the work type of the patient (private/Self_employed/Govt_job/children/Never_worked)      
    Residence_type: where the patient lives (Urban/Rural)
    avg_glucose_level: avg. blood sugar level
    bmi: body-mass index
    smoking_status: the smoking status of the patient (formerly smoked/never smoked/smokes/Unknown)
    stroke: had stroke (1/0)


<b> Goal </b>: Train a classifier to predict which patient had a stroke  <br>
<b> Approach </b>: I evaluated different classifiers to see, which of them yields the best classification results. Furthermore, to find out why the best performing classifier worked as it did, the python library eli5 was used. <br>
<b> Result </b>: The dataset is best classified by a random forest with an average accuracy of 0.86 (test_size = 0.2, cv = 10, grid searched parameters). As expected, the attribute age is most important for classifying strokes. After age, it is not entirely clear if ever_married_Yes or the avg_glucose_level has the second strongest influence on the model, since ever_married_Yes might be very similar to age.
