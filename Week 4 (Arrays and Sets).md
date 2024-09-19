### Arrays
```python
# Define Array
myArr = []

# Add to end
myArr.append(6)
myArr.append(7)
myArr.append(8)
print(myArr)

# Remove from end
myArr.pop()
x = myArr.pop()
print(x)
print(myArr)
```
### Array Slicing
```python
# Syntax:
# ARR[start:end:step]
myArr = ["ic", "pc", "jo", "na", "th", "an"]

# First N
n = 2
print(myArr[:n])

# Last N
n = 4
print(myArr[-n:])

# Every Other
print(myArr[::2])

# Reverse
print(myArr[::-1])
```
### Sets
```python
# Define Set
mySet = set()

# Add to set
mySet.add(11)
mySet.add(22)
mySet.add(33)
print(mySet)

# Remove from set
mySet.discard(22)
print(mySet)

# NOTE! No duplicate values in a set
mySet.add(44)
print(mySet)
mySet.add(44)
print(mySet)

# Set Union
myOtherSet = set([11,66,99])
print(myOtherSet | mySet)

#Set Intersection
print(myOtherSet & mySet)
```
