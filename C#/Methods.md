# Methods

## Create and call a method

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void MyMethod()
        {
            Console.WriteLine("I just got executed!");
        }

        static void Main(string[] args)
        {
            MyMethod();  
        }
    }
}
```

Output:

```text
I just got executed!
```

## Call a method multiple times

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void MyMethod()
        {
            Console.WriteLine("I just got executed!");
        }

        static void Main(string[] args)
        {
            MyMethod();
            MyMethod();
            MyMethod();  
        }
    }
}
```

Output:

```text
I just got executed!
I just got executed!
I just got executed!
```

## Method with parameters

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void MyMethod(string fname) 
        {
            Console.WriteLine(fname + " Refsnes");
        }

        static void Main(string[] args)
        {
            MyMethod("Liam");
            MyMethod("Jenny");
            MyMethod("Anja");  
        }
    }
}
```

Output:

```text
Liam Refsnes
Jenny Refsnes
Anja Refsnes
```

## Default parameter value

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void MyMethod(string country = "Norway")
        {
            Console.WriteLine(country);
        }

        static void Main(string[] args)
        {
            MyMethod("Sweden");
            MyMethod("India");
            MyMethod();
            MyMethod("USA");  
        }
    }
}
```

Output:

```text
Sweden
India
Norway
USA
```

## Multiple parameters

Code:

```csharp

namespace MyApplication
{
    class Program
    {
        static void MyMethod(string fname, int age)
        {
            Console.WriteLine(fname + " is " + age);
        }

        static void Main(string[] args)
        {
            MyMethod("Liam", 5);
            MyMethod("Jenny", 8);
            MyMethod("Anja", 31);  
        }
    }
}
```

Output:

```text
Liam is 5
Jenny is 8
Anja is 31
```

## Return value

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static int MyMethod(int x)
        {
            return 5 + x;
        }

        static void Main(string[] args)
        {
            Console.WriteLine(MyMethod(3));  
        }
    }
}
```

Output:

```text
8
```

## Return the sum of a method's two parameters

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static int MyMethod(int x, int y)
        {
            return x + y;
        }

        static void Main(string[] args)
        {
            int z = MyMethod(5, 3);

            Console.WriteLine(z);  
        }
    }
}
```

Output:

```text
8
```

## Named arguments

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void MyMethod(string child1, string child2, string child3)
        {
            Console.WriteLine("The youngest child is: " + child3);
        }

        static void Main(string[] args)
        {
            MyMethod(child3: "John", child1: "Liam", child2: "Liam");  
        }
    }
}
```

Output:

```text
The youngest child is: John
```

## Overload a method

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static int PlusMethod(int x, int y)
        {
            return x + y;
        }

        static double PlusMethod(double x, double y)
        {
            return x + y;
        }

        static void Main(string[] args)
        {
            int myNum1 = PlusMethod(8, 5);
            double myNum2 = PlusMethod(4.3, 6.26);

            Console.WriteLine("Int: " + myNum1);
            Console.WriteLine("Double: " + myNum2);  
        }
    }
}
```

Output:

```text
Int: 13
Double: 10.559999999999999
```