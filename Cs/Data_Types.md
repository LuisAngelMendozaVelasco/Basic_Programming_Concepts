# Data Types

## A demonstration of different data types in C#

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int myNum = 5;               // integer (whole number)
            double myDoubleNum = 5.99D;  // floating point number
            char myLetter = 'D';         // character
            bool myBool = true;          // boolean
            string myText = "Hello";     // string
            
            Console.WriteLine(myNum);
            Console.WriteLine(myDoubleNum);
            Console.WriteLine(myLetter);
            Console.WriteLine(myBool);
            Console.WriteLine(myText);       
        }
    }
}
```

Output:

```text
5
5.99
D
True
Hello
```

## Create an int type

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int myNum = 100000;

            Console.WriteLine(myNum);       
        }
    }
}
```

Output:

```text
100000
```

## Create a long type

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            long myNum = 15000000000L;

            Console.WriteLine(myNum);       
        }
    }
}
```

Output:

```text
15000000000
```

## Create a float type

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            float myNum = 5.75F;

            Console.WriteLine(myNum);       
        }
    }
}
```

Output:

```text
5.75
```

## Create a double type

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            double myNum = 19.99D;

            Console.WriteLine(myNum);       
        }
    }
}
```

Output:

```text
19.99
```

## Create a bool type

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

## Create a char type

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            char myGrade = 'B';

            Console.WriteLine(myGrade);       
        }
    }
}
```

Output:

```text
B
```

## Create a string type

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string greeting = "Hello World";

            Console.WriteLine(greeting);       
        }
    }
}
```

Output:

```text
Hello World
```