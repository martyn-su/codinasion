## Write a programme to convert years to days.

```
Input : 1
Output : 365
```

---

<CodeBlock slots="heading, code" repeat="3" languages="C#, Python, C" />

#### C#

```cs
using System;

public class YearsToDays
{
    static void Main(string[] args)
    {
        int YearsToDays(int years)
        {
            return years * 365;
        }

        // Input number of years
        Console.Write("Years : ");
        int years = int.Parse(Console.ReadLine());

        // Days output
        Console.WriteLine("Days  : " + YearsToDays(years));
    }
}
```

#### Python

```python
years = int(input("years : "))
print(f"\ndays  : {years * 365}")
```

#### C

```c
#include <stdio.h>

int main()
{
    int years, days;

    printf("Years : ");
    scanf("%d", &years);
    days = years * 365;
    printf("Days  : %d\n", days);
    return 0;
}
```
