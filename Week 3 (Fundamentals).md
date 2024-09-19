### Input and Output
```python
# Basic Input
myVar = input()
print(myVar)

# Space-separated numbers
a,b,c = map(int, input().split())
```
### Math
```python
print(3+14)  # Addition
print(14-3)  # Subtraction
print(5*5)   # Multiplication
print(2**6)  # Exponentiation
print(22/7)  # Floating-point Division
print(22//7) # Integer Division (rounds down)
```
### Conversions
```python
# String to Integer
print(int("4") * 4)

# Integer to String
print(str(4) * 4)
```
### Loops
```python
# For loop
for idx in range(10):
	print(idx)

# While loop
jonathanSanity = 10
while jonathanSanity > 0:
	jonathanSanity -= 1
	print(jonathanSanity)
```
### Conditionals
```python
s = "SETH"
while True:
	if len(a) < 20:
		s += "SETH"
	else:
		break
print(s)
```
### Misc.
```python
# Check length of variable
var = "hiya"
print(len(var))

# Check if a is in b
a = "magentadaffodil"
b = "tada"
print(b in a)
print(a in b)

# Split string by delimiter (default is space)
s = "i am a sentence"
print(s.split())

# Join list with delimiter
a = ["i", "am", "a", "list"]
print("---".join(a))

# Lower and Uppercase
s = "JonathandeKoning"
print(s.lower())
print(s.upper())
print(s[0].isupper())
print(s[0].islower())
```
