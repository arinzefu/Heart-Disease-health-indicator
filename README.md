# Heart Disease health indicator

About Dataset
The dataset is from kaggle and URL is https://www.kaggle.com/datasets/abubakarsiddiquemahi/heart-disease-dataset

I preprocessed the dataset and mapped  the columns 'HeartDisease', 'Smoking', 'AlcoholDrinking', 'Stroke', 'DiffWalking', 'PhysicalActivity', 'Asthma', 'KidneyDisease', 'SkinCancer' to Yes  = 1, No = 0
For the sex column 'Male': 1, 'Female': 0
I took the median of the age category column and for 80 and above i used 85
genhealth column = 'Very good': 0, 'Good': 1, 'Excellent': 2, 'Fair': 3, 'Poor': 4
diabetic column = 'No': 0, 'Yes': 1, 'No, borderline diabetes': 2, 'Yes (during pregnancy)': 3
race column = 'White': 0, 'Hispanic': 1, 'Black': 2, 'Other': 3, 'Asian': 4, 'American Indian/Alaskan Native': 5
column 'diffwalking' is Difficulty walking
column 'BMI' is body mass index
column 'GenHealth' is general health

I did not fully deploy the model but i gave how the interface should look like.

I also realize I did not test out the model like I hoped to I am sorry.
The code provided is a summary of a Jupyter Notebook titled "Heart_Disease_model.ipynb". Here are the key points covered in the code:

The input features are scaled using the MinMaxScaler from scikit-learn.
Time series generators are created using the TimeseriesGenerator class from Keras to generate input-output pairs for the LSTM model.
A sequential model is defined in Keras, consisting of convolutional, pooling, LSTM, and dense layers.
