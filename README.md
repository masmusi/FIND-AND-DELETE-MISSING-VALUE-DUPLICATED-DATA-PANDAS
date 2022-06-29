# FIND-AND-DELETE-MISSING-VALUE-DUPLICATED-DATA-PANDAS
Simple way how to find and delete missing value and duplicated data using Jupyter Notebook

-------------------------- FIND / DELETE MISSING VALUE ---------------------------------------------------------

Step 1. Save data with name 'Admission_data.csv'

![image](https://user-images.githubusercontent.com/108322484/176373706-84dfc5ba-114e-4059-8968-0bbd0ac06430.png)

Step 2. import pandas library and read file 'Admission_data.csv'
import pandas as pd
data = pd.read_csv('admission_data.csv')
data.head(5)

Step 3. Find missing value in data using code :
data.isna().sum()

![image](https://user-images.githubusercontent.com/108322484/176374243-462433e3-c2e4-48f6-8982-1d53370847e5.png)

Step 4. Delete missing value with code :
data = data.dropna()

Step 5. Finaly, missing value has deleted
data.isna().sum()

![image](https://user-images.githubusercontent.com/108322484/176375055-fe16827f-67f4-4b14-90d9-be80fa97c898.png)

-------------------------- FIND / DELETE DUPLICATED VALUE ---------------------------------------------------------
Step 1. Find duplicated value in data with code :
data.duplicated().sum()

![image](https://user-images.githubusercontent.com/108322484/176375578-a64782ff-6ef3-4191-b1e1-80561994eaa5.png)

Step 2. Delete duplicated value in data with code :
data = data.drop_duplicates()

Step 3. Finaly, duplicated value has deleted

![image](https://user-images.githubusercontent.com/108322484/176375744-520dbf56-151d-454e-ac44-19a1f5b29bab.png)

Noted :
You can find completed source code in 'TRAINING CODE.ipynb'
