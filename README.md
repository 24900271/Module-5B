# Python Manual Lab

# Module-5B

# EXP-01 Mathematical Operations on Pandas Series

# Aim: 

perform multiplication and division operations between two Pandas Series.

# Algorithm:

Import the Pandas library.
Create two Series a1 and a2.
Multiply corresponding elements of the Series.
Divide elements of a1 by a2.
Display the multiplication result.
Display the division result.

# Program:

```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import pandas as pd
a1 = pd.Series(eval(input()))
a2 = pd.Series(eval(input()))
multiplication_result = a1 * a2
division_result = a1 / a2
print("Multiplication of two Series:")
print(multiplication_result)
print("Division of Series1 by Series2:")
print(division_result)
```

# Output:

<img width="1187" height="943" alt="image" src="https://github.com/user-attachments/assets/1ee24945-9068-40dd-9ddd-30484baed26e" />

# EXP-02 CSV File Handling in Python

# Aim:

To create a CSV file containing car details and read its contents.

# Algorithm:

Import the csv module.
Create a CSV file named cars_model.csv.
Write the header row.
Write the car details into the file.
Open the file in read mode.
Read the header using next().
Read the remaining rows.
Display the header and data rows.

# Program:

```
import csv
column_name=['No', 'Company', 'Car Model']
car=eval(input())
header=['No', 'Company', 'Car Model']
with open("Names.csv",'w') as csvfile:
    writer=csv.DictWriter(csvfile, fieldnames=column_name)
    writer.writeheader()
    writer.writerows(car)
rows=[]
```

# Output:

<img width="1190" height="430" alt="image" src="https://github.com/user-attachments/assets/86739b1d-635e-4ffa-98a2-f09f1f580af8" />

# EXP-03 Frequency Count of Array Elements

# Aim:

To count the frequency of unique values in a NumPy array.

# Algorithm:

Import the NumPy library.
Create a NumPy array.
Use numpy.unique() with return_counts=True.
Store unique values and their frequencies.
Combine them into a two-column array.
Display the result.

# Program:

```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
a=np.array(eval(input()))
uv,c=np.unique(a,return_counts=True)
r=np.column_stack((uv,c))
print(r)
```

# Output:

<img width="1181" height="525" alt="image" src="https://github.com/user-attachments/assets/5ff501d5-94dd-4600-a200-c5055e9eddd0" />

# EXP-04 DataFrame Merging in Pandas

# Aim:

To merge two Pandas DataFrames using multiple join keys.

# Algorithm:

Import the Pandas library.
Create the first DataFrame.
Create the second DataFrame.
Display both DataFrames.
Use the merge() function with multiple keys (key1 and key2).
Store the merged result.
Display the merged DataFrame

# Program:

```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import pandas as pd
data1 = eval(input())
data2 = eval(input())
df1 = pd.DataFrame(data1)
df2 = pd.DataFrame(data2)
print("Original DataFrames:")
print(df1)
print("--------------------")
print(df2)
result = pd.merge(df1, df2, on=['key1', 'key2'])
print("\nMerged Data:")
print(result)
```

# Output:

<img width="1186" height="702" alt="image" src="https://github.com/user-attachments/assets/45f6b2cc-c584-494e-9109-fa8b61e967f0" />

# EXP-05 Create Arrays of Zeros, Ones, and Fives Using NumPy

# Aim:

To create arrays consisting of zeros, ones, and fives using NumPy.

# Algorithm:

Import the NumPy library.
Read the size of the arrays.
Create an array of zeros using np.zeros().
Create an array of ones using np.ones().
Create an array of fives using np.full().
Display all three arrays.
End the program.

# Program

```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
n1=int(input())
n2=int(input())
n3=int(input())
arr1=np.zeros(n1)
arr2=np.ones(n2)
arr3=np.full(n3,5,dtype=float)
print("An array of 10 zeros:")
print(arr1)
print("An array of 10 ones:")
print(arr2)
print("An array of 10 fives:")
print(arr3)
```

# Output:

<img width="1186" height="550" alt="image" src="https://github.com/user-attachments/assets/a21d4e3f-1561-415c-a41a-d537cf13f495" />






