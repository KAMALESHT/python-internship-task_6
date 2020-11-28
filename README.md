# python-internship-task_6


1.Write a program to loop through a list of numbers and add +2 to every value to elements in list.

Solution:

list_1=[1,2,3,4,5]

list_2=[]

for i in range(0,len(list_1)):

    list_2.append(list_1[i]+2)

print(list_2)

2.Write a program to get the below pattern

54321

4321

321

21

1

Solution:

r=int(input("Enter the no of rows:"))

for i in range(0,r+1):

    for j in range(r-i,0,-1):

        print(j,end='')

    print()

3.Python Program to Print the Fibonacci sequence

Solution:

def fibo(n):

    if n<=1:

        return n

    else:

        return fibo(n-1)+fibo(n-2)

fibo_terms=int(input("Enter the no:"))

if fibo_terms<=0:

    print("enter a valid no")

else:

    print("fibonacci sequence:")

    for i in range(fibo_terms):

        print(fibo(i))

4.Explain Armstrong number and write a code with a function

Solution:

n=int(input("Enter the no:"))

s=0

temp=n

while(temp>0):

    val=temp%10

    s+=val**3

    temp=temp//10

if(n==s):

    print("the no is an armstrong number")

else:

    print("the no is not an armstrong numer")

5.Write a program to print the multiplication table of 9

Solution:

n=9

for i in range(1,11):

    print(n,"x",i,"=",n*i)

n=int(input("Enter the no:"))

6.Check if a program is negative or positive

Solution:

if n>0:

    print("the no is positive")

else:

    print("the no is negative")

7.Write a program to convert the number of days to ages

Days=int(input("enter the no of days:"))

years=int(Days/365)

print("Days to years=",years)

8.Solve Trigonometry problem using math function write a program to solve using math function

Solution:

import math

x=math.pi/4

y=4

z=5

print("the cosine value of pi/4 is:")

print(math.cos(x))

print("the hypotenuse value of 4 and 5 is:")

print(math.hypot(y,z))

9.Create a calculator only on a code level by using if condition (Basic arithmetic calculation)

Solution:

print("***Calculator****")

print("    1.Addition")

print("    2.Subraction")

print("    3.Multiplication")

print("    4.Division")

choice=int(input("enter your choice:"))

if choice==1:

    x=int(input("enter the first no:"))

    y=int(input("enter the second no:"))

    z=x+y
    
    print("Sum=",z)

elif choice==2:

    x=int(input("enter the first no:"))

    y=int(input("enter the second no:"))

    z=x-y
    
    print("Differnce",z)

elif choice==3:

    x=int(input("enter the first no:"))

    y=int(input("enter the second no:"))

    z=x*y
    
    print("Product",z)

elif choice==4:

    x=int(input("enter the first no:"))

    y=int(input("enter the second no:"))

    z=x/y
    
    print("Quotient",z)

else:
    print("Invalid choice!!")
