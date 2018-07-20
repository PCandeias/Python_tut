# Python_tut
~~~~python
# You can create a variable as such:
a=5
# To print, you can simply use:
print(a)
# A variable can be modified, regardless of type
a='str'
# To create a list, you can do the following:
tab=[1,2,3]
# You can also create a list of different types:
tab=[1,'mot',3]
# You can access a specific element in the list by using [i]
print(tab[0])
# You can also modify it as follows:
tab[2]=5
# You can use a for loop to iterate through the list:
for element in tab:
  print(element)
# You can also use if-else blocks similar to other languages:
if tab[0] == 1:
  print('Hello world')
# Indentation is used in python to create separate blocks, instead of the typical {}
for element in tab:
  if element == 1:
    print(element)
~~~~

## Exercise 1
- Create an array containing 3 times the value 0. Print all the different values.
- Replace the first 0 with a 5. Print all the different values.


~~~~python
# You can create an iterable object containing numbers from 0 to 10, not including 10, as such:
obj=range(10)
# You can use that in a for loop to print all numbers from 0 to 10
for i in range(10):
  print(i)
# You can also create an iterable object from 5 to 10, not including 10, as such:
obj=range(5,10)
# In Python3, you can iterate through this object, but it's not a list. 
# To create a real list containing elements from 0 to 10, you can do:
array=list(range(10))
print(array)
# The same operators as in c++ are still valid in python, +,-,*,/,%, etc
# Instead of the typical '||' and '&&' operators, python uses 'and' and 'or'
# Example:
if i == 6 and i%2 == 0:
  print(i)
# Boolean values in python are 'True' and 'False'
~~~~

## Exercise 2
- Print all even numbers between 0 and 10

## Exercise 3
- Create an array of size 10 containing only 5's, without explicitly using array = [5,5,5,...,5,5]
###### Hint: use array[i] = 5 to modify value at index i


~~~~python
# A function can be defined in python as such:
def printHello():
  print('Hello')
# It can then be called using the following syntax:
printHello()
# Functions may contain arguments used to create different behaviours
def printHelloRepeat(num):
  for i in range(num):
    printHello()
# This would then be called as follows to print 'Hello' 5 times:
printHelloRepeat(5)
# Functions may also return values which can then be used in the rest of the program
def getNum(num):
  return num
a = getNum(5) # Has value 5
# Functions that return objects of a certain type can be used in any place where that type would make sense
if getNum(3) == 5:
  for i in range(getNum(4)):
    print(i)
~~~~

## Exercise 4:
- Create a function which takes a number as an argument and prints 'odd' if the number is odd and 'even if the number is even
- Create a function which return True if the number is odd and False otherwise. Use this function in a for loop to print all odd numbers between 0 and 10

~~~~python
# Similar to other programming languages, python can use while loops:
count = 0
while count <= 10:
  count += 1
  print('hello')
~~~~

## Exercise 5:
- Print the first 10 odd numbers that are a multiple of 5 and 3

## Exercise 6(Harder):
- Create a function that tells you if a number is prime or not
- Print the first 20 prime numbers
~~~~python
# A different syntax for creating arrays in python which is very useful is:
array = [i for i in range(10)] # Numbers from 0 to 10 (10 not included)
# This can be useful when you don't just use i:
array = [i*3 for i in range(10)] # Contains 10 first multiples of 3
# You can also filter some of the values by using ifs
array = [i for i in range(10) if i%2==0] # contains [0,2,4,6,8]
# You can access more then one element in an array by using the following syntax
array[1:3]
# You can also leave fields unspecified, and the interpreter will figure it out
array[:3] # Same as array[0:3]
array[0:] # same as array[0:5] for array of size 5
# You can learn the size of an array by using the len() function
size = len(array)
# You can also convert a int to a string using the str() function
a = 'str' + str(3)
# You can also convert a VALID string into a int using the int() function (it needs to actually only contain number caracters)
num = int('5434')
~~~~
