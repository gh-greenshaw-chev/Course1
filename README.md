# Python Course
<h3>Lesson 1 - Versions of Python, Hello World, Variables (Numbers, Strings and Lists), Operators</h3>

<h4>Versions</h4>
There are two main versions of Python, Version 2 and Version 3. We will be concentrating on Version 3, although most the statements will work on Python 2.
The notable exception is the 'print' statement, which requires brackets, as in 'print("hello world")', in Python 3, but you can get away with 'print "hello world"' in Python 2.

It is possible to write Python programs (also known as scripts) using a simple text editor, such as Notepad in Windows or nano in Linux, however, when Python is installed, it usually comes with an Integrated Development Environment (or IDE), known as IDLE. Some of the examples in these lessons will demonstrated  using IDLE. You can try out simple Python statements interactively in IDLE or create a new file and save it. Python programs should normally be saved with the filename extension of '.py'.

<H4>Hello World</H4>
Lets start with a single line program, that displays Hello World!
Open up the IDLE editor, it can usually be started with 'Python' or 'Idle'.
Enter:
>>>  print('Hello World!')
The three '>' symbols are already displayed by the editor.
When you press Return, the IDLE editor should display:
Hello World!
>>> 

If you exit the IDLE editor now, you would lose your one line program, so lets save it in a file.
Select 'File' from the IDLE menu, then select 'New File'
This should open a new window with a blank new file.
Enter:
print('Hello World!')
Then select 'File', then 'Save As' , navigate to the folder where you want to save your python programs, then enter the filename: 'hello.py' and press 'Save' button.
Now you can run this program by selecting 'Run', then 'Run Module'. You can alternatively use the short-cut F5 key.
This should also result in:
Hello World!
in the IDLE window.

<H4>Variables</H4>
Variables can be thought of as labels to areas of computer memory, where you want to store some values, temporarily, When your program finishes, those variables and the areas of memory will be discarded. If you need to keep those values, we need to write them to a file or a database - this will be covered later.

<H4>Variables and Types</H4>
Python is completely object oriented, and not "statically typed" like other languages.
You do not need to declare variables before using them, or declare their type. Every variable in Python is an object.

Variables can contain numbers or strings of characters or boolean values like True or False.
Numbers can be integers, like 1, 64, 1029 or floating point like 1.0, 63.99, 1234.5678.
Strings can be one or more characters, like "a", 'ABC', "The quick brown fox", enclosed in single or double quotes. If you start the string with a single quote you must end with a single quote, and similarly with double quotes. This means you can include quotes inside a string like: mystring = 'Batman "Zapped" the Penguin'.

Variable names must start with a letter (or an under-score '_') and can contain any number of other letters or digits or underscores.
For example: 'green=1', or 'Frog=99.3' or 'value100="chip"'. Note that the capitalization matters, for example 'Frog' and 'frog' would be two separate variables.

<H4>Numbers</H4>
Python supports two types of numbers - integers and floating point numbers
To define an integer, use the following syntax:
    myint = 7
    print(myint)
    
To define a floating point number, you may use one of the following notations:
    myfloat = 7.0
    print(myfloat)
    myfloat = float(7)
    print(myfloat)

<H4>Strings</H4>
Strings are defined either with a single quote or a double quotes.
    mystring = 'hello'
    print(mystring)
    mystring = "hello"
    print(mystring)

Simple operators can be executed on numbers and strings:
    one = 1
    two = 2
    three = one + two
    print(three)
    hello = "hello"
    world = "world"
    helloworld = hello + " " + world
    print(helloworld)

<H4>Exercise</H4>
The target of this exercise is to create a string, an integer, and a floating point number.
The string should be named mystring and should contain the word "hello".
The floating point number should be named myfloat and should contain the number 10.0, and the integer should be named myint and should contain the number 20.
    # change this code
    mystring = None
    myfloat = None
    myint = None

    # testing code
    if mystring == "hello":
        print("String: %s" % mystring)
    if isinstance(myfloat, float) and myfloat == 10.0:
        print("Float: %f" % myfloat)
    if isinstance(myint, int) and myint == 20:
        print("Integer: %d" % myint)

<H4>Lists</H4>
Lists are collections values, similar to arrays. But unlike most other programming languages, Lists can contain different types of values.
A list is created using the following syntax 'mylist=[]'. This will create an empty list, so if you 'print(mylist)' you will get '[]' indicating it is empty.
You can add items to the list using the append method, for example, 'mylist.append(2)' will add a new item '2' to the list. Add another item with 'mylist.append(1)' and another 'mylist.append("eggs")', then 'print(mylist)' will produce '[2, 1, 'eggs']'.
You can use any item in a list by referencing it by its index. The first index is always 0, so 'print(mylist[0])' would display 2.
The list can be referenced from the end by using the '-' sign, for example, 'print(mylist[-1])' would display 'eggs'.

<H4>Operators</H4>
Operators are symbols like '+', '-', '*' and '/', and are used to perform mathematical or logical operations on variables.
For example 'print(1+2*3/4.0)' would display 2.5. The reason for this is that there is a default order in which the operations are performed, i.e. First, Multiplication, Division, followed by Addition and Subtraction. So 2 multiplied 3 = 6, divided by 4.0 = 1.5, add 1 = 2.5.
You can force the order of the operations by using brackets, like 'print((1+2)*3/4.0)' would display 2.25, because the 1 and 2 and added together before being multiplied by 3.

Strings can be concatenated together using the '+' operator, so print("Hello" + " " + "World!") would display "Hello World!".

<H4>Exercises</H4>
Please try these exercises to test that you have understood today's topics:

1. What is wrong with this statement?     print("apples')

2. What will be displayed after these statements?
        apples = 5
        pears = 9.0
        bananas = 2
        grapes = 3
        print(bananas + apples * pears / grapes)

3. What will be displayed after these statements?
        primes=[1,2,3,5,7,11,13,17,19,23]
        magic=primes[4]+primes[7]
        print(magic)
