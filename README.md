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
   




