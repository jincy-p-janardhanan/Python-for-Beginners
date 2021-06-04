# Introduction to Python

- Data Types
- Input/Output
- Operators
- Flow Control
  - Loops



## Data Types

- Numbers

  - integers

    ```python
    a = 1
    b = 231
    ```

  - float

    ```python
    a = 15.23
    pi = 3.1415926535
    ```

  - complex

    ```python
    c = 1 + 2j
    c2 = 1 - 3j
    ```

- List

  ```python
  a = [ 1, 2, 3, 3, 4, 5]
  b = [ ' ', 'a', 'xyz']
  c = [1, 2, 2, 3.14, 'abcd', 1+2j]
  ```

- Tuple

  ```python
  a = (1, 3, 5, 5)
  b = (1, 2, 2, 3.14, 'abcd', 1+2j)
  ```

- Set

  ```python
  a = {1, 3, 5, 4}
  b = {'a', 'b', 10.26}
  ```

- Strings

  ```python
  msg = 'Hello world!'
  text = 'abcdefg'
  ```

- Dictionary

  ```python
  dict1 = { 'a' : 1, 'b' : 2, 'c' : 3}		# key-value pairs
  dict2 = { 'Jack':'New York', 'Jane':'Canada', 'Priya':'Yorkshire'}
  ```

  

## Input/Output



**Input**

```python
name = input('Your good name, please. ')
age = int(input("What's your age?"))
```

**Output**

```python
print(123)
print('Hello World')
print("Your name is ", name, "and you're ", age, 'years old.')
print("Your name is {} and you're {} years old.".format(name, age))
print("Your name is %s and you're %d years old." %(name, age))
print('pi = {:.2f}'.format(pi))
```



## Operators



### Arithmetic

- Addition : ` a = b + c`

- Subtraction: `a = b - c`

- Multiplication: `a = b * c`

- Division:`a = b / c`

- Modulo operator: `a = b % c`

  ​				Returns remainder

- Floor division:`a = b // c`

  ​				Returns the integer part of the quotient

- Exponent:`a = b ** c`

  ​					Returns  $\b^c$



---

#### Practice problems



> **Problem 1**: 
>
> Program to read a number and compute its square and square root.



> **Problem 2:**
>
> Program to calculate area of a triangle.



> **Problem 3:**
>
> A program that takes the number of `wins`, `draws` and `losses` and calculates the number of points a football team has obtained so far.
>
> - `wins` get `3` points
> - `draws` get `1` point
> - `losses` get `0` points



---



### Comparison

- Greater than: `a > b`
- Less than: `a < b`
- Equal to: ` a == b `
- Not equal to: `a != b`
- Greater than or equal to: `a >= b`
- Less than or equal to: `a <= b`



### Logical

- and: `a and b`
- or: `a or b`
- not: `a not b`



### Bitwise

- Bitwise AND: `a & b`
- Bitwise OR: `a | b`
- Bitwise NOT: `-a`
- Bitwise XOR: `a ^ b`
- Left shift: `a << b`
- Right shift: `a >> b`



---

**Notes** 

1. There are shorthand **assignment operators** for all the arithmetic and bitwise operators, like `+=` , `-=` , ` ^=` , etc.
2. There are also some **special operators** like `is` , `is not` , `in` , and `not in` , (which we will discuss shortly).

---



## Flow Control



#### if

Syntax:

```python
if condition:
    # do something
```

Example:

```python
a = 4
b = 5
if a < b:
    print(True)
```



#### if..else

Syntax:

```python
if condition:
    # do something
else:
    # do something else
```

Example:

```python
a = 4
b = 5
if a < b:
    print(True)
else:
    print(False)
```



#### if..else if.. ladder

Syntax:

```python
if condition_1:
    # do something
else if condition_2:
    # do something
...
else if condition_n:
    # do something
else:
    # do something, when all the condtions fail
```

Example:

```python
grade = 95
if grade < 40:
    print('Fail')
else if grade < 50:
    print('D')
else if grade < 60:
    print('C')
else if grade < 70:
    print('B')
else if grade < 80:
    print('A')
else if grade < 90:
    print('S')
else:
    print('O')

# output will be O
```



### Loops

#### while

 Syntax:

```python
while condition_is_true:
    # do something until the condition becomes false
```

Example:

```python
a = 1
while a <= 5:
    print(a)
    a += 1
# prints numbers 1 to 5
```



#### while .. else

Syntax:

```python
while condition_is_true:
    # do something until the condition becomes false
else:
    # do something once the condition becomes false and then exit the loop
```

Example:

```python
a = 1
while a <= 5:
    print(a)
    a += 1
else:
    print('Oh great! I just learnt the numbers 1 to 5. Hope I can pass my pre-school. :) ')
# prints numbers 1 to 5 and also the message in else
```



#### for

Syntax:

```python
for iterator in sequence:
    # do something until the iterator moves through all elements of the sequence
```

Example 1:

```python
for i in range(5):
    print(i)
# prints numbers 1 to 5
```

Example 2:

```python
number_list = [1, 2, 3, 4, 5]
for value in number_list:
    print(value)
# prints numbers 1 to 5
```

Example 3:

```python
alphabets = { 1:'a', 2:'b', 3:'c', 4:'d'}

for key, value in alphabets.items():
    print('Key is %d, value is %s' %(key, value))	# prints both keys and values
    											# i.e 1 and a, 2 and b, 3 and c, 4 and d
for key in alphabets.keys():
    print(key)									# prints only keys, i.e 1 to 4

for value in alphabets.values():
    print(value)								# prints only values, i.e a to d
```



##### for loop for list and dictionary comprehensions

Example 1:

```python
multiples_of_3 = [ i for i in range(3, 31, 3)]
# creates a list containing multiples of 3, from 3 to 30
```

Example 2:

```python
import string
alphabets_index = {alphabet : index+1 for index, alphabet in enumerate(string.ascii_lowercase)}
# creates a dictionary of alphabets mapped to their index positions, like 'a':1, 'b':2, etc
```

