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

- Exponent:`a = b ** c`

  ​					Returns  b power c



---

Try out the following programs.



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

## 

