# Elementary Programming Exercises

## Display 3 Different Messages

Write a program that displays:

```
Welcome to {YOUR PROG. LANGUAGE}
Welcome to Computer Science
Programming is Fun
```

<details>
  <summary>Python Solution</summary>

```py linenums="1"
print('Welcome to Python!')
print('Welcome to Computer Science!')
print('Programming is Fun!')
```

</details>

<details>
  <summary>JavaScript Solution</summary>

```js linenums="1"
console.log('Welcome to JavaScript!')
console.log('Welcome to Computer Science!')
console.log('Programming is Fun!')
```

</details>

---

## Compute the Area of a Circle

Write a program that:

* Gets a circle's radius from a user
* Uses it to compute the area of a circle
* Prints the area to the screen.

```
area = radius * PI

PI = 3.14159
```

!!! Tip
    Try using a math library to get the value of PI

<details>
  <summary>Python Solution</summary>

Solution #1

```py linenums="1"
radius = input('Enter the radius of a circle: ')

area = radius * radius * 3.14159

print('The area for the circle of radius {0} is {1}'.format(radius, area))
```

Solution #2

```py linenums="1"
import math

radius = input('Enter the radius of a circle: ')

area = pow(radius, 2) * math.pi

print('The area for the circle of radius {0} is {1}'.format(radius, area))
```

</details>

<details>
  <summary>JavaScript Solution</summary>

```js linenums="1"
console.log('Welcome to JavaScript')
console.log('Welcome to Computer Science')
console.log('Programming is Fun')
```

</details>
