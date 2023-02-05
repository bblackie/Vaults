
## CodeWOF

### Value

- Learning syntax and the importance of indentation
- A simple looking drag and drop problem can contain a surprising amount of information
	- e.g. Double Evens
- Shows us how important attention to detail is, i.e. a single wrong character will break test
- Note that there is a lot of information in the question, which will be very useful to you when you start handwriting Python
	- Note that some problems provide both the Parsons and hand-scripting interfact formats so you can solve the same problem first in Parsons and then flip to hand-scripting to see how much you have remembered
		- e.g. Double Evens
			- https://www.codewof.co.nz/questions/5/
			- https://www.codewof.co.nz/questions/4/
- Introduces us to TDD (Test Driven Development), which says write your tests first and iterate until they pass.
- When write code use comments to structure your thinking, i.e. start by copying down the question/requirements and then write your answer in pseudocode before actually writing it Python
	- A comment block in Python is created by wrapping, i.e. putting the key character or combination of character at either end.  We do a lot of wrapping in coding!
	e.g. '''Comment goes here''' or even better
	'''
	comment goes here
	'''
'''
Write a function double_even(number) that takes a number and returns double the number if it is even. 
Otherwise it returns the original number.

function double_even(number)
    if number is even    
        return number x 2
    else
        return number
'''
def double_even(number):
    if number % 2 == 0:
        return number * 2
    else:
        return number


		
			-


