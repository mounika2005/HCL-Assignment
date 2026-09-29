### 1.Print all prime numbers between input range (Ex – input 20 50, prints all prime numbers between 20 and 50).

```
start = int(input("Enter starting number: "))
end = int(input("Enter ending number: "))
print("Prime numbers:")

for num in range(start, end + 1):
    if num > 1:
        for i in range(2, num):
            if num % i == 0:
                break
        else:
            print(num, end=" ")

```
## output: 

<img width="1425" height="378" alt="image" src="https://github.com/user-attachments/assets/9faceb5d-ca9a-4999-97a3-241f0c0158ca" />




### 2.Factorial using recursion

```
def factorial(n):
    if n == 0 or n == 1:
        return 1
    return n * factorial(n - 1)

n = int(input("Enter a number: "))

print("Factorial:", factorial(n))

```
## output:
<img width="1367" height="331" alt="image" src="https://github.com/user-attachments/assets/4b23e79e-2a61-4e16-a759-6a416bf0d899" />


### 3.Square of numbers using lambda
```
square = lambda x: x * x

n = int(input("Enter a number: "))

print("Square:", square(n))

```
## output:
<img width="1367" height="215" alt="image" src="https://github.com/user-attachments/assets/09a800ae-7115-4e0c-b33a-613485926f7e" />


### 4.Find the second largest element in a list

```
numbers = list(map(int, input().split()))

numbers = list(set(numbers))
numbers.sort()

print("List:", numbers)
print("Second largest:", numbers[-2])

```
## output:

<img width="1342" height="311" alt="image" src="https://github.com/user-attachments/assets/ae7d51b7-f5fd-4786-84f0-50ef8be66494" />

### 5.Count frequency of characters in a string

```

text = input("Enter a string: ")
frequency = {}
for char in text:
    if char in frequency:
        frequency[char] += 1
    else:
        frequency[char] = 1

print("Character frequency:")
for char, count in frequency.items():
    print(char, ":", count)
```
## output:
<img width="1480" height="360" alt="image" src="https://github.com/user-attachments/assets/bd7032be-c08d-40b3-9cf6-9d566b7e7a48" />


### 6.Calculate area of a circle using math library.
```
import math

radius = float(input("Enter radius: "))

area = math.pi * radius * radius

print("Area of circle:", area)

```
## output:

<img width="1590" height="351" alt="image" src="https://github.com/user-attachments/assets/bccad384-5b98-4bf5-b86f-949d1f89a93e" />

### 7.Reverse a string without using built‑in reverse
 

```
text = input("Enter a string: ")

reverse = ""

for char in text:
    reverse = char + reverse

print("Reversed string:", reverse)

```
## output:
<img width="1495" height="350" alt="image" src="https://github.com/user-attachments/assets/9a378ed2-434c-464e-ad2c-1ff34c740145" />


### 8.Remove duplicates from a list

```

numbers = [10, 20, 10, 30, 20, 40, 30]

unique = []

for num in numbers:
    if num not in unique:
        unique.append(num)

print("Original list:", numbers)
print("List after removing duplicates:", unique)
```
## output:
<img width="1690" height="353" alt="image" src="https://github.com/user-attachments/assets/9a6a5800-7e14-4877-b137-dfcc414ffa13" />


### 9.Merge two dictionaries

```
dict1 = {"a": 10, "b": 20}
dict2 = {"c": 30, "d": 40}

merged = dict1.copy()
merged.update(dict2)

print("Dictionary 1:", dict1)
print("Dictionary 2:", dict2)
print("Merged dictionary:", merged)

```
## output:
<img width="1712" height="361" alt="image" src="https://github.com/user-attachments/assets/90f14713-2c06-420f-9d5b-a2e276c0bfa2" />


### 10.Fibonacci series using recursion


```
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n - 1) + fibonacci(n - 2)

n = int(input("Enter number of terms: "))

print("Fibonacci series:")

for i in range(n):
    print(fibonacci(i), end=" ")

```
## output:
<img width="1888" height="408" alt="image" src="https://github.com/user-attachments/assets/4f7012f2-bec6-4e1f-88b0-409ff9ea9f80" />

