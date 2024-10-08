# Strings

## Create a string

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string greeting = "Hello";

            Console.WriteLine(greeting);     
        }
    }
}
```

Output:

```text
Hello
```

## Find the length of a string

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

            Console.WriteLine("The length of the txt string is: " + txt.Length);         
        }
    }
}
```

Output:

```text
The length of the txt string is: 26
```

## Using methods to convert strings to uppercase and lowercase

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string txt = "Hello World";

            Console.WriteLine(txt.ToUpper());   // Outputs "HELLO WORLD"
            Console.WriteLine(txt.ToLower());   // Outputs "hello world"         
        }
    }
}
```

Output:

```text
HELLO WORLD
hello world
```

## String concatenation

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
            string name = firstName + lastName;

            Console.WriteLine(name);         
        }
    }
}
```

Output:

```text
Luis Mendoza
```

## String concatenation with the Concat() method

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
            string name = string.Concat(firstName, lastName);

            Console.WriteLine(name);         
        }
    }
}
```

Output:

```text
Luis Mendoza
```

## String interpolation

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string firstName = "Luis";
            string lastName = "Mendoza";
            string name = $"My full name is: {firstName} {lastName}";

            Console.WriteLine(name);         
        }
    }
}
```

Output:

```text
My full name is: Luis Mendoza
```

## Access characters in a string by referring to its index number

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string myString = "Hello";

            Console.WriteLine(myString[0]);         
        }
    }
}
```

Output:

```text
H
```

## Find the index position of a specific character in a string, by using the IndexOf() method

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string myString = "Hello";

            Console.WriteLine(myString.IndexOf("e"));         
        }
    }
}
```

Output:

```text
1
```

## Use the Substring() method together with the IndexOf() method

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main()
        {
            // Full name
            string name = "Luis Mendoza";

            // Location of the letter D
            int charPos = name.IndexOf("M");

            // Get last name
            string lastName = name.Substring(charPos);

            // Print the result
            Console.WriteLine(lastName);         
        }
    }
}
```

Output:

```text
Mendoza
```

## Use quotes in a string

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string txt = "We are the so-called \"Vikings\" from the north.";
            
            Console.WriteLine(txt);         
        }
    }
}
```

Output:

```text
We are the so-called "Vikings" from the north.
```