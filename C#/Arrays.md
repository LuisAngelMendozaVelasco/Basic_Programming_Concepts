# Arrays

## Create and access an array

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};

            Console.WriteLine(cars[0]);          
        }
    }
}
```

Output:

```text
Volvo
```

## Change an array element

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};

            cars[0] = "Opel";
            Console.WriteLine(cars[0]);           
        }
    }
}
```

Output:

```text
Opel
```

## Find the length of an array

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};

            Console.WriteLine(cars.Length);          
        }
    }
}
```

Output:

```text
4
```

## Access and change an array element

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
            
            cars[0] = "Opel";
            Console.WriteLine(cars[0]);              
        }
    }
}
```

Output:

```text
Opel
```

## Loop through an array

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};

            for(int i = 0; i < cars.Length; i++) 
            {
                Console.WriteLine(cars[i]);
            }          
        }
    }
}
```

Output:

```text
Volvo
BMW
Ford
Mazda
```

## Loop through an array with foreach

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};

            foreach(string i in cars) 
            {
                Console.WriteLine(i);
            }             
        }
    }
}
```

Output:

```text
Volvo
BMW
Ford
Mazda
```

## Sort an array

Code:

```csharp

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            // Sort a string
            string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};

            Array.Sort(cars);

            foreach(string i in cars)
            {
                Console.WriteLine(i);
            }    
            
            Console.Write($"{Environment.NewLine}");

            // Sort an int
            int[] myNumbers = {5, 1, 8, 9};

            Array.Sort(myNumbers);
            
            foreach(int i in myNumbers)
            {
                Console.WriteLine(i);
            }          
        }
    }
}
```

Output:

```text
BMW
Ford
Mazda
Volvo

1
5
8
9
```

## Using System.Linq

Code:

```csharp
using System;
using System.Linq;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int[] myNumbers = {5, 1, 8, 9};

            Console.WriteLine(myNumbers.Max());  // largest value
            Console.WriteLine(myNumbers.Min());  // smallest value
            Console.WriteLine(myNumbers.Sum());  // sum of myNumbers          
        }
    }
}
```

Output:

```text
9
1
23
```