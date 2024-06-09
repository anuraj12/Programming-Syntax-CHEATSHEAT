# Programming-Syntax-CHEATSHEAT

## List/Vector Operations

add remove
slice operations


## Set operations
add
remove


## Map Operations

add
remove

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

