# Type Casting

## Implicit casting

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int myInt = 9;
            double myDouble = myInt;  // Automatic casting: int to double

            Console.WriteLine(myInt);
            Console.WriteLine(myDouble);       
        }
    }
}
```

Output:

```text
9
9
```

## Explicit casting

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            double myDouble = 9.78;
            int myInt = (int) myDouble;  // Manual casting: double to int

            Console.WriteLine(myDouble);
            Console.WriteLine(myInt);       
        }
    }
}
```

Output:

```text
9.78
9
```

## Type conversion methods

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int myInt = 10;
            double myDouble = 5.25;
            bool myBool = true;

            Console.WriteLine(Convert.ToString(myInt));    // Convert int to string
            Console.WriteLine(Convert.ToDouble(myInt));    // Convert int to double
            Console.WriteLine(Convert.ToInt32(myDouble));  // Convert double to int
            Console.WriteLine(Convert.ToString(myBool));   // Convert bool to string       
        }
    }
}
```

Output:

```text
10
10
5
True
```