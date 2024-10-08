# Operators

## Addition operator

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int x = 5;
            int y = 3;
            
            Console.WriteLine(x + y);
        }
    }
}
```

Output:

```text
8
```

## Subtraction operator

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int x = 5;
            int y = 3;
            
            Console.WriteLine(x - y);
        }
    }
}
```

Output:

```text
2
```

## Multiplication operator

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int x = 5;
            int y = 3;

            Console.WriteLine(x * y);
        }
    }
}
```

Output:

```text
15
```

## Division operator

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int x = 12;
            int y = 3;

            Console.WriteLine(x / y);
        }
    }
}
```

Output:

```text
4
```

## Modulus operator

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int x = 5;
            int y = 2;

            Console.WriteLine(x % y);       
        }
    }
}
```

Output:

```text
1
```

## Increment operator

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int x = 5;

            x++;
            Console.WriteLine(x);
        }
    }
}
```

Output:

```text
6
```

## Decrement operator

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int x = 5;
            
            x--;
            Console.WriteLine(x);       
        }
    }
}
```

Output:

```text
4
```

## Assignment operator

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

            Console.WriteLine(x);       
        }
    }
}
```

Output:

```text
10
```

## Addition assignment operator

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
            
            x += 5;
            Console.WriteLine(x);       
        }
    }
}
```

Output:

```text
15
```