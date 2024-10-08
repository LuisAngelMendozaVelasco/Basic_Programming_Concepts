# Conditions

## The if statement

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            if(20 > 18) 
            {
                Console.WriteLine("20 is greater than 18!");
            }       
        }
    }
}
```

Output:

```text
20 is greater than 18!
```

## The else statement

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int time = 20;

            if (time < 18) 
            {
                Console.WriteLine("Good day!");
            } 
            else 
            {
                Console.WriteLine("Good evening!");
            }       
        }
    }
}
```

Output:

```text
Good evening!
```

## The else if statement

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int time = 22;

            if (time < 10) 
            {
                Console.WriteLine("Good morning!");
            } 
            else if (time < 20) 
            {
                Console.WriteLine("Good day!");
            } 
            else 
            {
                Console.WriteLine("Good evening!");
            }       
        }
    }
}
```

Output:

```text
Good evening!
```