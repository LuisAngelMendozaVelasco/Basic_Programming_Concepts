# Booleans

## Create a bool (boolean) type

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            bool isCSharpFun = true;
            bool isFishTasty = false;

            Console.WriteLine(isCSharpFun);   // Outputs True
            Console.WriteLine(isFishTasty);   // Outputs False
        }
    }
}
```

Output:

```text
True
False
```

## Find out if an expression is true or false

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int x = 10;
            int y = 9;
            
            Console.WriteLine(x > y); // returns True, because 10 is higher than 9
        }
    }
}
```

Output:

```text
True
```

## Use the "equal to" operator to evaluate a boolean expression

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int x = 10;
            
            Console.WriteLine(x == 10); // returns True, because the value of x is equal to 10    
        }
    }
}
```

Output:

```text
True
```