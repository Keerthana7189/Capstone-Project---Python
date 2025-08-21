# Capstone-Project---Python

This repository contains the Python Capstone Project using CSV datasets. The project demonstrates data cleaning, analysis, and transformations using Python.

---

## Datasets Used

- Project DataFrame  
- Employee DataFrame  
- Seniority-Level DataFrame  

---

## Project Overview

The project covers the following tasks using Python and pandas:

1. Create three DataFrames (Project, Employee, Seniority-Level) and save as CSV files.
2. Fill missing Cost values in Project DataFrame using running average with a for loop.
3. Split Name column in Employee DataFrame into FirstName and LastName, drop the old Name column.
4. Join all three DataFrames into a single DataFrame called Final.
5. Add a 5% bonus column in Final for employees with completed projects.
6. Demote designation level by 1 for employees whose projects failed, and delete records where designation level > 4.
7. Add "Mr." or "Mrs." to FirstName based on gender, and drop the Gender column.
8. Promote designation level by 1 for employees older than 29 years.
9. Compute total project cost per employee and save as a new DataFrame TotalProjCost.
10. Print all employee details whose City contains the letter "o".

---

## Python Section

**Libraries used:**
- pandas
- numpy

### Python Section: Employee DataFrame

**Create Employee DataFrame**
```python
import pandas as pd

# Create Employee DataFrame
employee_data = {
    'ID': ['A001','A002','A003','A004','A005'],
    'Name': ['John Alter','Alice Luxumber','Tom Sabestine','Nine Adgra','Amy Johny'],
    'Gender': ['M','F','M','F','F'],
    'City': ['Paris','London','Berlin','Newyork','Madrid'],
    'Age': [25, 27, 29, 31, 30]
}

# Creating DataFrame
df_employee = pd.DataFrame(employee_data)

# Display DataFrame
df_employee

