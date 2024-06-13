# Programming-Syntax-CHEATSHEAT

--- enumerate

## Math Operation

Min and Max of two numbers
```python
print(min(5, 7)) # 5
print(max(5, 7)) # 7
```

Absolute value
```python
print(abs(-69)) # 69
```

Infinite max and min values
```python
# Positive Infinity
float("inf")
math.inf

# Negative Infinity
-float("inf")
-math.inf
```


## List Operations

add remove
slice operations

## Queue Operations

```python

# Declaring a Queue
queue = deque()
queue = deque(['name','age'])   

# Appending
queue = deque(3)
queue.append(6)      # append to the end of the queue   = [3, 6]
queue.appendleft(9)  # append to the front of the queue = [9, 3, 6]

# Popping
Print(queue.pop())     # 6  queue = [9, 3]
Print(queue.popleft()) # 9  queue = [3]
```
Additional operartion 

```python
index(ele, beg, end):- This function returns the first index of the value mentioned in arguments, starting searching from beg till end index.
insert(i, a) :- This function inserts the value mentioned in arguments(a) at index(i) specified in arguments.
remove():- This function removes the first occurrence of the value mentioned in arguments.
count():- This function counts the number of occurrences of value mentioned in arguments.
```

## Set operations
add
remove


## Map Operations

add
remove

## String Operation

Check if a string contains the prefix

```python
'''
Syntax: str.startswith(prefix, start, end)

prefix: prefix ix nothing but a string that needs to be checked.
start: Starting position where prefix is needed to be checked within the string.
end: Ending position where prefix is needed to be checked within the string.
Return:  Returns True if strings start with the given prefix otherwise returns
'''
var = "new9 string"
 
print(var.startswith("new")) # True
```

Check if string contains digits, alphabets

```python
'''
Syntax: string.isdigit()

Returns:
True – If all characters in the string are digits.
False – If the string contains 1 or more non-digits.
'''
string = '15460'
print(string.isdigit()) # True
 
string = '154abc60' 
print(string.isdigit()) # False
```

```python
'''
Syntax:  string.isalpha()

True: If all characters in the string are alphabet.
False: If the string contains 1 or more non-alphabets.
Errors and Exceptions:

- It contains no arguments, therefore an error occurs if a parameter is passed
- Both uppercase and lowercase alphabets return “True”
- Space is not considered to be the alphabet, therefore it returns “False”
'''

string = 'abc'
print(string.isalpha()) # True
  
string = 'abc111'
print(string.isalpha()) # False
  
# checking if space is an alphabet
string = 'abc abc'
print( string.isalpha()) # False
```

```python
'''
Syntax:  string_name.isalnum()
Return: 
True: If all the characters are alphanumeric 
False: If one or more characters are not alphanumeric
'''

string = "abc 123"
print(string.isalnum())  # False
 
string = "abc_123"
print(string.isalnum())  # False
 
string = "000"
print(string.isalnum())  # True
 
string = "aaaa"
print(string.isalnum())  # True
```

## Lamda operations
### Sorting

sort with passing lamda to sort/sorted functions.
```python
name_list.sort(key=lambda name: name.split()[1])
sorted(key=lambda name: name.split()[1])
```

sort with creating a separate lamda and then passing it.
```python
# The lambda
sorter_key = lambda name: name.split()[1]
name_list.sort(key=sorter_key)
sorted(key=sorter_key)
```

sort with defined function.
```python
# Function to return key used for sorting.
def get_sort_key(name):
  return name.split()[1]
name_list.sort(key=get_sort_key)
sorted(key=get_sort_key)
```
collections.counter

