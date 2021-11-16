# Functions Exercises

## Conversions Between Celsius and Fahrenheit

Write a module that contains the following two functions:

```text
# Converts from celcius to fahrenheit
def celsiusToFahrenheit(celsius):

# Converts from fahrenheit to celsius
def fahrenheitToCelsius(fahrenheit):

The formulas for the conversions are:

celsius = (5 / 9) * (fahrenheit - 32)
fahrenheit = (9 / 5) * (celsius + 32)
```

Write a test program that invokes these functions to display the following tables:

```text
Celsius   Fahrenheit   |   Fahrenheit   Celsius

40.0      104.0        |   120.0        48.89
39.0      102.2        |   110.0        43.33
...
32.0      89.6         |   40.0         4.44
31.0      87.8         |   30.0         -1.11
```

<details>
  <summary>Python Solution:</summary>

```py linenums="1"
def celsiusToFahrenheit(celsius):
    """
    """

    return (9 / 5) * (celsius + 32)


def fahrenheitToCelsius(fahrenheit):
    """
    """

    return (5 / 9) * (fahrenheit - 32)


def conversion_table():
    """
    """

    print("Celsius     Fahrenheit")
    print("")
    for i in reversed(range(31, 41)):
        fahrenheit = round(celsiusToFahrenheit(i), 1)
        print(f"{i}          {fahrenheit}")

    print("")

    print("Fahrenheit     Celsius")
    print("")
    for i in reversed(range(30, 130, 10)):
        celsius = round(fahrenheitToCelsius(i), 1)
        print(f"{i}             {celsius}")


conversion_table()
```

</details>
