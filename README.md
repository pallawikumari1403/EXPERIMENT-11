# Experiment No. 11: Create and Load Dataset using Pandas
## Aim:
To create a dataset using Python and Pandas, save it as a CSV file, and perform basic data analysis operations. Also, to load an existing dataset and explore its structure and contents.
## Theory:
# Dataset Creation
A dataset of student details was created using a Python dictionary and converted into a Pandas DataFrame.
Dataset Attributes
* Roll_No
* Gender
* Department
* CGPA

### Code

```python
import pandas as pd

data = {
    "Roll_No":[101,102,103,104,105],
    "Gender":["Female","Male","Female","Male","Female"],
    "Department":["Computer","IT","ENTC","Mechanical","Computer"],
    "CGPA":[8.2,7.5,9.1,6.8,8.7]
}
<img width="1117" height="791" alt="Screenshot 2026-03-30 105343" src="https://github.com/user-attachments/assets/3f2fe37c-5d3a-472a-8ef7-149edc61cb68" />
<img width="1119" height="786" alt="Screenshot 2026-03-30 105422" src="https://github.com/user-attachments/assets/15240fc3-b3cd-49d6-af37-747fd65b7e8d" />
<img width="1120" height="783" alt="Screenshot 2026-03-30 105455" src="https://github.com/user-attachments/assets/1e334d8b-a6d7-42ca-b458-b6a07eea389f" />

df = pd.DataFrame(data)
df.to_csv("students.csv", index=False)<img width="1117" height="791" alt="Screenshot 2026-03-30 105343" src="https://github.com/user-attachments/assets/59a6acda-c2a8-4a5f-b7f7-298827a22e30" />
<img width="1119" height="786" alt="Screenshot 2026-03-30 105422" src="https://github.com/user-attachments/assets/e8dfab48-6fc6-407f-83b3-2534c79c26dc" />
<img width="1120" height="783" alt="Screenshot 2026-03-30 105455" src="https://github.com/user-attachments/assets/363d826e-4f05-4ecb-873c-a90006a1a520" />

```

* Dataset contains **5 rows and 4 columns**
* No missing values
* Data types:

  * Integer (Roll_No)
  * Float (CGPA)
  * Object (Gender, Department)

---

## Dataset Exploration
 Basic Operations Performed

* `df.size` → Total elements = 20
* `df.shape` → (5, 4)
* `df.info()` → Structure and data types
* `df.describe()` → Statistical summary

---

##  Loading Existing Dataset

An existing dataset (`Cars93.csv`) was loaded and analyzed.

### Code

```python
import pandas as pd
import numpy as np

df = pd.read_csv('/content/Cars93.csv')
```
## Dataset Details
Columns
* Manufacturer
* Model
* Type
* Price
* MPG.city
* AirBags
* Horsepower
* Passengers
* Rear.seat.room
* Luggage.room

### Shape & Size

* Rows: 93
* Columns: 10
* Total elements: 930

---

## Data Analysis Operations

### Functions Used

* `df.head()` → First 5 rows
* `df.tail()` → Last 5 rows
* `df.sample(10)` → Random sample
* `df.columns` → Column names
* `df.nunique()` → Unique values

---

## Data Cleaning:
 Missing Values
* AirBags: 34 missing
* Rear.seat.room: 2 missing
* Luggage.room: 11 missing

 Duplicate Records
* No duplicate rows found

## Statistical Summary
* Average Price: 19.50
* Average MPG.city: 22.36
* Average Horsepower: 143.82
* Passenger capacity ranges from 2 to 8

## Conclusion:
Therefore we learn
* How to create and save datasets using Pandas
* How to load external datasets
* Performing exploratory data analysis (EDA)
* Identifying missing values and dataset structure
using python
Pandas provides powerful and efficient tools for handling structured data in Python.
## Refrence Images:

