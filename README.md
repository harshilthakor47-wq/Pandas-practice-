# Pandas-practice-
import pandas as pd

data = {

        "name" : ["A","B","C","D"],

        "math": [45,60,88,30],

        "science": [78,55,92,40]
        
}

df=pd.DataFrame(data)



print(df[["math","science"]])




print(df.loc[0])




df["total"]=df["math"]+df["science"]

print(df["total"])

print(df)


print(df[df["math"]>50])


print(df["math"])
print(df["math"].mean())


df["average"] = (df["math"]+df["science"])/2


print(df)

print(df[df["average"]>60])

print(df)
print(df["total"].idxmax())
