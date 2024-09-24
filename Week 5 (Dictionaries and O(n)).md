## Dictionary
```python
# Initialization
myDict = {}

# Adding Keys and Values
myDict["name"] = "Jonathan"
myDict["age"] = 20
myDict["isSingle"] = True

# Get all keys or all values
allKeys = myDict.keys()
allVals = myDict.values()
print(allKeys)
print(allVals)

# Loop through keys and values
for key, val in myDict.items():
	print(f"Key: {key}, Val: {val}")

# Keys can be any immutable data type,
# but values can be any data type (even dictionaries)
myDict[True] = "False"
myDict[(1,2,3)] = [4,5,6]
myDict["huh"] = myDict
print(myDict["huh"]["huh"]["huh"]["huh"])

# Example Counter
nums = [1,2,1,2,1,2,1,3,3,4,9,8,7,6,5,4,3,2,1]
myCount = {}

for num in nums:
	if num not in myCount:
		myCount[num] = 1
	else:
		myCount[num] += 1

print(myCount)
```

## Defaultdict and Counter
```python
# Defaultdict allows you to modify a key/value pair in a
# dictionary that doesn't exist yet by providing a default value
from collections import defaultdict, Counter

# The default value for integers is 0
myCount = defaultdict(int)
nums = [1,2,1,2,1,2,1,3,3,4,9,8,7,6,5,4,3,2,1]

# So instead of checking if our number is in the dictionary,
# we can do this instead:
for num in nums:
	myCount[num] += 1
print(myCount)

# Alternatively, a Counter object lets us count 
# the frequency of objects in a list all by itself
myCount = Counter(nums)
print(myCount)
```
## O($n$)
```python
# O(n) is the notation used to express how quickly
# the runtime of a program grows as the number of 
# inputs grows

# An O(1) algorithm/operation always takes the same
# amount of time. For example: popping the last element
# in a list is O(1)
short_list = [1,2,3]
long_list = list(range(100000))

a = short_list.pop()
b = long_list.pop()

# An O(n) algorithm/operation scales linearly, meaning
# it goes over some number of the elements some number of
# times, regardless of how many loops it takes 
# (assuming the number of loops is constant)
short_list = list(range(1000))
long_list = list(range(100000000))

print(sum(short_list))
print(sum(long_list))

# An O(n^2) algorithm/operation scales exponentially, meaning
# that for every element, we loop over every element.

short_list = list(range(5000))
long_list = list(range(10000))

short_count = 0
for a in short_list:
	for b in short_list:
		short_count += b
print(short_count)

long_count = 0
for a in long_list:
	for b in long_list:
		long_count += b
print(long_count)

# More O(n) coming soon...
```
