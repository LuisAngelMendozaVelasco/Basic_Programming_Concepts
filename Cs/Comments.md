# Comments

## Single-line comment before a line of code

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            // This is a comment
            Console.WriteLine("Hello World!");
        }
    }
}

```

Output:

```text
Hello World!
```

## Single-line comment at the end of a line of code

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");  // This is a comment
        }
    }
}
```

Output:

```text
Hello World!
```

## Multi-line comment

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            /* 
            The code below will print the words Hello World
            to the screen, and it is amazing 
            */
            Console.WriteLine("Hello World!");
        }
    }
}
```

Output:

```text
Hello World!
```