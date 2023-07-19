# Why Python is a MUST for Day2day Activities?
• Automation --> Python needs automation in business and day-to-day activities
• Data Visualization --> Plots and graphical representations.
• Data Analytics --> Analyse and understand raw data for insights and trends.
• AI and machine learning --> simulate human behavior and learn from past data without hard coding.
• Create web applications
• Handles databases
• Handles accounting to perform complex mathematical operations along with quantitative and qualitative analysis


## Python Variables
• Variables are containers
• Variable type does not need to be declared explicitly.

Example:
name = "Singam" #type str batch = 1.0	#type int
Job = True #type bool

Unordered list — Used to create a list of related items, in no particular order.
Ordered list — Used to create a list of related items, in a specific order

Scope of variable: Local/Global Variable:
def f():
#local variable
s = "DevOps course." print(s)
## Global variable s = "Python Data" f()
print(s)

## Data Types
## Sequenced data:
- list: A list is an ordered collection of data with elements separated by a comma and enclosed within square brackets. 
  Lists are mutable and can be modified after creation.

 list_data = [9, 2.9, [-3, 5], [”jenkins", ”Jira"]] print(list_data)
 Output: [9, 2.9, [-3, 5], ['jenkins', 'Jira']]

- Tuple
A tuple is an ordered collection of data with elements separated by a comma and enclosed within parentheses.
Tuples are immutable and can not be modified after creation

tuple1 = ((”cicd", ”Jenkins"), (” security", ”fortify"))
print(tuple1)
Output: (('cicd', 'Jenkins'), ('security', 'fortify'))

- Range
Returns a sequence of numbers as specified by the user. If not specified by the user, then it starts from 0 by default and increments by 1.

sequence1 = range(4,14,2) 
for i in sequence1:
print(i)
Output:4 6 8 10 12

- data: dictionary
A dictionary is an ordered collection of data containing a key: value pair. The key: value pairs are enclosed within curly brackets. No duplicated allowed

dict1 = {"name":"Devops", "project":1.0, "canVote":True,"name":"test"} print(dict1)

print(dict1["name"])

- Set
Set is an unordered collection of elements in which no element is repeated
info = {"test", 19, False, 5.9, 19} 
print(info)
{False, 5.9, 19, 'test'}


## Python Numbers/Operators 
- data type
• Int -> int1 2345698
• Float -> flt1 = -8.35245
• Complex -> cmplx1 = 2 + 4j

- Data Conversion -> Python allows data conversion
  num1 = 25
  num2 = float(num1)
  Output: 25.0

- Python Booleans
  print("Integer:",bool(23))

- Python Strings
  string is essentially a sequence or array of textual data.


## Strings
• Length of a String: Length of a string using len() function.
• String as an Array: String is essentially a sequence of characters also called an array.
• Loop through a String: Strings are arrays and arrays are iterable.
• String Methods: For Example str = ”jenkins”
• str.upper()
• str.lower()
• str.strip()
• str.replace(“Jen”,”Doc”)
• str.split(“k”)
• str.capitalize()
• str.find(”ins"))


## List Indexes
Item/element in a list has its own unique index.

ToolsData = ["Maven", "Ansible", "Jenkins", "Sonar"] 
CloudData = [”AWS", ”AZURE", ”GCP"]
Indexing : [0] [1] [2] [3]

Add list Items : ToolsData.append()
Insert list Items: ToolsData.insert(1,”Docker”)
Extend list Items: ToolsData.extend(CloudData) [ Add two lists, set, dict ] 
POP list items: ToolsData. pop() [#removes the last item of the list] 
REMOVE list items: ToolsData.remove(“Maven”)
Delete list items: del ToolsData[3]
Clear list items: clear():
 

EXAMPLE
 
ToolsData = ["Maven", "Ansible", "Jenkins", "Sonar"] 
if "Maven" in ToolsData:

print("Maven is present.") else:
print("Maven is absent.")

ToolsData.append("Fortify")
 
## List Comprehension

List comprehensions are used to create new lists from other iterables like lists, tuples, dictionaries, sets, and even arrays and strings.

Syntax:
List = [expression(item) for item in iterable if condition]

EXAMPLE
ToolsData = ["Maven", "Ansible", "Jenkins", "Sonar"]
names = [item for item in ToolsData if "o" in item] print(names)


## List Methods
• sort(): This method sorts the list in ascending order.
• reverse(): This method reverses the order of the list.
• index(): This method returns the index of the first occurrence of the list item.
• count(): Returns the count of the number of items with the given value.
• copy(): Returns copy of the list.

Conditional Statements if Statement
if-else Statement
elif Statement


## Python for Loop

- Iterating over string

name = 'Azizul' 
for i in name:
print(i)

- iterating over a tuple

tools = ("Maven", "Jenkins", "sonar", "jira") 
for x in tools:
print(x)

## While loop
count = 5
while (count > 0): 
print(count) 
count = count - 1
 
## NESTED LOOPS
i=1
while (i<=3):
#for loop will run till end 
for k in range(1, 4): 
print(i, "*", k, "=", (i*k)) 
i = i + 1
print()

for i in range(1, 4): 
k = 1
while (k<=3):
print(i, "*", k, "=", (i*k)) 
k = k + 1
print()


## Python Functions

Two types of functions:
built-in functions -> min(), max(), len(), sum(), type(), range(), dict(), list(), tuple(), set(), print(), etc.

user-defined functions -> Functions to perform specific tasks as per our needs.

EXAMPLE:

def toolname(security, analysis) 
    print("Tools,", security, analysis)
    toolname("Fortify", "Sonar")


## Function Arguments
• Default Arguments
• Keyword Arguments
• Required Arguments
• Variable-length Arguments

CASE 1
def name(fname, mtame = "Jenkins", boardname = "Jira"):
print("Hello,", fname, mtame, boardname)

name("Sonar")
CASE 2
def name(firsttool, secondtool, thirdtool): print("Hello,", firsttool, secondtool, thirdtool)

name(thirdtool = "Ansible", firsttool = "Terraform", secondtool = "Jmeter")
CASE 3
def name(firsttool, secondtool, thirdtool): print("Hello,", firsttool, secondtool, thirdtool)

name("Ansible", "Terraform", "Jmeter")
CASE 4
def name(*name):
print("Hello,", name[0], name[1], name[2])

name("Ansible", "Terraform", "Jmeter")


## Python Recursion
Function calling a function

Python Modules: These are the Python files that help us write the Python code easily.

Python Packages: Python packages are essentially folders that contain many Python modules. As such, packages help us to import modules from different folders.
  NumPy, SciPy, Pandas, Seaborn, sklearn, Matplotlib, etc.


## Python OOPS
Class means blueprint/template for creating objects.

self method: The self parameter refers to the current instance of the class and is used to access variables that belong to the class. It must be provided as the extra parameter inside the method definition.


## Python File Handling
file = open("someText.txt")
print(file.read())

Create a File: file = open("Text.txt", "x")

Write into a File:
file = open("Text.txt", "w") 
file.write(”New DevOps.") 
file.close

Read a File:
file = open("Text.txt", "r") 
print(file.read()) 
file.close

## Thank You! 
# Stay CONNECTED !!

https://www.youtube.com/channel/UCNwP7KEElaJ7cdDTLP-KbBg

https://www.linkedin.com/in/azizul-maqsud/

https://azizulmaqsud-1684501031000.hashnode.dev/

https://medium.com/@azizulmaqsud

https://twitter.com/Sohail2me

https://github.com/azizulmaqsud
