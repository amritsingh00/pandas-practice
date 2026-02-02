# pandas-practice
This repository contains Python programs for data analysis using Pandas
#adding column 
#there are 2 methodsprint(df)
#1st method df["column_name"]= some_data
#using insert method(important) - df.insert(loc,"column_name", some_data)

import pandas as pd
data = {
    "name" : ["Rahul", "Aman", "Priya", "Neha", "Rohit", "Anjali"],
    "ages" : [22, 24, 21, 23, 25, 22],
    "salaries" : [25000, 30000, 22000, 28000, 35000, 26000],
    "performance_scores" : [7, 8, 6, 9, 8, 7]
}
df = pd.DataFrame(data)
print(df)
#increment of 10% OF SAlary by 1st method
df["bonus"] = df["salaries"] * 0.1
print(df)

#2nd method - making employee id
df.insert(0,"employee ID",[ 10,20,30,40,50,60])
print(df)
