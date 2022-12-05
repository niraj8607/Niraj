# Niraj
"""LIST OF LEAP YEARS AND NOT LEAP YEARS BETWEEN TWO DATE DY USER INPUT"""
starting_date=input("enter the date in dd/mm/yyyy format:")
ending_date=input("enter the date in dd/mm/yyyy format:")
x=int(starting_date[6:10])
y=int(ending_date[6:10])
a=list()
b=list()
print("list of leaps years----")
for i in range(x,y+1):
    if (i%400==0) or (i%4==0 and i%100!=0):
        a.append(i)
    else:
        b.append(i)
print(a)
print("list of non leaps years------")
print(b)
