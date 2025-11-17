# 📘 Python Tuple

## 🧠 What is a Tuple?
A **tuple** in Python is a collection of items that is:

- **Ordered**
- **Immutable** (cannot be changed after creation)
- Allows **duplicate values**
- Can store **multiple data types**

Tuples are written using **parentheses `( )`**.

### Example
```python
my_tuple = (10, 20, 30)
print(my_tuple)
```

### ✨ Why Use Tuples?
- Faster than lists  
- Data remains safe because tuples cannot be changed  
- Can be used as dictionary keys  
- Good for fixed data  

### 📍 1. Creating Tuples
#### ✔ Normal Tuples
```python
numbers = (1, 2, 3, 4)
```

#### ✔ Tuple with multiple data types

```python
student = ("Rahim", 21, 3.75, True)
```

#### ✔ Tuple without parentheses (tuple packing)
```python
fruits = "apple", "mango", "banana"

```

#### ✔ Single-item Tuple (Important)
```python
single = (10,)       # Correct
not_tuple = (10)     # Wrong → This is an integer

```

### 📍 2. Accessing Tuple Items
#### ✔ Access by index
```python
numbers = (10, 20, 30, 40)
print(numbers[0])   # 10
print(numbers[2])   # 30

```
#### ✔ Negative indexing
```python
print(numbers[-1])  # 40
print(numbers[-2])  # 30

```


### 📍 3. Slicing Tuples
####
```python
letters = ('a', 'b', 'c', 'd', 'e')

print(letters[1:4])   # ('b', 'c', 'd')
print(letters[:3])    # ('a', 'b', 'c')
print(letters[2:])    # ('c', 'd', 'e')

``` 
### 📍 4. Looping Through Tuples
#### ✔ Using for loop
```python
colors = ("red", "green", "blue")

for c in colors:
    print(c)

```
#### ✔ Using index

```python
for i in range(len(colors)):
    print(colors[i])

```

### 📍 5. Useful Tuple Methods
#### ✔ count()
Counts how many times a value appears.

```python
numbers = (1, 2, 3, 2, 4, 2)
print(numbers.count(2))   # 3

```
#### ✔ index()
Returns the index of the first occurrence.

```python
print(numbers.index(3))   # 2

```
### 📍 6. Tuple Unpacking
#### ✔ Basic Unpacking
```python
person = ("Rafi", 25, "Dhaka")

name, age, city = person

print(name)  # Rafi
print(age)   # 25
print(city)  # Dhaka

```
#### ✔ Using * (Star) for multiple values
```python
values = (10, 20, 30, 40, 50)

a, b, *rest = values

print(a)     # 10
print(b)     # 20
print(rest)  # [30, 40, 50]





### 📍 7. Tuple vs List (Quick Comparison) 

| Feature    | Tuple      | List         |
| ---------- | ---------- | ------------ |
| Syntax     | `( )`      | `[ ]`        |
| Changeable | ❌ No       | ✅ Yes        |
| Faster     | ✅ Yes      | ❌ No         |
| Used For   | Fixed data | Dynamic data |

### 📍 8. Practical Examples
#### ✔ Example 1: Return multiple values from a function
```python 
def calculate(a, b):
    return (a + b, a * b)

sum_result, mul_result = calculate(10, 5)

print(sum_result)  # 15
print(mul_result)  # 50

```
#### ✔ Example 2: List of tuples (student records)
```python
 students = [
    ("Shuvo", 24),
    ("Fairoz", 23),
    ("Tamim", 22),
    ("Sayem", 25)
]

```

### 📍 9. Practice Questions
#### ✔ Basic
- Create a tuple with 5 items and print each item.  
- Create a tuple of numbers and find the sum.   
- Print the last item of a tuple using negative indexing.  

#### ✔ Intermediate
- Slice a tuple to get the middle three items.  
- Count how many times a value appears in a tuple.  
- Unpack a tuple into 4 variables.
  
#### ✔ Advanced
- Write a function that returns (min_value, max_value) without using min() or max().  
- Store multiple student records using a list of tuples and print only the names.  
- Modify the tuple value using index number [you can search it]