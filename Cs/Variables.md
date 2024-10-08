# Variables

## Create a string variable

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string name = "Luis";

            Console.WriteLine(name);       
        }
    }
}
```

Output:

```text
Luis
```

## Create an integer variable

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int myNum = 15;

            Console.WriteLine(myNum);       
        }
    }
}
```

Output:

```text
15
```

## Create a variable without assigning the value, and assign the value later

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int myNum;

            myNum = 15;
            Console.WriteLine(myNum);
        }
    }
}
```

Output:

```text
15
```

## Overwrite an existing variable value

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int myNum = 15;

            myNum = 20;
            Console.WriteLine(myNum);       
        }
    }
}
```

Output:

```text
20
```

## Combine text and a variable on display

Code:

```csharp
using System;

namespace MyApplication
{
  class Program
    {
        static void Main(string[] args)
        {
            string name = "Luis";
            
            Console.WriteLine("Hello " + name);       
        }
    }
}
```

Output:

```text
Hello Luis
```

## Add a variable to another variable

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string firstName = "Luis ";
            string lastName = "Mendoza";
            string fullName = firstName + lastName;

            Console.WriteLine(fullName);       
        }
    }
}
```

Output:

```text
Luis Mendoza
```

## Declare many variables of the same type with a comma-separated list

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int x = 5, y = 6, z = 50;

            Console.WriteLine(x + y + z);       
        }
    }
}
```

Output:

```text
61
```