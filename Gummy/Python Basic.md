# Python basic syntax

## Introduction

Because the team has some programming experience in other languages, we found the basic syntax of Python easy to pick in that is has many similarities. It is said that Python is a higher level language or "glue" language  similar to Perl rather than lower level language such as Java or C. The advantage of this is that you can quickly produce working programs with just a few lines of code. For example, there is a lot you can do in Python without even defining a class and just using the standard built-in types and functions. In this report, we will demonstrate the basic syntax and some of the built-in types and functions of Python.

### The interpreter

Python is available to Windows, Mac OS X, and Unix operating systems. On Windows, it must be downloaded and installed. For Unix and OS X it comes pre-installed with most distributions but the versions differ. If you wish to upgrade, you can download and install the latest version. Python has two main versions still in use which are 2.x and 3.x. The syntax varies greatly between versions but now that 2.x versions are no longer being developed, it is recommended to learn one of the 3.x versions.

Once installed, you can start the interpreter interactively by running the python executable. This is also known as "calculator mode" and it allows you to write an expression and it will process the value. This mode is great for banging out commands or writing small programs. Below is an example of starting Python interactively.

		PS C:\temp> & python.exe
		Python 3.6.2 (v3.6.2:5fd33b5, Jul  8 2017, 04:14:34) [MSC v.1900 32 bit (Intel)] on win32
		Type "help", "copyright", "credits" or "license" for more information.
		>>> 2 + 2
		4
		>>>
		>>> quit()
		PS C:\temp>

To run a script with the python interpreter, run the cmd followed by the path to the script. You can also use argument -i to stay open interactively.

		PS C:\temp> python -i C:\temp\hello.py
		Hello world
		>>>
		>>>
		>>> quit()
		PS C:\temp>

## Define, assign and use of variables

The main built-in types available are bool, int, float and string. You can assign a value to a variable using the = sign as per examples below:

		>>> bool = True
		>>> int = 1
		>>> float = 1.23
		>>> string = "This is a string"
		>>> concatenated_string = string + ", and this is extending the string"
		>>> concatenated_string
		'This is a string, and this is extending the string'
		>>> concatenated_string[0:16] + " slice"
		'This is a string slice'

You can combine expressions and variables. For example, to calculate the total cost of a kids party:

		>>> kids = 22
		>>> lunch = 10.80
		>>> entry = 22.0
		>>> total_cost = kids * lunch + kids * entry
		>>> total_cost
		721.6

### Input and print functions

You can capture input and print output to users using the input and print built-in functions.

		>>> user_input = input("Hello, how are you today? ")
		Hello, how are you today? Good thanks!
		>>> print(user_input)
		Good thanks!


## Define, assign and use of arrays

Python has a few different types of arrays, some of which are mutable and some immutable.

### Lists

Lists are a mutable collection and are created using square brackets and comma separated values. They can be indexed and updated with new values.

		>>> list = [2, 4, 22, concatenated_string, bool]
		>>> list
		[2, 4, 22, 'This is a string, and this is extending the string', True]
		>>> list[1]
		4
		>>> list[-2]
		'This is a string, and this is extending the string'
		>>> list[-2] = "new string"
		>>> list[-2]
		'new string'
		>>> list
		[2, 4, 22, 'new string', True]
		>>> list.append("new string")
		>>> list
		[2, 4, 22, 'new string', True, 'new string']

### Tuples

Tuples are like lists but are imutable. They are created using values separated by commas. You can also use round brackets but these are optional.

		>>> tuple = (2, 4, 6)
		>>> tuple
		(2, 4, 6)
		>>>
		>>> tuple = 2, 4, 6, "eight"
		>>> tuple
		(2, 4, 6, 'eight')
		>>> tuple[3]
		'eight'
		>>> tuple[3] = 8
		Traceback (most recent call last):
		File "<stdin>", line 1, in <module>
		TypeError: 'tuple' object does not support item assignment

### Sets

Sets are unordered collection with no duplicate elements

		>>> basket = {'apple', 'orange', 'apple', 'pear', 'orange', 'banana'}
		>>> basket
		{'apple', 'banana', 'orange', 'pear'}

### Dictionaries

Dictionaries are an unordered set of key:value pairs. The key must be unique.

		>>> status = {'red': 'alert', 'green': 'healthy', 'amber': 'warning'}
		>>> status
		{'amber': 'warning', 'red': 'alert', 'green': 'healthy'}
		>>> status['red']
		'alert'
		>>> list(status.keys())
		['amber', 'red', 'green']
		>>> list(status.values())
		['warning', 'alert', 'healthy']
		>>>

## Control structures and loops

Python supports common programming structures such as if, while and for. The structures will run or loop while the expression evaluates as true or is a positive number. You can use comparisons for evaluations which include:

Operation | Meaning
--- | ---
< 	| less than
<= 	| less than or equal
\> 	| greater than
\>= 	| greater than or equal
== 	| equal
!= 	| not equal
is 	| object identity
is not | negated object identity
in	| value occurs in a sequence
not in	| does not occur in sequence
and	| boolean operator for chaining comparisons where both must be true
or | boolean operator for chaining comparisons where one must be true

### Spaces not tabs

Python differs from other languages such as Perl and C# in that it doesn't use curly brackets to group structures. Instead is uses line indentation. This encourages clean and highly readable code because the coder must ensure they are using the correct indentation. This also keeps code compact in that there is no need for closing brackets. The recommended indentation based on Python's style guide is to use 4 spaces rather than tabs.

### If statement

Below is an example of the if statement.

		>>> x = input("Is it raining today? ")
		Is it raining today? yes
		>>> if x == "yes":
		...     print("Don't forget your umbrella!")
		... else:
		...     print("Enjoy the sunshine!")
		...
		Don't forget your umbrella!
		>>>

### For statement

Below is an example of the for loop.

		>>> animals = ["cat", "dog", "chicken", "bird"]
		>>> for x in animals:
		...     print(x)
		...
		cat
		dog
		chicken
		bird

### For with range function

The range function returns an iterable. You can use it as show in below two examples.

		>>> for i in range(5):
		...     print(i)
		...
		0
		1
		2
		3
		4

Ror with range and len function. Len gives you the length of the collection.

		>>> for i in range(len(animals)):
		...     print("number", i, "Animal", animals[i])
		...
		number 0 Animal cat
		number 1 Animal dog
		number 2 Animal chicken
		number 3 Animal bird
		>>>

### While statement

Example of using a while loop.

		>>> x = 0
		>>> while x < 50:
		...     print("This number is", x)
		...     x = x +8
		...
		This number is 0
		This number is 8
		This number is 16
		This number is 24
		This number is 32
		This number is 40
		This number is 48

### Break and continue statements

The break statement is used to exit out of a loop.

		>>> for i in range(8):
		...     if i == 5:
		...         break
		...     print("loop is number", i)
		...
		loop is number 0
		loop is number 1
		loop is number 2
		loop is number 3
		loop is number 4
		>>>

The continue statement is used to skip an iteration of the loop.

		>>> for i in range(8):
		...     if i == 4:
		...         continue
		...     print("loop is number", i)
		...
		loop is number 0
		loop is number 1
		loop is number 2
		loop is number 3
		loop is number 5
		loop is number 6
		loop is number 7
		>>>


## Read and write values from a file

You can use the open function to read and write to text and binary files. The different modes available are:

Mode	|	Description
----	|----
r		| read (default mode)
w 	| write (existing file is replaced)
a		| append
r+		| reading and writing

To create a file object, use the open function with the file name and mode as arguments.

		>>> f = open('testfile.txt', 'r')

### Read file method

Once the file is open, you can read the file with the read method.

		>>> s = f.read()
		>>> s
		'This is a test file.\nSecond line in file.'
		>>> print(s)
		This is a test file.
		Second line in file.

You can also loop over the file object and process one line at a time. This is memory efficient and fast.

		>>> f = open('testfile.txt', 'r')
		>>> for line in f:
		...     print(line, end='')
		...
		This is a test file.
		Second line in file.
		>>>


### Write file method

Open the file in write mode and write changes as required.

		>>> f = open('testfile.txt', 'w')
		>>> f.write(s)
		41
		>>> f.write('\n')
		1
		>>> f.write('Adding third line to file')
		25
		>>> f = open('testfile.txt', 'r')
		>>> print(f.read())
		This is a test file.
		Second line in file.
		Adding third line to file
		>>>

### Optional

Because on some console (command prompt) there could be a problem with encoding with files and making everything crash, it is preferably to use encoding argument when opening (or even writing) files.

		>>> f = open('testfile.txt', 'w', encoding='utf-8')
		>>> f.write(s)
		41
		>>> f.write('\n')
		1
		>>> f.write('Adding third line to file')
		25
		>>> f = open('testfile.txt', 'r', encoding='utf-8-sig')
		>>> print(f.read())
		This is a test file.
		Second line in file.
		Adding third line to file
		>>>

Solution to the encoding error on windows console (command prompt) is to run this command:

```bat
	REM Activates UTF-8 code page
	chcp 65001
	REM OUTPUT: Activated code page: 65001
	
	REM Activates default code page (United States)
	chcp 437
	REM OUTPUT: Activated code page: 437
```

## Definition and use of functions

You can define a function using def keyword follow by any required parameters. The below shows a basic function.

		>>> def hello(name):
		...     print("Hello " + name + ", how are you today?")
		...
		>>> hello('david')
		Hello david, how are you today?
		>>>

This could be turned into a module. To do this, you would save the function to a file such as myModule.py. You then load the module using the import function.

		>>> import myModule
		>>> myModule.hello('Rifai')
		Hello Rifai, how are you today?
		>>>
