## Write a program to convert the temperature from Celsius to Fahrenheit

```
Input ( C )  : -40
Output ( F ) : -40
```

---

<CodeBlock slots="heading, code" repeat="5" languages="C, Python, C++, Java, C#" />

#### C

```c
#include <stdio.h>

void main()
{
  float c;
  printf("Enter temp. (in C) : ");
  scanf("%f", &c);
  float f = ((9 * c) / 5) + 32;
  printf("Temp. in F : %f\n", f);
}
```

#### Python

```python
def celsius_to_fahrenheit(celsius: int) -> float:
    """Converts celsius to farenheit"""
    fahrenheit = (celsius * 9 / 5) + 32
    return fahrenheit


if __name__ == '__main__':
    user_input = input('Enter celsius : ')
    print(f"\nFahrenheit : {celsius_to_fahrenheit(int(user_input))}")
```

#### C++

```cpp
#include <iostream>

using namespace std;

int main()
{

  float Fahrenheit; // initialize Fahrenheit
  float Celsius;    // initialize Celsius

  cout << "Enter the temperature in Celsius: ";
  cin >> Celsius;

  Fahrenheit = ((Celsius * 9.0) / 5.0) + 32;

  cout << "\nThe temperature in Celsius is: " << Celsius << endl;
  cout << "The temperature in Fahrenheit is: " << Fahrenheit << endl;
}
```

#### Java

```java
import java.util.Scanner;

class Celsius_to_Fahrenheit {
    public static void main(String[] args) {
        float cel, far;

        Scanner s = new Scanner(System.in);
        System.out.print("Input ( C )  : ");
        cel = s.nextInt();

        far = cel * 9 / 5 + 32;

        System.out.println("Output ( F ) : " + far);
    }
}
```

#### C#

```cs
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace codinasion
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Enter temp. (in C) : ");
            float temperature = float.Parse(Console.ReadLine());
            temperature = ((9 * temperature) / 5) + 32;
            Console.Write("Temp. in F : " + temperature + "\n");
        }
    }
}
```
