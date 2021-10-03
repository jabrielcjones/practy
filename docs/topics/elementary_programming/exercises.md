# Elementary Programming Exercises

## Display 3 Different Messages

Write a program that:

* displays, on 3 separate lines, the following messages

```text
Welcome to {YOUR PROG. LANGUAGE}
Welcome to Computer Science
Programming is Fun
```

<details>
  <summary>Python Solution:</summary>

```py linenums="1"
print('Welcome to Python!')
print('Welcome to Computer Science!')
print('Programming is Fun!')
```

</details>

<details>
  <summary>JavaScript Solution:</summary>

```js linenums="1"
alert('Welcome to JavaScript!')
console.log('Welcome to JavaScript!')

alert('Welcome to Computer Science!')
console.log('Welcome to Computer Science!')

alert('Programming is Fun!')
console.log('Programming is Fun!')
```

</details>

<details>
  <summary>C# Solution:</summary>

```csharp linenums="1"
using System;  

namespace Test  
{  
   class TestClass  
   {  
     static void Main(string[] args)  
     {  
       Console.WriteLine("Welcome to C#!");
       Console.WriteLine("Welcome to Computer Science!");
       Console.WriteLine("Programming is Fun!");
     }  
   }  
}
```

</details>

---

## Display a Message n Times

Write a program that:

* Displays the following message 5 times

```text
Welcome to {YOUR PROG. LANGUAGE}
```

<details>
  <summary>C# Solution:</summary>

```csharp linenums="1"
using System;
using System.Text; 

namespace repeatStringXTimes
{  
   class Program 
   {  
     static void Main(string[] args)  
     {  
       string str = new StringBuilder("Welcome to C#! ".Length * 5).Insert(0, "Welcome to C#! ", 5).ToString();
       Console.WriteLine(str);
     }  
   }  
}
```

</details>

---

## Compute the Area of a Circle

Write a program that:

* Gets a circle's radius from a user
* Uses it to compute the area of a circle
* Prints the area to the screen.

```text
area = radius * PI

PI = 3.14159
```

!!! Tip
    Try using a math library to get the value of PI

<details>
  <summary>Python Solution:</summary>

Solution #1

```py linenums="1"
radius = input('Enter the radius of a circle: ')

area = radius * radius * 3.14159

print(f'The area for the circle of radius {radius} is {area}')
```

Solution #2

```py linenums="1"
import math

radius = input('Enter the radius of a circle: ')

area = pow(radius, 2) * math.pi

print(f'The area for the circle of radius {radius} is {area}')
```

</details>

<details>
  <summary>JavaScript Solution:</summary>

Solution #1

```js linenums="1"
let radius = prompt('Enter the radius of a circle: ')

let area = radius * radius * 3.14159

alert(`The area for the circle of radius ${radius} is ${area}`)
console.log(`The area for the circle of radius ${radius} is ${area}`)
```

Solution #2

```js linenums="1"
let radius = prompt('Enter the radius of a circle: ')

let area = Math.pow(radius, 2) * Math.PI

alert(`The area for the circle of radius ${radius} is ${area}`)
console.log(`The area for the circle of radius ${radius} is ${area}`)
```

</details>

<details>
	<summary>C# Solution:</summary>

Solution #1

```csharp linenums="1"
using System;  

namespace Test  
{  
   class TestClass  
   {  
     static void Main(string[] args)  
     {  
       string input;
       int radius;

       Console.WriteLine("Enter the radius of a circle: ");

       input = Console.ReadLine();

       radius = Convert.ToInt32(input);
       double area = radius * radius * 3.14159;

       Console.WriteLine("The area for the circle of radius {0} is {1}.", radius, area);
     }  
   }  
}
```

Solution #2

```csharp linenums="1"
using System;  

namespace Test  
{  
   class TestClass  
   {  
     static void Main(string[] args)  
     {  
       string input;
       int radius;

       Console.WriteLine("Enter the Radius of a Circle: ");

       input = Console.ReadLine();

       radius = Convert.ToInt32(input);

       double area = Math.Pow(radius, 2.0) * Math.PI;

       Console.WriteLine("The area for the circle of radius {0} is {1}.", radius, area);
     }  
   }  
}
```

</details>
