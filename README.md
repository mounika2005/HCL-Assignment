### 1.	Write a function calculate(a, b, operation) that performs addition, subtraction, multiplication, or division based on the supplied operation.
```
def calculate(a, b, operation):
    if operation == "+":
        return a + b
    elif operation == "-":
        return a - b
    elif operation == "*":
        return a * b
    elif operation == "/":
        return a / b
    else:
        return "Invalid operation"
a = 20
b = 5
operation = "+"

result = calculate(a, b, operation)

print("Result:", result)



```
## output:
<img width="1303" height="660" alt="image" src="https://github.com/user-attachments/assets/c9117f41-c3cd-40f9-8bb4-b5bf4e3e0020" />


### 2.	Write a function sum_numbers(*args) that accepts any number of arguments and returns their sum.


```

def sum_numbers(*args):
    return sum(args)


result = sum_numbers(10, 20, 30, 40)

print("Sum:", result)

```
## output:
<img width="1325" height="315" alt="image" src="https://github.com/user-attachments/assets/79f1ee4f-d287-41f4-a937-86421b8b8f85" />


### 3.	Write a function employee(**args) that accepts employee information such as name, ID, department and salary, then displays the information.


```

def employee(**args):
    print("Employee Information:")
    
    for key, value in args.items():
        print(key, ":", value)


employee(
    name="Mounika",
    ID="EMP101",
    department="Cyber Security",
    salary=40000
)

```
## output:
<img width="1555" height="462" alt="image" src="https://github.com/user-attachments/assets/4b86858f-6502-47c6-98fd-33274153bbd1" />


### 4.	Write a function remove_duplicates(lst) that returns a list containing only unique elements while preserving their original order.

```

def remove_duplicates(lst):
    unique_list = []

    for item in lst:
        if item not in unique_list:
            unique_list.append(item)

    return unique_list


numbers = [10, 20, 10, 30, 20, 40, 30]

result = remove_duplicates(numbers)

print("Original List:", numbers)
print("List after removing duplicates:", result)

```
## output:

<img width="1617" height="465" alt="image" src="https://github.com/user-attachments/assets/0eb6f330-50b4-448c-acac-76388bb34a7f" />


### 5.	Using a lambda function, sort a list of tuples based on the second element. Example: [(1,5), (2,3), (4,1)].

```

numbers = [(1, 5), (2, 3), (4, 1)]

sorted_list = sorted(numbers, key=lambda x: x[1])

print("Original List:", numbers)
print("Sorted List:", sorted_list)


```
## output:
<img width="1611" height="250" alt="image" src="https://github.com/user-attachments/assets/08167014-4f1f-4f26-adff-a9afb1adc5e6" />

