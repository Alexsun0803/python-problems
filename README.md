# python-problems
Task 1

Given an integer, , perform the following conditional actions:
If n is odd, print Weird
If n is even and in the inclusive range of 2 to 5 , print Not Weird
If n is even and in the inclusive range of 6 to 20 , print Weird
If n is even and greater than 20 , print Not Weird

Solution

N=int(input())

if(N%2==1):
   print("Weird")
 
 elif(N in range (2,6)):
   print("Not Weird")
   
 elif( N in range (6,21)):
   print("Weird")
   
 elif(N>20):
   print("Not Weird")
   
-----------------------------------------------------------------------------
Task 2

Read two integers and print two lines. The first line should contain integer division, a //b . The second line should contain float division,  a/ b.
You don't need to perform any rounding or formatting operations.

Solution

a = int(input())
b = int(input())

print(a//b) #integer division
print(a/b) #floating point division

--------------------------------------------------------------------------------
Task 3

Read two integers from STDIN and print three lines where:
The first line contains the sum of the two numbers.
The second line contains the difference of the two numbers (first - second).
The third line contains the product of the two numbers.


Solution

a = int(input())
b = int(input())
print(a+b)
print(a-b)
print(a*b)


---------------------------------------------------------------------------------------
Task 4

Read an integer N. For all non-negative integers i < N , print i **2. See the sample for details.


Solution 1

a = int(input())
for i in range (a):
   print (i**2)
   
Solution 2

for i in range(int(raw_input())):
    print i**2
   
 ------------------------------------------------------------------------------------------  
Task 5
 
 
We add a Leap Day on February 29, almost every four years. The leap day is an extra, or intercalary day and we add it to the shortest month of the year, February. 
In the Gregorian calendar three criteria must be taken into account to identify leap years:
The year can be evenly divided by 4, is a leap year, unless:
The year can be evenly divided by 100, it is NOT a leap year, unless:
The year is also evenly divisible by 400. Then it is a leap year.
This means that in the Gregorian calendar, the years 2000 and 2400 are leap years, while 1800, 1900, 2100, 2200, 2300 and 2500 are NOT leap years.


 
You are given the year, and you have to write a function to check if the year is leap or not.
Note that you have to complete the function and remaining code is given as template.


Solution

#writnig a Fuction
def is_leap(year):
    leap = False
    
    # Write your logic here
    if(year%4==0):
        
        if(year%100 ==0):
            if(year%400==0):
                return True
            else:
                return False
        else:
            return True
               
    else:
        return False
        
        
year = int(input())
print(is_leap(year))

--------------------------------------------------------------------------------------


