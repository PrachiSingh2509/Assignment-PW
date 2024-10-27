# Assignment-PW
#notes
-->operators in python:
var1 = "Ajay" #mem block wala concept repeat
when we want to manipulate data we want some operation and for that we use operators.
#python operators-Special keywords or symbols that are used to perform some operations on values or variables. 
Why? Because we want to manage, do computation and make decision using data.
a=2     
b = 3   
a+b #here + is operator which help to get the sum as 5.

a=3
b=2

1.Arithmetic operators
add = a+b
100-3
3*5
3-5
21/4 #Division
21 % 4 #Modulus
2**5 #This means 2 to the power 5
3**100

2. floor operator
2.33 can become 2 or 3
4/3 = 1.33 (But we want the nearest round value)
4//3 = 1 (Here, // is called as floor operator)

lower side ka value deta hai

3. Comparison operator
It compare 2 value >> compare >>return true or false.
2 == 2
2 != 2
5 != 2
10>3
10>=5
10<9
10 <= 14

4. Logical operator

It is of 2 types: and & Or
True - False
True and True

AND & OR operator truth table remember?
run all condition for AND & OR

5. not operator
not True #Output will be False
not False #Output will be True.


6. Assignment operator
a = 10 #We assigned value to a
a 

a + 5

b = 10
b = b + 10 OR, b += 10 # Both mean the same.



7. Membership operator.

a = "pwskills"
#We have to check if p is there in a or not?
"p" in a #Output will be True
"p" not in a #False


b = "Ajay"
"am" in b #False

#Membership operator says if some member is there in string or the container or not.


8. identity operator
It compares the location of two objects/variable in memory.
a = 2
b = 3
a is b #Is both referring to same memory block? No
a is not b


a = 2
b = a #This means b will also point to the same memory block.
a is b #True


9. bitwise operator
Operations at bit level(0 & 1), manipulating individual bits within integer.

#Bit wise representation = see ss
 
&, |, ~, ^, XOR
 10 & 10 #1010 & 1010 : 0&0=0, 1&1=1, 0&0=0, 1&1=1 , So result will be 10

18 & 3 #10010 & 00011: 00010 = 2

bin(18)

3 | 7

do some permutation & combination

#Negation
~3 #-3

#Bitwise xor operator.
represented by ^ cap or hat.
5 ^ 3  #o/p 6

#XOR work
  a b a^b
  0 0 0
  1 0 1
  0 1 1
  1 1 0
returns 1 when exactly 1 operand is 1.

HW: 2^6


10. Shift operator: left shift & right shift
Shift operator shifts the bit to the left/right by specified number of position.

Left shift << shifts the bit to left by no. of position by filling 0's on right.
35 << 3 
bin(35) # 10011
#35 shift by 3 means 10011000 (3 0's added to right) so value is 280
bin(280) #100011000


5 << 1 #10


right shift operator
280 >> 3 # 35
#remove the number of elements in the binary.
280 >> 3


11. Order of precedence
Execution of python statement will be from left to right
b = 5
b += 5 #first + then assign to b
b


2+3-8 #-3

#Always parenthesis will be prioritized else left to right calc.



---> Conditionals in python
Flow control:
1. conditional statements

#I will keep checking out the dishes in a buffet.
#Helps to code based on some condition.

-if:-
if condition True:
   block of code will be executed
-if-else :Two conditions 
-if-elif-else :Multiple condition, we can have multiple elif.
-nested-if else: You can have multiple if else inside if else.

x = 1
y = 6
if x > 5:
  if y > 5:
    print("hnhdbh")
  else:
    print("gew")
else:
  print("cdrfyth")

2. Loop statements

# I will keep checking out dishes until all dishes are over.

-for 
-while

3. control statement

#I will check out all the dishes until I get pasta.
-break
-continue

-->Input a number:-
a = input("enter a number:")
print("The number is: ", a)

type(a) #str
#Convert to int
a = int(input("gbyheio"))kmjii9



-->Loop statement: It allows you to execute block of code repeatedly.
Two types of loop: while & for

1. while loop:-

It repeatedly executes a block of code until a condition is met.
syntax: while->it is keyword
while condition:
  block of code to bee executed
Ex.
n = 7
i = 1
while i < n:
  print(i)
  i = i + 1 #O/P: 1 2 3 4 5 6 

Ex.
count = 5
while count>0:
  print(count)
  count = count - 1
#5>0 ->true = 5
#4>0->true = 4
...#0>0 false ->while loop break so O/P is 5 4 3 2 1


#We have else also with while.
Ex.
count = 5
while count>0:
  print(count)
  count = count - 1
else:
  print("This will be executed when the while loop run without any break.")


#Break statement in while loop:
n = 7
i = 1
while i < n:
  print(i)
  i = i + 1
  if i == 3:
    break
else: 
  print("This will be executed when the while loop run without any break.")

#break means come out of the loop, no need to do any execution of loop block after break is achieved.
#Break terminates / exits the loop. The condition is met it will break loop.
So O/P will be 1 2 and else block won't get printed.


#Continue statement
It skips the iteration.
Ex. 
n = 7
i = 1
while i < n:
  i = i + 1
  if i == 3:
    continue
  print(i)
else: 
  print("This will be executed when the while loop run without any break.")
#explaination:1<7 ->True -->No print
Now i = i+1 - 1+1 = 2
2 == 3-->False --> print 2
2<7-->true-->2+1 = 3--> 3 == 3--> True-->No print
3<7-->True-->3+1=4--> 4 == 3 -->False--> Print 4
... so o/p is 2 4 5 6 7 else_wala_line 


#For loop
Iterate over a sequence of elements. 
Strings, list are sequential data.
Ex.
for i in "pwskills":
  print(i)#O/P:p w s k i l l s

Ex. a ="Prachi"
for i in a:
  print(i)

Ex.
L = [1,2,"Ajay", "Prachi"] #This is list
for i in L:
  print(i)
O/P: 1 2 Ajay Prachi

for i in L:
  print(i)
else:
  print("This will be executed when for loop ends without a break statement")


#Break statement in for loop:
for i in L:
  if i  == "Ajay":
    break
  print(i)
else:
  print("This will be executed when for loop ends without a break statement") #1 2


#Continue statement in for loop:
for i in L:
  if i == "Ajay":
    continue
  print(i)
else:
  print("This will be executed when for loop ends without a break statement")
#O/P: 1 2 Prachi else_wala_line


#range
If I want to generate a sequence of element then how can I generate? So range is some code in python which will give you directly the range of values

ex.
range(0, 10) #It will give value from 0 to 9

Ex. list(range(0,10))

Ex. 
for i in range(10):
  print(i)

Ex. 
Ex. 
for i in range(10):
  print(i end=" ") )










####DATA STRUCTURES - MODULE 3

##LECTURE 1: OVERVIEW OF DATA STRUCTURES IN PYTHON:-


a = "Ajay" #Memory block wala concept. Here data is organised in sequential way so we can access the data also.
Similarly this happens in list.

DSA Definition and types. string, list, set, tuples, dictionary, array

--> List
#We can store anything in it. Stores heterogeneous data
#It is ordered collection of elements that can be of any type.
#It is mutable
#Rep: []

num = [ 1, 2, 3, 4, 5]
num
type(num)

#We already seen in previous module that access can be done using negative as well as positive index.

#If you are accessing an index which is not present then it will give error as list index out of range.

a = [1, a,True, (3+7i)]

#Adding element to the list:
a.append("orangr")

o/p: a = [1, a,True, (3+7i), 'orange']

(hit shift + tab to know functionality of append)


#Remove:
a.remove("orange")
o/p: a = [1, a,True, (3+7i)]

#We can also have list inside list
accessing element of list inside list:
lis = [[1,2,3], [4,5,6], [7,8,9]]
type(lis)
lis[0][1] #O/P: 2

#Iteration in list:
for i in a:
  print(i, end =" ")
#O/P: 1 a True (3+7i)


--> Tuples:
#It is immutable.
#Representation: ()

point = (2,3)
type(point)

#Why we need Tuple? Ex. Aadhar no., employee ID, account no., etc cannot be edited and we dont want to edit it, that is why we need a data structure which store data which cannot be edited.

#Tuple can also store heterogeneous data.

emp_name = ("ajay", Ajay1", "Bijay", "Sanjay")
type(emp_name)

emp_name.count("ajay") #Count of number of times o occurrence of ajay.



#If someone left the office then?

#We can access elements of tuple using negative as well as positive indexing.

emp_name[2] = "Rahul" #He joined at place of bijay but this wont get executed as it is immutable.
#So, we can access the elements but tuple is immutable.

#We can have tuple inside tuple:-
box1 = ("a", "b")
box2 = ("c", "d")
choc_bag = (box1, box2)
type(choc_bag)

choc_bag # o/p: - (('a', 'b'), ('c', 'd'))

#Iteration in tuple:
for box in choc_bag:
  for choc in box:
    print(choc)
O/p: a b c d


--> Sets:-
#It is unordered collection of unique elements.
#REpresentation: {}

s = {"red", "orange"}
type(s)

s = {"red", "orange", "red", "blue", "orange"}
s #O/P: {'blue', 'orange', 'red'}

#There are 5 elements in s but the duplicate elements are removed.
#There is no order of output so it is unordered collection of unique element.
#There is no concept of indexing as sets are unordered and unique.
s[0] #Error

#We can add element to a set.
s.add("Prachi")
o/p: {'blue', 'orange', 'red', 'prachi'}

#Mutable sets as we can add the element.

#We can remove also:
s.remove("prachi")
o/p: {'blue', 'orange', 'red'}

#Use case of sets>> To get unique elements


-->Dictionaries:-
#It stores the data in the form of key value pair.
my_dict = {}
type(my_dict) #O/P: dict

my_dict = {"key_course":"data_science","duration":200}
type(my_dict)

#Usecases:
phonebook = {"Dad":1234, "Mom":456}
phonebook

phonebook["Dad"]

#The index provide by python is replaced by key of the dictionary.


phonebook = {"Dad":1234, "Mom":456, "Dad": 780}
phonebook["Dad"] #Output will be the updated number: 780

#Change the value:

phonebook["Dad"] = "I don't want to give you."

phonebook
{'Dad': 'I don't want to give you.', 'Mom': 456}


#If you want all the values:
phonebook.values


--> Array
from array import array

#Array is similar to list>>Homogeneous data

array('i", [1,2,3,4,5])
O/P: array('i", [1,2,3,4,5])

-->String
s = 'Ajay'
type(s)

for i in s:
  print(i)

#String is immutable. We can access the elements.



##LECTURE 2: STRINGS

#String is a sequence of character which represents and manipulate textual data.
#Characters are represented using numerical values >>each character is assigned a unique value.
#There are ways to encode characters, so, here there are 2 ways:
Special characters converted to numbers
1. ASCII -> (American Standard Code for Information Interchange) (7 bits) ->2 to power 7 character can be represented Or it represent 128 character.
2. UTF -> Unicode(16 bits)-> 2 to power 16. It is huge as it almost covers every characters of every language.

UTF: Unicode Transformation Format.
There are 2 UTF: utf8 & utf16>>widely accepted.

#ASCII Representation:
char = "A"
ord(char) #It will give the ordinal of A in number. O/P: 65
#ord is ordinal, it will give numerical order of character.

chr(65) #It will give character for 65. O/P: 'A'
#chr is character, it gives the corresponding character to that number.

ord("a") #97


#UNICODE Representation
#Omega

'\u03A9' #O/P:OMEGA

'\u03A3' #O/P: SUMMATION

'\u0973' #O/P: HINDI KA A

#strings
string1 = "Prachi"
string1
type(string1)


'I'm a student'   #Error
#As it has one open single quote.

"I'm a student"  #CORRECT

"I"m a student"  #ERROR


#To avoid this error you can use ''' OR """

"""I'm a student"""

'''I'm a student'''


'''I'm a student
I'm a student
I'm a student
'''  

#In output it will show \n and this represents a new line.

#Concatenation of string>>Combination of two strings

"Hello" + "WORLD"
#O/P: 'Hello WORLD'

#We only use + sign for concatenation.

string1 = "Prachi"
string2 = "Hello"
string1 + ", " + string2


#Extract sub part of string : slicing
a = "Ajay" #indexing u know , now we will slice it
a[0]

a[-1]

a[4] #Throw an error that 4th index doesn't exist.


string1 = "I am a good student" #Here index, I=0, space = 1, a=2, m=3,etc
string1[0:3]	 #O/P: 'I am' 
Here 3 is exclusive, [a,b] >>It will give result till b-1 index.


string1[0:] #start index : end_index-->If you not provide end index, it will be default give substring till the last index.

string1[3:]

string1[:-3]

string1[-3:]


#By default it has step value of 1.
#It is similar to range function
#We can have step 

string1[0:5:2] #here 2 is the step to be skipped.


string1[::1]

string1[::2]

#steping is from left to right

string1[::-1]#Here string is reversed. Iterate over the sequence in reverse order.
#It means start from the end, move to the beginning and step backward by one character.

#Strings are immutable.

#number of characters in the string
len(string1)


#String can be modified although it is immutable.
We can replace the substring
#Modification of string
s = "I am a student"
s[0] = m #error
s.replace("old_substring", "new_substring")
s.replace("student", "teacher")


#Use case
address = "123 suhana apt, marathalli, Banagalore"
address.replace("apt", "apartment")


#lower and upper case
text = "Hello"
text.lower() #O/P: hello
text.upper() #O/P: HELLO

text.title() #1st letter capital

text.swapcase()#Convert upper case to lower case and vice versa.
#hELLO

text.capitalize() #Makes 1st letter capital and other small.


#String searching
sentence = "I am prachi"
"am" in sentence

#Use case:
search_word = "am"
if search_word in sentence:
  print("Good")
else:
  print("bad")

#In email also like it is manadatory to have @ in email else not valid


#String comparison
str1 ="hello"
str2 = "hello"
str1 == str2 


str1 ="hello"
str2 = "Hello"
str1 == str2 

str1 ="hello"
str2 = "hEllo"
str1.lower() == str2.lower()


SEE SS

#String ordering
name = ["Ajay", "sanjay", "bijay"]
sorted(name)


#Common string operations:
input_str = "         Prachi"
input_str

input_str.strip() #All white spaces removed.


#String splitting
data = "Ajay. data science, teacher"
data

info = data.split(',') #Based on separator provide in '' it will have number of elements.

info


name = info[0]
sub = info[1]
des = info[2]


#Escape sequences
These are special combination of characters used within a string.

address = """123 suhana apt,
 marathalli, 
Banagalore"""
#O/P: '123 suhana apt,\nmarathalli, \nBanagalore'
It means python understands new line.

print(address)

address = """123 suhana apt,\nmarathalli, \nBanagalore"""
print(address)


#\n >> To insert a new line character

#\t escape character >> tab
table = "Name\tAge\tGrade\nAjay\t21\nBijay\t22\tA+"
print(table)


#File path printing
file_path = "C:\\USERS\\DOWNLOADS\\FILES.txt"
print(file_path)
#C:\USERS\DOWNLOADS\FILES.txt
#\\ this is escape character for path

#\' Single quote escape
str1 = "I can\'t believe"
print(str1)

#Carriage return \r>>Moves the cursor to the beginning of line
print("Hello, I am \rAjay, I am going to Delhi")
#O/P: Ajay, I am going to Delhi
Jahan se \r hoga waha se print ho jaega.


#String formatting
print("My name is Ajay")
print("My name is Bijay")
print("My name is Sanjay")

#O/p: 

Creating string with placeg=holder for variables:
name = "Ajay"
greetings = f"hello{name}, how are you?"
print(greetings)

OR,
name ="Prachi"
greeting = "Hello %s, wish you luck"%name
print(greeting)


#Format
template = "Hello, {} welcome to {}
message = template.format('ajay", "Data science")

# OR ke baad wala old approach hai and lengthy hai so isliye naya approacha aya.



#f string (Formatted string literals)

course = "Pw data + frontend"
duration = 4
f"My course is {course} and its duration is {duration} years.


Celsius = 30
f"{celcius} is equals to {(Celsius * 9/5)+32}F"


str1 = "Prachi"
str1.startswith("Pra")

#True
str1 = "Prachi"
str1.endswith("lly")#False


#Check if string is alphanumeric or not
a = "123abc"
a.isalnum()

a = "123"
a.isalnum()

a = 123
a.isalnum()


s = "Prachi"
count = 0
for i in s:
  print(i)
  count = count+1
print(count)





##LECTURE 2 : LIST

gl = ["Milk", 1, 3+5j]
type(gl)

#Innitial introduction part already studied.

#Adding value in list
lis = ["Apple", "Orange"]
lis.append("Banana")
lis #O/P: ["Apple", "Orange", "Banana"]

#List is mutable

lis[0] = "mango"
lis

#inserting element before index:
lis.insert(1, "Potato")
lis


#extend: Used to append elements from another list
my_list = ["Apple", "Banana", "Orange"]
brothers_list = ["brinjal"' "potato"]
my_list.extend(brothers_list)
my_list

my_list + brothers_list #It will create a new list and won't extend the original list


#Repeatation operation
"*" * 15
"-" * 10
[0] * 10
[1,2,3] * 5

list(range(10)) * 3


msg = "i am bad \n"
print(msg * 3)


#Membership in, not in
gl
"milk" in gl
"POTATO" not in gl

#DEEP COPY AND SHALLOW COPY

1. Shallow copy: Since both list pointing to the same location, so if you are updating one list the other will also get updated.
Suppose, list1 = [A, B, C]
list2 = [1,2,3]
list1 & list2 both are pointing to same  memory location. 
list1 = list2
if you change list1 = [4,2,3]
list2 will also get changed as, list2 = [4,2,3]

#Value will change with change in other list
a = gl
a
gl
a[0] = "Prachi"
gl #This is also updated


2. Deep Copy: If you make change to one copy then it will not reflect on other.


#Sorting of list
book_list = ["Data Str", "Algorithm", "web", "Algorithm"]
sorted(book_list)

Now I want to know index of algorithm
book_list.index("Algorithm") #Returns the index of first occurrence

len(book_list) #No. of elements in book_List

book_list.count("Algorithm") #count gives the count of a specific element in a list

book_list.remove("Data Str")

book_list.sort()

del book_list #book_list variable has been deleted



book_list = ["Data Str", "Algorithm", "web", "Algorithm"]
#I want to del element inside the book_list
book_list.clear()



book_list = ["Data Str", "Algorithm", "web", "Algorithm"]
#I want to del last element
book_list.pop() #By default if you do not pass anything in pop(), it will remove last element


#List comprehension
prices = [10, 20, 30, 40, 50]
doubles_price = []
for i in prices: 
  doubled_price.append(i*2)
doubled_price

OR,
For writing the same 4 line of code in single line :-

[price * 2 for price in prices] #Same output as 4 line wala code

names = ["ajay", "kanak"]
[name.capitalize() for name in names]


str1 = "doc1.ppt"
str1.split(".")[-1]

file_name = ["soc1.ppt", "doc2.pdf", doc3.jpg, "doc4.py"]
[file.split(".")[-1] for file in file_name] #O/P: ['ppt', 'pdf', 'jpg', 'py']



#Conditional list comprehension
email_addres = ["aj@gmail.com", sj@yahoo.com",cjdscn@gmail.com"]
[email for email in email_addres if email.endswith("@yahoo.com")]


#Nested list comprehension
for x in [1,2,3]:
  for y in [4,5,6]:
    pairs.append([x, y])

OR We can do it in nested list comprehension

[[x, y] for x in [1,2,3] for y in [4,5,6]]




#List as stack and queue(Optional)
1. stack
image hai ek push pop wala stack ka concept bataya.
LIFO principle
It has 1 end

stack_of_plates = []

stack_of_plates.append("plate1")
stack_of_plates.append("plate2")
stack_of_plates.append("plate3")
stack_of_plates.append("plate4")
stack_of_plates

stack_of_plates.pop() #Last plate will be removed 1st


#use case
You have browsing history, when you press back button it will pop out last page.


2. Queue
Queue ka concept samjhaya.
FIFO 
It has 2 end.
It works in orderly sequential manner.
enqueue-->back   front--> dequeue
In python we have library to do this.

Library is needed to have reusable code.
library is the collection of multiple python scripts(modules) for reusing the code.

Implementing enqueue and dequeue

from collections import dequeue
#collections here is a library and dequeue is module.
checkout = deque()#Object made for the class
checkout.append("cust1")
checkout.append("cust2")
checkout.append("cust3")
checkout.append("cust4")
checkout.append("cust5")
checkout

while checkout:
  customer = checkout.popleft() #Pop from left side
  print("Serving", customer)


from queue import Queue
print_queue = Queue()
print_queue.put("Print the 1 pdf") #put is similarto psh
print_queue.put("Print the 2 pdf")
print_queue.put("Print the 3 pdf")
print_queue.put("Print the 4 pdf")
print_queue.put("Print the 5 pdf")
while not print_queue.empty():
  print_job = print_queue.get() #get is similar to pop
  print("printing", print_job)

 


##LECTURE 2 : TUPLES AND SETS

1. TUPLES

#Tuples are orderedcolection of elements, heteroeneous
#Intro you alrady know.

emp_name = ("ajay", Ajay1", "Bijay", "Sanjay",1,1,1,5)
emp_name.index("ajay")

print(emp_name * 2)

#Slicing in tuple
emp_name[0:4]


emp_name[::-1]

#iterate n tpe
for i in emp_name:
  print(i, type(i))


t1 = (1,2,100, 0, 200)
max(t1)
min(t1)

t2 = (101, 201)
t1

t3 = (t1,t2) #Nested tuples
t3
type(t3)

#Del ar t3
del t3
t3 #error

#Length of t1
ln(t1)

#membership operator
1 in t1

'ajay' in emp_name

t1

t2

#combine bot tuple
t1 + t2


2. SETS
Sets are unordered and unique collection of elements.
It doesn't allow duplicate elements 
Unordered, indexing will not work.

s = {1,2,3,4}
type(s)

s = {1,2,1,2,2,"Ajay","Ajay","Ajay","Ajay","ajay","ajay"}
s

#Use case
#Converting list to a set
list1 = [1,2,3,"Brinja","Brinja", "Apple", "Apple"]
s = set(list1)
s

#Convertig set to list
list1 = list(s)
list1

s[0] #Error as set object is not subscirptable.
s[1]


s = {1,1,2,3,3,4}
s

s = {1,2,3,4,5,{4,5,6}} #Error as unhashable type: set
#Immutable data structure has a stable hash value. (Hash is some sort of encoding). The immutable data structure has a stable hash values like tuples.
#unhashable type >>It is mutable-list, set

#Set inside set must be immutable
Unhashable type means it is mutable.
list , set are mutable so we will get the error

{1,2,3,4,5,(4,5,6)} #It will not throw error as it is tuple(immutable)

s[0] #Error as not support indexing, slicing


#iteration

for i in s:
  print(i)


#Set is mutable
s.add(100) #We can add element. It is not compulsory that the element will be added to the last of set.

s.pop() # It is not necessary that it will remove the last element.


s.remove(100) #It will specifically remove 100. It wremoves element specifically unlike pop.

s.pop(4) #It will throw error as it is not specific to the element.


s.remove(102) # It will throw an error as 102 is not there in the set.

#Update set
s.update("Ajay")
s #It will add individual character {'A'.'a', 'j','y'}
#So updates take iterable
#Write like this:
s.update(["Ajay"])
s

#Update an integer
s.([2,3]) #If 2 already there then not update 2. Also for integer you have to update like this else it will throw an error.
s

#Set can have multiple data structure.
s = {(1,2,3), 100, '2', 3.4}
type(s)

s.clear() #We will get empty set.

del s #Set s will be deleted.


#Remove an element
s = {(1,2,3), 100,101,  '2', 3.4}
s.remove(101)

s.remove(110) #Throw error as not present

s.discard(100)
s

s.discard(110)
s # It will not throw error even if element is not present.

#Set operations
(I)Union: All elements from both set
(II)Intersection: Common elements
(III)Difference: Present in 1st set and not in 2nd.
(IV)Symmetric difference: It returns all the elements other than common elements.

s1 = {"hiking", "Reading", "Coding"}
s2 = {"Coding", "Photography", "Travelling"}

s1 | s2 #union
s1 & s2 #Intersection
s1-s2 #Difference
s1 ^ s2 #Symmetric difference.

#Frozen set
s = {1,2,3}
s.add(100) 
s 
We have already seen that. Sometimes you don't want the set to be mutable. So python have concept of Frozen set.
#Frozen sets>>Immutable version of set, cannot be added or removed any new element.

my_fs = frozenset([1,2,2,2,3,3,4,5})
my_fs
Type(my_fs)

#we can not add or remove element
#It is used in case when you have duplicate values bit you want to fix the unique values of the data.




##LECTURE 2 : DICTIONARY

#It is a data structure that stores the data as a key value pair.
#Keys are unique and immutable.
#Note: Dictionaries are unordered but from python 3.7 version, dictionaries retain the order of insertion.
#This means that if you iterate over a dictionary, the items will be returned in the order they were added.

d = {}
type(d)

d = {"name":"Ajay", "Email"::ajay@gmail.com", "Contact":1234}
d #key:value pair

type(d)

#How do dict store data?
key value pair

list = [1,2,3,4,5]
uk how data store in list and can be accessed by indexing so similarly we can access data of dictionary by key.

d['name']
d["email"]


#updating
d['name'] = "bikay"
d


d = {"address": "26th cross, banagalore"}
d["address"]


d = {"key":1}
d["key"]

#Can you access key using pair? No. error will be thrown. vice versa is not possible.

#Web can have, integer, float, Boolean, tuple, etc as key.
#we can not have #, @, list, set, dictionary, etc as a key. 
#Hence only strings and numbers can be used as key of the dictionary.


d = {"name":"Ajay", "Email"::ajay@gmail.com", "Contact":1234, "name": "Bijay"}
d #in name, bijay will be updated.
#always the last key's value will be used.

#Value as a list, tuple
d = {"name": ["Ajay", 'Sanjay', 1, 2], "Email"::ajay@gmail.com", "Contact":(1234, 678)}

d['name'][1] #accessing element.

#Adding a new key value pair in d
d["address"] = "Bangalore"
d

#Delete the key value pair
del d["address"]

#Delete whole dictionary
del d

d#Error


#Empty dictionary
d = {"name":"Ajay", "Email"::ajay@gmail.com", "Contact":1234, "name": "Bijay"}
d.clear()
d

#Length of dictionary
len(d)


#Access keys
d.keys()

#Access value
d.values

#Copy dictionary
d1 = d.copy()
d1

#We can del d1 and d can still be there

#Using pop() to remove pair
d.pop("contact")

#Updating d with adding elements of d1
d1 = {"course": "ds"}
d.update(d1)
d

#Same thing to access the element we can use .get()
d["name"]
  OR
d.get("name")
d

#from keys()
It creates a dictionary from any iterable.
d.fromkeys((1,2,3),("a","b","c")) #1,2 and 3 will be treated as keys and (a,b,c) will be value for each one of them.
d


#zip function
students = ["arun", "Ajay", "Bijay"]
marks = [80,95,100]
#Zip() will put both values together one by one
for i in zip(students, marks):
  print(i)


#store the above info in key value pair>>dict
students = ["arun", "Ajay", "Bijay"]
marks = [80,95,100]
student_marks = {}
for student, mark in zip(students, marks):
  student_marks[student] = mark

student_marks


#Dictionary comprehension
we can do above thing easily using this

students = ["arun", "Ajay", "Bijay"]
marks = [80,95,100]
{student:marks for student, marks in zip(students, marks)}



Ex. 
user_id = [1,2,3]
user_name = ["a21", "a22", "a23"]
user_id

user_name

{u_id:u_name for u_id, u_name in zip(user_id, user_name)}

#if you want to see all key value pairs 
dict_name.items()


#Iterate (Both key and value)
for key, value in d.items():
  print(key, value)

#Iterate only keys
for key in d.keys():
  print(key)

#Iterate only valuess
for value  in d.values():
  print(value)













####FUNCTIONS - MODULE 4

##LECTURE 1: FUNCTIONS:-


#Inbuilt function:

type(5)
#functions>> print, len, type>>inbuilt python function.
#ceiling function: gives nearest highest value. ceil()
#floor() >>It gives nearest lowest value.
floor & ceil gives whole number value.

#importing library:

import math as m #math(library) is a collection of function
m.ceil(6.5) #7
m.floor(6.5) #6


#User defined function:

#syntax
def func():
  #do something>> Body of function

#function is a block of code which performs some specific task/computation.

#Why function? Functions are reusable.; code remains neat and clean.; organized.; saves time.


#Ex. greeting
def greet():
  print("Welcome to the office")

greet()
#Variable inside the function
#Ex. greeting with name
def greet(name):
  print("Welcome to the office", name)

greet("Ajay")
#If you don't provide name then it will throw an error as positional argument.

#
def greet(name):
  print("Welcome to the office", bijay)
greet("Ajay") #O/P: Welcome to the office Ajay


#Ex. 
def func():
	print("This is my first function")


#concatenating strings
"This is my first function" + "in Python"

#other way to concatenate
func() + "in Python" #It will throw an error. As null + string cannot be combined.

type(func()) #non type



#Return

def func():
	#do something here
	return "This is my first function"
func() + "in Python" #Now this will give the concatenated output.


Summarize:
1. def
2. name of func
3. variable you want to pass
4. return statement.


#Ex. 
def funct():
	return "This is that", 1, 2.2, True, 3+7j

funct() #Return tuple

a=funct()
type(a)#Tuple


#ex.
a, b, c, d, e = funct()
a #"This is that
b #1
c#2.2
d #True
e #3+7j
#If you give only 4 values (a, b, c, d) and function has 5 values then it will return error

OR
a[0]
a[1]



#Ex. 
def func():
	calc = 2+3+6+5
	return calc

func()

type(func()) #Int


#Squre of number
def square_no(a): #a is called as an argument
	return a*a

square_no(5)


#Do sum, sub, div of number. int, list, tuple etc

#Positional arguments: The order in which you will provide the argument , in the same order it will be printed. 

def add(a, b):
	return a+b
add("P", "w")

add("w", "p")

#a and b are positional arguments>> it maintains order

#Assign >> if I want to keep w as b and p as a
add(b = "w", a = "p") #This is correct


#Sum ex.
def sum1(a, b, c):
	return a+b+c
sum(1,2,3)

#Suppose if I dont give value for a variable in add() then it will throw error but we can avoid it by assigning 0 as, when there is no value for that variable it will consider it as 0.
Note: It is called as default argument and default arg. should pe put at last, if we don't do so then error will occur.
def sum1(a = 0, b, c):
	return a+b+c #Throw error


Ex.
def sum1(b, c, a = 0):
	return a+b+c
sum1(b = 1, c = 2)


#We can have all var as default arg.
 
def sum1(b=3, c=0, a = 0):
	return a+b+c

sum1
sum1(1) #O/P: 1 as it will take value of b as 1.


sum(c = 1) #O/P: 6


Ex.
def add_two_number(): #Before we used to pass two variables
	a = int(input("enter the 1st no: "))
	b = int(input("enter the 2nd no: "))
	return a+b

add_two_number()


Q. Write a function that takes  list as input and return all numeric values in a list.

solution:

def only_num(a):
	n = []
	for i in a:
		if type(i) == int or type(i) == float:
			n.append(i)
		return n

only_num([1, 2.2, "Ajay", True, 3+7j, "pwskills"])


#Now in input take nested list
only_num([1, 2.2, "Ajay", True, 3+7j, "pwskills", [100, 101, "Bijay"]])

we need to update the code:
def only_num(a):
	n = []
	for i in a:
		if type(i) == list:
			for j in i:
				if type(j) == int or type(j) == float:
				n.append(j)
		else:
				if type(i) == int or type(i) == float:
				n.append(i)
	return n



#Example: we can have multiple arguments : Variable length arguments
When you dont know number of arguments. For this, python says just put * before any arg.

def sum1(*args):
	return args

sum1(1, 2,3) #will return tuple


#define it for iteration of sum.
def sum1(*args):
	sum = 0
	for i in args:
		s = s+i
	return s

sum1(1,2,3,4,5,6,7,100)


#variable argument with default argument
def test(*args, a):
	return args, a

test(1,2,3,4) #error. You have to pass the value for a.

def test(*args, a = 100): #So, you must pass any value in the var arg.
	return args, a
test(1, 4, 18, 29)


#Variable argument >> takes any no. of argument
#Positional arguments >> fixed arguments


Q. Write a function can take any no. of values and returns the list
Solution:
def val(*args):
	l = []
	for i in args:
		if type(i) == list:
			l.append(i)
	return l

val(1,2,3.2, {2,3}, [1,2,3,4,5], (2,3), True, "Jaya")
#O/P: [1,2,3,4,5]


#example:
def team(name, project):
	return f"{name} is working on {project}"
#Variable length argument and keyword argument together
def test1(*args, **arg1):
	return args, args1

test1(1, 2, 3, 4, a=100, b = 50)
test1()



#Python namespace
def greet():
	message = "Hello, welcome!" #This is a local variable, local to function.
	print(message)

greet() #O/P will be correct and come

print(message) #Error, as message is local variable, scope is only inside the function.


 
Example:
subpart = "to the course" #Global variable, it can be accessed outside the function as well.
def greet():
	message = "Hello, welcome" + subpart
	print(message)

greet() #O/P will come.


#Local var>> A function defined inside the function should be accessed in the function only.
#Global var>> Accessed anywhere


#Function inside function
ex.
def marks(**kwargs):
	#Summation of all arg
	marks_list = []
	for sub, mark in kwargs.items():
		marks.append(mark)

	return marks_list

ex. now writing func in func
def marks(**kwargs):
	def total_marks(marks_list): #Local
		return sum(marks_list)
	marks_list = []
	for sub, mark in kwargs.items():
		marks.append(mark)

	return total_marks(marks_list)

sum([90, 20])


#A function can be called inside the function
#But, always call function from outside


#Calling function from outside

def total_marks(marks_list): #Global
	return sum(marks_list)

def marks(**kwargs):
	marks_list = []
	for sub, mark in kwargs.items():
		marks.append(mark)

	return total_marks(marks_list)




#Example:
def find_power(num, power):
	return num*power
find_power(2, 50)

#For big projects these small function may get mixed up or confuse so always write description.

#Best practice for industries: For writing description, use docstring ("""    """)
def find_power(num, power):
	"""This function returns the power of no.
	Args:
	 num(int): Provide any integer as input
	 power(int): Provide power as integer
	Returns:
	 integer: Power of no.
	"""
	return num*power
find_power(2, 50)





##LECTURE 2: ITRTORS AND GENARATORS:-

Ex.
for i in "Prachi":
	print(i) #uk output

Ex.
for i in 5:
	print(i)#Error


#Iterable is any python object/sequential structure/data structure that is capable of returning its members one at a time.
#Permitting it to be iterated over in a for loop
#Example>>List, tuple, etc

Ex.
lis = [1,2,"Ajay"] #List is an iterable object
for i in lis:
	print(i)

Ex.
for i in 6:
	print(i) #Error

#Iteration: It is a process of looping through the elements of an iterable(ex. list, string) and this is done using a loop.
#The process of returning element one by one is iteration.
#Iterator: An iterator is an object representing a stream of data>>return the data one by one.

#analogy
#potato(iterable) >> it cannot be cooked in original form. If you chop/wash the potato, then it is ready for cooking >> iterator. The process of cooking is iteration.

for i in s:
	print(i)

#How python decided that s should be iterated?
#Python says >> can I prepare s for iteration?
iter(s) #iterator object

#So, we checked that s is ready to be iterated.


next(p)
next(w)
next(s)
next(k)....This is iteration only.


for i in "pwskills: #First converting the iterable string to iterator object(using iter) and then access using next()
	print(i)


l = iter([1, 2, 3, 4])
l

next(l)
next(l)
next(l)
next(l) #Error as no element left in l



d = iter({"name":"Ajay"})
d
next(d)

#We are studying this because we have to use it in generator function.


#Generator Function :-
#Regular func: takes a list and gives square of each of the list.
def sq_no(n):
	result = []
	for i in range(n):
		result.append(i ** 2)
	return result
sq_no([5, 10, 16])
#Regular function calculates the square of the values and return in one go. Since it is returning in one go, for that point of time the memory usage will be more and if you provide bigger number then it will take a lot of execution time.

#Can we have something to generate result one by one instead of one go? Yes, using yield()
#Yield is a general function uses return statement but a generator function use yield statement

def square_number_generators(n):
	for i in range(n):
		yield i**2

square_number_generators(10) #It is an generator object. Yield is creating a generator similar to iterator object.

gen = square_number_generators(10)
gen

next(gen)
next(gen)
.
.
.
.


Ex. You remember range(). If you only write
range(1, 10) #Will not give value. But if you write,
for i in range(1, 10):
	print(i) #It will give value


#Fibonacci series: 0 1 1 2 3 5 8 13....
def fib(n):
	a = 0
	b = 1
	for i in range(n): #if n = 5,0,1,2,3,4
		yield a #a is 0, so give value of a.
		a, b = b, a+b #1, 1, 2
f = fib(100000000)
f
next(f) #0
next(f) #1
.
.
.
.





#LECTURE 3: LAMBDA, MAP, REDUCE AND FILTER

#Lambda function: It is also called as anonymous function or short hand function

syntax:
lambda argument: expression

#No need of return statement and def keyword

Ex.
sq_lambda = lambda x: x**2
sq_lambda(2)

Homework:  Do addition, even odd

Ex. 
x = ["Python", "DS", "Ajay"]
x

sorted(x) #By default sorting based on alphabetical order

#Now, sort the list based on length of element of List
#We use length function to know the length
le = lambda x: len(x) 
le("Ajay")

#so complete code is pass this lambda length function in sorted.
sorted(x, key = lambda x: len(x))

#Fibonacci series using lambda function
fib = lambda n: n if n<=1 else fib(n-1) + fib(n-2)
[fib(i) for i in range(10)]


#Factorial of 5: 5! = 5x4x3x2x1
Approach1:
def fact_num(f):
	if f==0:
		return 1
	else:
		return f*fact_num(n-1)
fact_num(6)

Approach 2:
fac = lambda f: 1 if f==0 else f*fac(f-1)
fac(5)


##MAP 

#Def: Executes a specified function for each of item of an iterable.
#Syntax: map(func,*iterables)

Ex. Approach1
l = [1, 2, 3, 4, 5]
def square(l):
	sq = []
	for i in l:
		sq.append(i**2)
	return sq
square(l)


Ex. Approach2 :By map function
def sq(x):
	return x**2

l
 
list(map(sq, l)) #map(func, iterable)



Ex. addition in l
def add(x):
	returnx+10
list(map(add, l))


#Using lambda with map
list(map(lambda x: x**2, l))


list(map(lambda x: x+10, l))

Ex. converting string to integer
l = ["1", "2", "3"]
list(map(lambda x: int(x), l))

Ex. Adding corresponding elements of 2 lists
l1 = [100, 200, 300, 400]
l2 = [1, 2, 3, 4]
list(map(lambda x, y : x+y, l1, l2))

Ex. uppercase
s = "pwskills"
list(map(lambda x: x.upper(), s))

Ex. Makng first letter of a word capital.
words = ["Python", "ajay"]
list(map(str.capitalize, words))


Ex. 
grades = ["A", "B", "C", "D"]
list(map(lambda grade: 4 if grade == "A" else (3 if grade == "B" else 2), grades)


##REDUCE:

#Reduce means folding or reduction
#Syntax>> reduce(func, itrable)
#import library
from functools import reduce

l = [2, 1, 3, 4, 4, 5, 6]
reduce(lambda x, y:x+y, l)
# 2+1; 3 is and3 is y= 3+3; 6 is x and 4 is y= 6+4;....25

#Reduce will always take 2 argument function.
Reason:

l = [2, 1, 3, 4, 4, 5, 6]
reduce(lambda x, y, z:x+y+z, l) #Give error as missing 1 argument z as it is not compatible for z. If suppose one no. inc. in l then how you will bring z?


That's why reduce takes only 2 functions.
#Empty iterable cannot be there
reduce(lambda x, y:x+y, []) #Error

#One arg is fine
reduce(lambda x, y:x*y, l)


Ex.
words = ["Data", "Science", "courses"]
reduce(lambda x, y: x+ " "+y, 












####OOPS - MODULE 5

##LECTURE 1:- OOPS(Object oriented programming system)

a = 5
a

type(a)
print(type(a)) #O/p: class integer

#What is this class?
This concept of class comes from oops

Ex. YOU HAVE secured good rank in IIT(AJAY)-->IIT will give a form to fill and ajay will fill it. Rahul also asks for the form and IIT gave him the xerox form...so similar for other students too. IIT will never say that there is no original form they will give xerox form which can be called as template. So master template T have many T1, T2, T3, etc. This original "template" is called as "CLASS". The "xerox" of T is called "OBJECT".
Each template has (name, percentile, rank ) and this is called as "PROPERTY/ATTRIBUTE" of the template.

#Classes are blueprint / template for creating an object.

#So, class int is a template and a=4, b=3 are the objects of template integer.
#We are different objects of class human being.

#class car is nothing but a template.
#Concept of defining a class.
class Car: #naming convention>> UpperCamelCase
	pass
c1 = Car() #instance/ object
print(type(c1))


#We already have functions then why oops?
Ans.: If u r working on big project and there are multiple functions def f1, def f2, def f3, etc . So project has many components backend(f1, f2) and so on

def f1():
	pass
def f2():
	pass
def f3():
	pass
and so on.

#Now, if a backend developer wants to work/ change some backend functions>> all the functions are mixed and it is not in a arranged manner so it becomes difficult tp pick the correct function
#OOPS helps you to arrange the required functions in respective classes. Ex frontend func in that class same for backend and etc.

Ex.
class Car:
	pass
c1 = Car()
print(type(c1))


class Car:
	def accelerate():
		print("Car is accelerating")

c1 = Car()

c1.accelerate() #It will throw an error.why?
#It is because --> Car(class) or gujiya maker machine--> c1(object) or materials for gujiya maker-
- > accelerate(method) OR different gujiyas must differ in taste. So similarly, accelerate is not able to identify whether it is the method for c1, c2 or which type/number of car.
To resolve this issue we use "self" keyword in accelerate which depicts that this car belongs to you(For each object/c1, c2...)


class Car:
	def accelerate(self):
		print("Car is accelerating")

c1 = Car()
c1.accelerate() #O/P: Car is accelerating

c2 = Car()
c2.accelerate() #O/P: Car is accelerating

#self>> It is a variable that represent instance of the class using which you can access method/function of the class, also attribute/ property/data of the class.

#self makes sure that each object knows that the method is associated with it or in other words the method is referenced to that particular object.

#Self>> It is just a convention, you can also pass ajay, rita, etc any name in place of self and then also you will get the same output. Self is not a python keyword you can pass any variable but best practice is to pass self.


#Ex. car can have break or deaccelerate also
class Car:
	def accelerate(self):
		print("Car is accelerating")
	def brake(self):
		print("Car is stopping")

c1 = Car()
c1.accelerate()

c1.brake()


#Ex. bank deposit
class Bank:
	def deposit(self):
		print("I am depositing the money")
	def withdraw(self):
		print("I am withdrawing the money")

c1 = Bank()
c1.deposit()

c1.withdraw()

c2 = Bank()
c2.deposit()


Ex.
#Passing data in the class>> can also be called as property/attribute.
class Bank:
	def deposit(self, amount):
		print("I am depositing the money")
	def withdraw(self, amount_withdraw):
		print("I am withdrawing the money")

ajay = Bank()
ajay.deposit()#Throw an error

ajay.deposit(1000)# correct

ajay.withdraw(500)


Ex. bank will ask for a default amount
#Amount is attribute/property/data of class Bank.
class Bank:
	amount = 1000
	def deposit(self, amount):
		print("I am depositing the money")
	def withdraw(self, amount_withdraw):
		print("I am withdrawing the money")	

ajay = Bank() #Ajay is our customer
ajay.deposit(1000)

#Attributes/property can also be accessed the same way as methods/ functions are accessed.
ajay.amount


#Making instance of a class
Ex. Extract odd and even numbers from a list.

class ListOps:
	l = [1, 2, 3, 4, 5]
	def extracr_even(self, l):
		l1 = []
		for i in l:
			if i%2 == 0:
				l1.append(i)
		return l1
	def extract_odd(self, l):
		l1 = []
		for i in l:
			if i%2 != 0:
				l1.append(i)
		return l1

ops1 = ListOps()
ops1.l

ops1.extract_even(ops1.l)

ops1.extract_odd(ops1.l)

ops1.extract_even(ops1.l)

ops1.extract_odd([8, 11, 12, 14])

#if you make any object the attribute l is fixed
#Inspite of passing a different list above you are still getting the fixed l([1, 2, 3, 4, 5])
ops1.l

#I want to take the attribute value of the class for each object differently, so for this we will use __init__ method.

class ListOps:
	def __init__(self, l):
		self.l = l
	
	def extract_even(self, l):
		l1 = []
		for i in l:
			if i%2 == 0:
				l1.append(i)
		return l1
	def extract_odd(self, l):
		l1 = []
		for i in l:
			if i%2 != 0:
				l1.append(i)
		return l1


#__init__ method is also called as magic/ dunder method as it starts with __ and init means to initialize

ops1 = ListOps() #Now will throw error >> while making object/instance of the class, the first method that is executed is __init__ and __init__ needs an argument.

ops1 = ListOps([1, 3, 5, 7, 19])
ops1.l

ops2 = ListOps([11, 78, 3, 21, 2])
ops2.l

ops1.extract_even() #throw an error


#Note:#Be careful when you are using __init__ method then you dont need to pass l.
class ListOps:
	def __init__(self): #Be careful when you are using __init__ method then you dont need to pass l. 
		self.l2 = l
	
	def extract_even(self):
		l = self.l2 #Just write this line in extra along with removing l argument. Everywhere you will be able to access l using self.l2
		l1 = []
		for i in l:
			if i%2 == 0:
				l1.append(i)
		return l1
	def extract_odd(self):
		l = self.l2
		l1 = []
		for i in l:
			if i%2 != 0:
				l1.append(i)
		return l1


#Why wrote l = self.l?
see pic
self.l is heading class ListOps and = l means l is that list we are entering.
obj1 =ListOps([1,2,3,4]), so ListOps = l in this l will be [1,2,3,4]


Ops1 = ListOps([1,3,4,5,6])
Ops1.extract_even() #Noneed to pass arg in () now.



#Multiple attributes
pass dynamic variable instead of fixed variable
Ex. In a library a book is associated with author, title, name. We have to access author and title  & author and name.

class Book:
	def __init__(self, name, author, title):
		self.name_of_book = name
		self.book_author = author
		self.title_name = title

	def extract_details_name_title(self):
		print(self.name_of_book, self.title_name)

	def extract_details_name_author(self):
		print(self.name_of_book, self.book_author)

student1 = Book("stats", "joss", "descriptivestats")
student1.extract_details_name_title()


#In the above code the variables were dynamic but if we keep the variable fixed or static then it will be an issue as if we try to update the details then it will throw error.

class Book:
	def __init__(self, name, author, title):
		self.name_of_book = "Harry"
		self.book_author = "Ross:
		self.title_name = "Metricith"

	def extract_details_name_title(self):
		print(self.name_of_book, self.title_name)

	def extract_details_name_author(self):
		print(self.name_of_book, self.book_author)

student1 = Book("stats", "joss", "descriptivestats")
student1.extract_details_name_title() #O/P: Harry, metricith





#LECTURE 2: INHERITANCE AND ABSTRACTION

1. INHERITANCE
#Def: It refers to process of child receiving the properties of parent class. 
#Syntax:
class BaseClass:
	#Body of base class
class DerivedClass(BaseClass):
	#body of derived class

#Derived class has all the properties of base class.

#Types of inheritance

(i) SINGLE INHERITANCE --> When a derived class has only one parent class.
  parent class
	|
	|
	\/
  child class

#Example.
class Father:
	def father_property(self):
		print("This is the father property")

class Son(Father):
	def job(self):
		print("Son has property from job")

child_oj = Son() #object/instance of son class
child_obj.job()

child_obj.father_property()

#A father will have only his property
father_obj = Father()
father_obj.father_property()

father_obj.job() #Error, as you cant access son property.


#Parent class will not have access to attribute /method of child class but child have access to itself and parent class properties.

Ex.
class Fruit:
	def fruit_info(self):
		print("Inside parent class")
class Apple(Fruit):
	def apple_info(self):
		print("Inside the child class")

obj = Apple()
obj.apple_info()

obj.fruit_info()

par = Fruit()
par.fruit_info()

par.apple_info() #Error



#Method overriding

Def: It is re-writing/re-defining methods of parent class in derived/child class.
Ex.
class Fruit:
	def fruit_info(self):
		print("Inside parent class")
class Apple(Fruit):
	def fruit_info(self):
		print("Inside child class (fruit info)")
	def apple_info(self):
		print("Inside the child class")

#same method created in parent and child class. So if we call it which method will be called? When the method is in parent class as well as in child class then always remember that the method of child class will be executed. 

#method overriding>> child class is very powerful

obj = Apple()
obj.fruit_info()


#Method overriding happens between two class.

(ii) MULTI-LEVEL INHERITANCE
parent class-->child class1--> child class2

Ex.
class GrandFather:
	def prop_grand_father(self):
		print("I am your grandfather, this is my property")
class Father(GrandFather):
	def prop_father(self):
		print("I am your father, and I have my as well as your grand father property")
class Son(Father):
	def prop_son(self):
		print("I am the king, I have both and mine property")

son = Son()
son.prop_father(0

son.prop_grand_father()

son.prop_son()

fath = Father()
fath.prop_grand_father()

fath.prop_father()

gf = GrandFather()
gf.prop_grand_father()


#Use case
class Vehicle:
	def vehicle_info(self):
		print("Inside vehicle class")
class Car(Vehicle):
	def car_info(self):
		print("Inside the car class")
class SportsCar(Car):
	def sports_car_info(self):
		print("Inside sports car")

s1 = SportsCar()
#same chiz jo upar wale example me kiye

#Another example of method overriding:
class Vehicle:
	def vehicle_info(self):
		print("Inside vehicle class")
class Car(Vehicle):
	def car_info(self):
		print("Inside the car class")
class SportsCar(Car):
	def sports_car_info(self):
		print("Inside sports car")

s1 = SportsCar()
s1.vehicle_info() #Method overrin=ding>> Child class is most powerful


(iii) MULTIPLE INHERITANCE
One child class may inherit the property of multiple parent class.
parent class1 + parent class 2 ----> Child class


Ex.
class ParentClass1:
	def method1(self):
		print("Method 1 of parent class 1")
class ParentClass2:
	def method2(self):
		print("Method 2 of parent class 2")

class ChildClass(ParentClass1, ParentClass2):
	def method(self):
		print("Method of child class")

c1 = ChildClass()
c1.method()
c1.method1()
c1.method2()

#Diamond problem>> It occurs when a class inherits from 2 or more than 2 class>>Will lead to ambiguity in calling of method.
#To remove diamond problem>> python uses method resolution prder(MRO) algorithm called c3 linearization.
#Means that the class that is inherited first in the derived class, that method will be called.
#Now suppose all have same method name:

class ParentClass1:
	def method_par(self):
		print("Method 1 of parent class 1")
class ParentClass2:
	def method_par(self):
		print("Method 2 of parent class 2")

class ChildClass(ParentClass1, ParentClass2):
	def method(self):
		print("Method of child class")

c1 = ChildClass()
c1.method_par() #As in child class the parent1 comes first as written so here it will call parent class 1 method.


Ex. Diamond problem
class A:
	def method(self):
		print("Method of class A")
class B(A):
	def method(self):
		print("Method of class B")
class C(B):
	def method(self):
		print("Method of class C")
class D(C,B):
	pass

d = D()
d.method()


(iv) HIERARCHIAL INHERITANCE 
One parent class and multiple(more than two) child class
Parent class ---> child class1, child class2, child class3

Ex.	
class Vehicle:
	def info(self):
		print("This is vehicle")
class Car(Vehicle):
	def car_info(self, name)
		print("This is car info", name)
class Truck(Vehicle):
	def truck_info(self, name):
		print("Truck info", name)

c1 = Car()
c1.info()

c1.car_info("BMW")

obj2 = Truck()
obj2.truck_info("Truck1")



(v) HYBRID INHERITANCE
#Multiple types or combination of different inheritance
#parent class --> child class 1 and child class 2--> child class 3
Ex.
class Vehicle:
	def vehicle_info(self):
		print("Inside the vehicle class")
class Car(Vehicle):
	def car_info(self):
		print("Inside the car class")
class Truck(Vehicle):
	def truck_info(name):
		print("Inside truck info", name)
class SportsCar(Car, Vehicle):
	def sports_info(self):
		print("Innside sports car class")

obj1 = SportsCar()
obj1.car_info()

obj1.vehicle_info()

obj1.car_info()



2.ABSTRACTION
#It is the concept of hiding complex implementation
#Hiding unneeded details and exposing the required
#Abstract class cannot be instantiated(cannot make object)
#Abstract class should always be subclasses
#Abstract class may contain methods that are just declared and not implemented in abstract class itself, subclass are responsible for implementing these abstract methods.
#Ex. u only see interface of pwskills and no backend things. only imp info for u is shown.
#Abstraction can be achieved using abstract class>> import abc
#If in inherited class a method is not present from abstract class it will not throw error.

import abc #This is a module. Collection of multiple functions is a module.

#Inside this module we will have abstract meyhods
#Use case
#In any class at pwskills>> for data science/ frontend / etc domains, the following three methods will be common. So now we know that these three things will be common for any domain in pwskills then we will make pwskills class as a abstract class using a "Decorater"


#Declaring methods(not implementing as using pass) 
class PwSkills:

	@abc.abstractmethod #This @Abc is abstract method
	def student_details(self):
		pass

	@abc.abstractmethod
	def student_assignment(self):
		pass

	@abc.abstractmethod
	def student_marks(self):
		pass


#Implementing the declared method
class DataScience(PwSkills): #It will inherit pwskill class
	def student_details(self):
		return "Data Science course details"
	
	def student_marks(self):
		return "give ds student marks"

class WebDev(PwSkills):
	def student_details(self):
		return "This will give web devstudent assignment"
	def student_marks(self):
		return "webdev student marks"

ds = DataScience()
ds.student_assignment() #It will not throw any error even if any method is not define.

ds.student_details()


w = WebDev()
w.student_marks()


#Use case
class Shape:

	@abc.abstractmethod
	def calculate_area(self):
		pass

class Rectangle(Shape):
	def calc_area(self):
		return "Area is len*breadth"

class Circle(Shape):
	def calc_area(self):
		return "Area is pi r **2"

rect = Rectangle()
rect.calc_area()






#LECTURE 3: POLYMORPHISM AND ENCAPSULATION

1. POLYMORPHISM

#Poly means may and morphism means forms/states.
#Refers to an object taking several forms depending on the methods/data.

len("Ajay")

len([1,2,3,4,5])

len((1,2))

#So you can see same len() is used to calculate length of different data structure.


#Ex.
def func(a, b):
	return a+b

func(2, 3) #Same function is adding two numbers.

func("pw", "Skills") #Same function is combining two strings

func([1,2,3],[4,5,6])

#Observation>> func is taking different forms with respect to ifferent data passed.

class teacher_lecture:
	def lec_info(self):
		print("This is lec info with teacher perspective")
class student_lecture:
	def lec_info(self):
		print("This is lec info with student perspective")

obj1 = teacher_lecture()
obj2 = student_lecture()
class_obj = [obj1, obj2]

def parcer(class_obj):
	for i in class_obj:
		i.lec_info() #at this point, lec_info is taking two forms wrt teacher and student.

parcer(class_obj)

#Polymorphism in OOPS takes place in two ways:
#Method overloading >> Python doesn't support true method overloading
#Method overriding

#Method overloading:

class Student:
	def student(self):
		print("Welcome to pwskills class")
	def student(self, name = ""):
		print("Welcome to pwskills class", name)
	def student(self, name = "", course = "")
		print("Welcome to pwskills class", name, course)

stud = Student()
stud.student()

stud=ud.student("Ajay") #By default it executed 2nd method

stud.student("Ajay", "DS")


#Method Overloading >> student method is taking different forms, the last methods overload the previous ones in the same class.
#It always happens in the same class.

#Method overriding >> Method in parent class with same signature, then child class will be executed. (Seen in last lecture)



2. ENCAPSULATION
#Means hiding something
#Bundling of data and methods of a class
#Access modifier>> Three types: public, protected, private.


(i) Public modifier:-

Ex.
class Student:
	def __init__(self, name, degree):
		self.name = name
		self.degree = degree
stud1 = Student("Ram", "masters")
stud1.name

stud1.degree

stud2 = Student("Sam", "bach")
stud2.degree

stud2.degree = "Phd" #By mistake if I do this
stud2.degree #Then also it will be modified to Phd. 
#As it is public
#So this was the example of public modifier.


#If you dont want to change data then you need to change the modifier from public to private or protected.

(ii)Private
The data and method is only accessible within its class, use __ to make private
Ex.
#Accessing the public data member inside the other method of same class
class Student:
	def __init__(self, name, degree):
		self.name = name
		self.degree = degree

	def show(self):
		#Accessing the private and public data member
		print("name", self.name, "degree", self.degree)
Student("Ajay", "Masters")
aj.show()

#Let's make name as public and degree as private:

class Student:
	def __init__(self, name, degree):
		self.name = name
		self.__degree = degree #private data

	def show(self):
		#Accessing the private and public data member
		print("name", self.name, "degree", self.__degree) #Just add two _ _ and you are done.

aj = Student("Ajay", "Masters")
aj.show() #Now you will not be able to access degree

aj.degree() #error

aj.__degree #error

aj.degree = 'phd' #error
aj.__degree #Error

#if you want to access private variable then:
aj._Student__degree #Will show output


#Making a method private:
class Student:
	def __init__(self, name, degree):
		self.name = name
		self.__degree = degree #Privvate

	def show(self):
		#Accessing the private and public data member
		print("name", self.name, "degree", self.__degree)
	def __private_method(self):
		print("This is a private method")

obj1 = Student("Ajay", "Masters")
obj1.private_method() #Throw an error

#how to access it:
obj1._Student__private_method() #It will give the output


#Way to provide an option to see the private method>> a wrapper

class Student:
	def __init__(self, name, degree):
		self.name = name
		self.__degree = degree #Privvate

	def show(self):
		#Accessing the private and public data member
		print("name", self.name, "degree", self.__degree)
	def __private_method(self):
		print("This is a private method")
	
	def access_private_method(self):
		self.__private_method()

obj1 = Student()
obj1.access_private_method() #Will show output

#Ex. Another use case
class Car:
	def __init__(self, year, make, speed, model):
		self.__year = year
		self.__make = make
		self.__speed = speed
		self.__model = model

c1 = Car("1995","maeruti", "80", "Brezza")
c1.year #Error, since all variables are private


Ex. 
class Car:
	def __init__(self, year, make, speed, model):
		self.__year = year
		self.__make = make
		self.__speed = speed
		self.__model = model
	def set_speed(self, speed):
		self.__speed = 0 if speed < 0 else speed
	def get_speed(self):
		return self.__speed

c1 = Car("1995","maeruti", "80", "Brezza")
c1.year #Now it will give output

c1.set_speed(-10000)
c1.get_speed()

Ex. Another use case
class Bank: #Either you deposit or withdraw.

	def __init__(self, balance):
		self.__balance = balance
	
	def deposit(self, amount): #amount is new deposition
		self.__balance = self.__balance + amount

	def withdraw(self, amount):
		if self.__balance >= amount:
			self.__balance = self.__balance - amount
			return True
		else:
			return False

	def get_balance(self):
		return self.__balance

acc1 = Bank(1000)
acc1.get_balance()

acc1.deposit(500)
acc1.get_balance()

acc1.withdraw(100)

acc1.get_balance()

acc1.withdraw(500000) #False


(iii)Protected
>>within the class and its subclass, protected member can be access, (_)

class College:
	def __init__(self):
		self._college_name = "PwSkills"
class Student(College):
	def __init__(self, name):
		self.name = name
		College.__init__(self) #Accessing variable of base class>>classname__init__(self)

	def show(self):
		print("name". self.name,"college", self._college_name) #directly call the base class variable using _


stud = Student("ajay")
stud.name
stud.show()


coll = College()
coll._college_name #accessing the protected variable.


#Another way to access the data of base class is using super() class
class College:
	def __init__(self):
		self._college_name = "PwSkills"
class Student(College):
	def __init__(self, name):
		self.name = name
		super.__init__(self) #instead of writing class name just write super.
#include super and remove self, base class is super class

	def show(self):
		print("name". self.name,"college", self._college_name)


stud = Student("ajay")
stud.show()






##LECTURE 4: CLASS AND STATIC METHOD
1. class methods
#Bound to the class(and not to a particular instance of the class)
#It can access/modify methods and attributes associated to the class across all the instances.
#Class method can be defined by using: @classmethod decorator
#Instead of self, we will directly use cls as first parameter.
#you can consider it as alternative of init method.
#

Ex.
class Student:
	#this particular method(init) is constructor >> constructor class with initialisation of variables/data
	def __init__(self, name):
		self.name = name

obj = Student("Ajay")
obj.name


#ex. now in same class student we are going to define a class method.
class Student:
	def __init__(self, name):
		self.name = name #self means this variable/method is referring to current instance of the class

	@classmethod #bound/binds to the class
	def student_details(cls, name): #instead of self as first parameter, you are using cls>>means, this method is associated/reffering to the class itself.
		return cls(name)

#What is the meaning that is referring the class?
--> Earlier to access any method/attribute >> first make instance/object of class
--> then obj.attribute
--> but if it is class method you can directly access it.


Student.student_details("Ajay") 
OR,
obj1 = Student.student_details("Ajay") #Since student_details directly binds to the class you can directly call it without making any object. 
obj1.name

#WE are here actually doing method overloading.
#We are seeing class method as alternative of init method. Actually class method is overloading init method.

Ex. How class method is overloading init method
#modifying the class/instance method
class Student:
	def __init__(self, name):
		self.name = name

	@classmethod #bound/binds to the class
	def student_details(cls, name1):
		return cls(name1)

stud = Student.student_details("Ajay") 
obj1.name #You will get Ajay inspite the variable name1, because it is overloading init method and hence you can consider it as alternative of init method.



#Class method can modify class state applicable to all the instances of the class
Ex.
class Student:
	total_students = 0 #class variable
	def __init__(self, name): #instance method
		self.name = name  #instance variable
		Student.total_students = Student.total_students+1 #total_student is the class variable associated with all the instances.

	@classmethod
	def get_total_students(cls):
		return cls.total_students

Students.total_students

std1 = Student("Ajay")
std2 = Student("Bijay")

std1.name

std2.name

Students.total_students #You will get a 2 as this class variable was before 0+1 = 1 now you put bijay also so it become 1+1=2

Student.get_total_students()

#Hence it is proved that class variable can modify the variable across all instances.
#That's why you see increase in the count



Ex. To make external function as class method
class Student:
	total_students = 0 
	def __init__(self, name): 
		self.name = name  
		Student.total_students = Student.total_students+1

	@classmethod
	def get_total_students(cls):
		return cls.total_students


def course_details(cls, course_name):
	print("The details of the course are:", course_name)
Student.course_details = classmethod(course_details) #adding external function as class method

Student.course_details("Data Science")


Ex. Delete any class method
del Student.course_details

Student.course_details("Data Science") #Error, as deleted this method.

Student.get_total_students()

#Another way to delete
delattr(Student, "get_total_students")

Student.get_total_students() #Error



2. Static method
#Does not modify class or instance state, doesn't access instance or class state
#It doesn't depend on class/instance
#It behaves like a plain function that belongs to class
#It doesn't take either self or cls
#@static method is used
#works with the parameters passed

Ex. 
class Calculator:

	@staticmethod
	def add(x, y):
		return x+y

	@staticmethod
	def subtract(x, y):
		return x-y

Calculator.add(5, 6)

Calculator.subtract(10, 5)





##LECTURE 5: DUNDER METHOD

#dunder/magic/special method

print("Hello world") #print is a keyword/inbuilt function

#Dunder/magic/special methods are the methods defined by built-in classes in python
#Classes define these type of methods for creating custom objects >> for init it means for data for every object. 
#implementing operator overloading in python

#d+under
#double underscore>> All methods surrounding double underscore is a dunder method. 


Ex.
a = "pw
b = "skills
a+b

#other way to do this
a.__add__(b) #a dunder method/special/magic method associated with strings

#all dunder methods associated with strings
dir(str) #U will get all dunder methods

Ex.
a = 3
b = 5
a.__add__(b)
 

#useful dunder methods
#__init__ >> to take data with respect to object
class Student:
	def __init__(self, name):
		print(name, "This is the first thing that will be executed when you make instance/object of the class")
obj1 = Student("Ajay")

obj2 = Student("Bijay")


#Ex. another magic method >> __new__
class Student:
	#_new__ is responsible for creating new instance of a class 
	def __new__(cls): #Since cls>> so it will be reffering to the class directly.
		print("This will be executed even before init.")
	#It is used to initialize the newly created insance/object>>It sets up any initial state/properties of the object.
	def __init__(self, name):
		print(name, "This is the first thing that will be executed when you make instance/object of the class")

obj = Student()


#Another dunder method>> __st__
class Student:
	def __init__(self):
		self.phone = 999999999

Student() #Hexadecimal representation of memory of student object will be output

print(Student())

Ex.
class Student:
	def __init__(self):
		self.phone = 999999999

	def __str__(self): #__str__ will return a string representation of object
		return "This method overloads the print statement of object.

Student()
print(Student())

#Another dunder method __repr__ >> Meaning representation
#Itreturns unambiguous string representation of the object as it is, that can be used torecreate the object.

class MyClass:
	def __int__(self, x):
		self.x = x
	def __repr__(self):
		return f"MyClass({self.x})"
obj = MyClass(5)
obj

print(repr(obj))

#Another magic method __eq__
True == True

3 ==3

a = 3
b = 3
a.__eq__(b)

#use case of this
class Point:
	def __init__(self, x, y):
		self.x = x
		self.y = y
	def __eq__(self, other):
		return self.x == other.x and self.y == other.y
p1 = Point(1, 2)
p2 = Point(1, 2)
print(p1 == p2) #Comparing both object
2#When you are using == operator with point objects, python internally calls __eq__


#__add__
class Point:
	def __init__(self, x, y):
		self.x = x
		self.y = y
	def __eq__(self, other):
		return Point(self.x + other.x, self.y + other.y)
p1 = Point(1, 2)
p2 = Point(1, 2)
p3 = p1 + p2#When you are using + operator with point objects, python internally calls __add__
print(p3.x, p3.y)





##LECTURE6: DECORATORS
#It allows to modify or extend the behavior or functions/class without directly modifying their code.
#Similar to you decorating your room (putting different lights, sticker, posters)>> extends/decorates the basic behavior of the room.

1. Function decorators

Ex.
# To understand use case>> Say you want to use a line before the computation and after computation after each time you create or call function. So it will take a lot of time to type the lines repetitively. Thta's why decorators comes into picture.
  
def my_decorator_func():
	print("The line before computation.")
	print(11*1200) #Decorating the actual computation with line above and line below 
	print("The line after computation")
my_decorator_func()


#In other approach you have to write all the line as many times as you are creating the different functions.
#Lets see the decorator approach.


#Decorator approach for function>>use case1:
 def my_decorator(func): #This is decorator function that takes another function as argument
	def wrapper(): #wrapper is a nested function that adds the functionality before and after calling original function.
		print("The line before computation:")
		func() #say_hello which is the func will be executed here
		print("The line after computation.")
	return wrapper

@my_decorator #syntax to decorate the say_hello function.
def say_hello()
	print("Hello")

say_hello()
#when say_hello is called, it is actually calling the decorator function.>> Which in turn is calling wrapper function and then wrapped function is printing the line and calling the say_hello function.


#Ex. Another use case of function decorator.
#run time of a code

import time
def timer_decorator(func):
	def timer():
		start = time.time()
		func()
		end = time.time()
		print("The time for executing the code". end-start)
	return timer

@timer_decoratior
def func_test():
	print(1100000*1000)
func_test()


#Why do we need decorators?
-->Reusability of code>> reuse the common code
--> enhancing the function without modifying the original function
-->Use cases>> execution time of code, logging, caching, validation


2. Class decorators

class MyDecorators:
	def __init__(self, func): #similar to function decorator you are passing func in class decorator.
		self.func = func
		print("Inside the init method")
	def __call__(self):  
		print("Something is happening before function.")
		self.func()
		print("something is happening after function.")

@MyDecorator #class __call__ will be executed as the object of the class will be called as function>> so first __init__ method will be executed and then __call__ method will be executed.
def say_hello():
	print("Hello")
say_hello()


#__call__ is a special method which is called/invoked when you call instance/object of the class as a function.


obj1 = MyDecorator() #error


Ex. 
class MyDecorators:
	def __init__(self): #similar to function decorator you are passing func in class decorator.
		#self.func = func
		print("Inside the init method")
	def __call__(self):  
		print("Something is happening before function.")
		#self.func()
		print("something is happening after function.")

obj1 = MyDecorator() #It will run
#When you make an object of the class, init is executed first	


obj1() #When you call an object of a class as function __call__ method will be invoked 



#Some inbuilt decoretors: INTRODUCTION

(i). @classmethod >> The method that tales the class itself as the first argument
Ex.
class Math:
	@classmethod #takes reference to the class itself to modify and access class level attributes
	def add(cls, x, y):
		return cls.__name__, x + y #cls.__name__ >> class math

#you dont need any init method to take data
Math.add(3, 5)
#classs method is bound to class and not the instance of the class, class itself as the first argument >> conventionally cls

(ii). static method
The method which can be called without creating any instance of class, and without using self or cls.
Ex.
class Math:
	def add(self, x, y):
		return x+y
a = Math() #make object/instance
a.add(2, 3)

#use of static method
class Math:
	@ataticmethod
	def add(x, y): #no need of self or cls
		return x+y
Math.add(2, 3) #no need of making any object



#Comparision of Class method and static method:
(i) in Class method, cls is as first argument whereas in static there is no first argument.
(ii) In class method you can access and modify class level state whereas in static we cannot access.

#Class method to be used when you want to modify class level data.
#static method >> when you dont want to interact with class level data.


3. Property decorator
It allows method to be accessed as attribute
Ex.
class Circle:
	def __init__(self, radius):
		self.radius = radius

obj = Circle(5)
obj.radius #accessing data / attribute


class Circle:
	def __init__(self, radius):
		self.radius = radius
	def area(self):
		radius = self.radius
		return 3.14*radius**2

obj1 = Circle(5)
obj.radius

obj.area() #earlier

#Use of property decorator
class Circle:
	def __init__(self, radius):
		self.radius = radius
	@property
	def area(self):
		radius = self.radius
		return 3.14*radius**2
obj1 = Circle(5)
obj1.radius
obj1.area #No need of parenthesis.





##LECTURE7: PROPERTY DECORATORS
clas  Student:
	def __init__(self, name, price):
		self.__name = name
		self.__price = price
#here name and price are private variables which you will not be able to access from outside the class
stud = Student("Ajay", 3000)
stud.name #error as name and price are private variables.
#still you can access private variables if you know structure of the class
stud._Student__name #using class name and exact variable name


#another way to expose private variables using property decorators

class Student:
	def __init__(self, name, price):
		self.__name = name
		self.__price = price
	@property
	def access_price(self):
		return self.__price
stud = Student("Ajay", 5000)
stud.access_price


#If you want to modify the price
class Student:
	def __init__(self, name, price):
		self.__name = name
		self.__price = price

	@property
	def access_price(self):
		return self.__price

	@access_price.setter
	def price_set(self.price_new):
		self.__price = price_new

stud.access_price

stud.price_set = 1500
stud.access_price



#delete variable
class Student:
	def __init__(self, name, price):
		self.__name = name
		self.__price = price

	@property
	def access_price(self):
		return self.__price

	@access_price.setter
	def price_set(self.price_new):
		self.__price = price_new

	@access_price.deleter
	def del_price(self):
		del self.__price

stud = Student("Ajay", 15000)
stud.access_price

stud.price_set = 20000
stud.access_price

stud.del_price

stud.access_price
