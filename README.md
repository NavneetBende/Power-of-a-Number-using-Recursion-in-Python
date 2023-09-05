# Power-of-a-Number-using-Recursion-in-Python


Power  of  a  Number
On this page we will see how to find Power of a Number in Python. We will see three methods to do so. User have to give base and power as input. Power of a number is basically multiplying the base number by itself , power number of time.

Example :

Input  :  base = 2, power = 3
Output  :  8
Explanation  :   23 means 2 is base and 3 is power which is 3 times 2 (  2 x 2 x 2 ) which is equals to 8
Method 1 : Using Recursion
Algorithm
We will first assign value of a as base and b as power of number.
We will pass a and b to function power.
We will use recursion to find the answer.
We will recursively call the function power and each time we will return a*power(a,b-1) till the time b is not equal to zero. Each recursion call will return a multiply by a till b is not zero. In each call we will decrement the value of b by 1.
If b is equal to zero then we will return from the function.
Python Program for Power of a Number

Python Code
Run
def power(a, b):
    if b != 0:
        return a * power(a, b - 1)
    else:
        return 1


a = 2
b = 3
print(a, "to the power", b, "is", power(a, b))
Output:

2 to the power 3 is 8
Related Pages
Finding Number of times x digit occurs in a given input
 
Finding number of integers which has exactly x divisors
 
Smallest element in an array

Prime Number

Largest element in an array

Method 2 : Using For Loop
Algorithm
We will first assign value of a as base and b as power of number.
We will pass a and b to function power.
We will declare a new variable ans to store final answer.
We will use for loop to find power using variable i.
For loop will run from o till b-1. And for each iteration we will multiply a with a.
After completing iterating from for loop we will then return ans.
Python Code
Run
def power(a, b):
    ans = a
    for i in range(b - 1):
        ans = a * ans
    return ans


a = 2
b = 3
print(a, "to the power", b, "is", power(a, b))
Output:

2 to the power 3 is 8
