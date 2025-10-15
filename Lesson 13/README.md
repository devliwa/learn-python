# debugging-how-to-find-and-fix-errors-in-your-code

- [python-questions](https://stackoverflow.com/questions/tagged/python)

#### describe-the-problem
```python
def my_function():
    for i in range(1, 21):
        if i == 20:
            print("You got it")


my_function()
```

#### reproduce-the-bug
```python
from random import randint
dice_images = ["❶", "❷", "❸", "❹", "❺", "❻"]
dice_num = randint(0, 5)
print(dice_images[dice_num])

```

#### play-computer
```python
year = int(input("What's your year of birth?"))

if year > 1980 and year < 1994:
    print("You are a millennial.")
elif year >= 1994:
    print("You are a Gen Z.")

```

#### fix-the-errors
```python
try:
    age = int(input("How old are you?"))
except ValueError:
    print("You have typed in a an invalid number. Please try again with a numerical response such as 15.")
    age = int(input("How old are you?"))

if age > 18:
    print(f"You can drive at age {age}.")

```
#### use-print
```python
pages = int(input("Number of pages: "))
word_per_page = int(input("Number of words per page: "))
total_words = pages * word_per_page

print(f"pages = {pages}")
print(f"words_per_page = {word_per_page}")
print(total_words)

```

#### use-a-debugger

math.py
```python
def add(n1, n2):
    return n1 + n2
```

main.py
```python
import random
import maths


def mutate(a_list):
    b_list = []
    new_item = 0
    for item in a_list:
        new_item = item * 2
        new_item += random.randint(1, 3)
        new_item = maths.add(new_item, item)
        b_list.append(new_item)
    print(b_list)


mutate([1, 2, 3, 5, 8, 13])
```

