# Conditionals Exercises

## Addition Quiz

Write a program that:

* Generates 2 random numbers
* Prompts the user for the sum
* Prints the result

```
# Example 1
What is 3 + 5? 9
3 + 5 = 9 is False

# Example 2
What is 4 + 1? 5
4 + 1 = 5 is True
```

<details>
  <summary>Python Solution</summary>

```py linenums="1"
import random

num1 = random.randint(0, 9)
num2 = random.randint(0, 9)

answer = int(input('What is {0} + {1}?  '.format(num1, num2)))

print('{0} + {1} = {2} is {3}'.format(num1, num2, answer, num1 + num2 == answer))
```

</details>

<details>
  <summary>JavaScript Solution</summary>

```js linenums="1"
let num1 = Math.floor(Math.random() * 9) + 1
let num2 = Math.floor(Math.random() * 9) + 1

answer = parseInt(prompt(`What is ${num1} + ${num2}?  `))

alert(`${num1} + ${num2} = ${answer} is ${num1 + num2 === answer}`)
console.log(`${num1} + ${num2} = ${answer} is ${num1 + num2 === answer}`)
```

</details>

---

## Guess Birthday

Write a program that guesses a users birthday by:

* Initializing birthday to 0
* Asking the user if their birthday is in Sets 1-5
* Updating the birthday based on the user's answer
* Printing the birthday

```
# If birthday in Set 1, add 1 to birthday

# Set 1
1 3 5 7
9 11 13 15
17 19 21 23
25 27 29 31

# If birthday in Set 2, add 2 to birthday

# Set 2
2 3 6 7
10 11 14 15
18 19 22 23
26 27 30 31

# If birthday in Set 3, add 4 to birthday

# Set 3
4 5 6 7
12 13 14 15
20 21 22 23
28 29 30 31

# If birthday in Set 4, add 8 to birthday

# Set 4
8 9 10 11
12 13 14 15
24 25 26 27
28 29 30 31

# If birthday in Set 5, add 16 to birthday

# Set 5
16 17 18 19
20 21 22 23
24 25 26 27
28 29 30 31
```

<details>
  <summary>Python Solution</summary>

```py linenums="1"
day = 0

question1 = """
Is your birthday in Set1?
    1 3 5 7
    9 11 13 15
    17 19 21 23
    25 27 29 31
Enter 0 for No and 1 for Yes:  """

answer = int(input(question1))

if answer == 1:
    day += 1

question2 = """
Is your birthday in Set2?
    2 3 6 7
    10 11 14 15
    18 19 22 23
    26 27 30 31
Enter 0 for No and 1 for Yes:  """
answer = int(input(question2))

if answer == 1:
    day += 2

question3 = """
Is your birthday in Set3?
    4 5 6 7
    12 13 14 15
    20 21 22 23
    28 29 30 31
Enter 0 for No and 1 for Yes:  """
answer = int(input(question3))

if answer == 1:
    day += 4

question4 = """
Is your birthday in Set4?
    8 9 10 11
    12 13 14 15
    24 25 26 27
    28 29 30 31
Enter 0 for No and 1 for Yes:  """
answer = int(input(question4))

if answer == 1:
    day += 8

question5 = """
Is your birthday in Set5?
    16 17 18 19
    20 21 22 23
    24 25 26 27
    28 29 30 31
Enter 0 for No and 1 for Yes:  """
answer = int(input(question5))

if answer == 1:
    day += 16

print('\nYour birthday is {}!'.format(day))
```

</details>

<details>
  <summary>JavaScript Solution</summary>

```js linenums="1"
var day = 0
var answer = 0

var question1 = `
Is your birthday in Set1?
    1 3 5 7
    9 11 13 15
    17 19 21 23
    25 27 29 31
Enter 0 for No and 1 for Yes:  `

answer = parseInt(prompt(question1))

if(answer === 1)
    day += 1

var question2 = `
Is your birthday in Set2?
    2 3 6 7
    10 11 14 15
    18 19 22 23
    26 27 30 31
Enter 0 for No and 1 for Yes:  `
answer = parseInt(prompt(question2))

if(answer === 1)
    day += 2

var question3 = `
Is your birthday in Set3?
    4 5 6 7
    12 13 14 15
    20 21 22 23
    28 29 30 31
Enter 0 for No and 1 for Yes:  `
answer = parseInt(prompt(question3))

if(answer === 1)
    day += 4

var question4 = `
Is your birthday in Set4?
    8 9 10 11
    12 13 14 15
    24 25 26 27
    28 29 30 31
Enter 0 for No and 1 for Yes:  `
answer = parseInt(prompt(question4))

if(answer === 1)
    day += 8

var question5 = `
Is your birthday in Set5?
    16 17 18 19
    20 21 22 23
    24 25 26 27
    28 29 30 31
Enter 0 for No and 1 for Yes:  `
answer = parseInt(prompt(question5))

if(answer === 1)
    day += 16

alert(`Your birthday is ${day}!`)
console.log(`Your birthday is ${day}!`)
```

</details>

---
