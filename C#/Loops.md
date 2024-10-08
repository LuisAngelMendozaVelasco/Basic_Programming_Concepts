# Loops

## While loop

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int i = 0;

            while(i < 5) 
            {
                Console.WriteLine(i);
                i++;
            }     
        }
    }
}
```

Output:

```text
0
1
2
3
4
```

## Do while loop

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            int i = 0;

            do 
            {
                Console.WriteLine(i);
                i++;
            }
            while(i < 5);     
        }
    }
}
```

Output:

```text
0
1
2
3
4
```

## For loop

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            for (int i = 0; i < 5; i++) 
            {
                Console.WriteLine(i);
            }   
        }
    }
}
```

Output:

```text
0
1
2
3
4
```

## foreach loop

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] cars = {"Volvo", "BMW", "Ford", "Mazda"}; // Declare a single-dimensional

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

## Break a loop

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            for(int i = 0; i < 10; i++) 
            {
                if(i == 4) 
                {
                    break;
                }
                
                Console.WriteLine(i);
            }     
        }
    }
}
```

Output:

```text
0
1
2
3
```

## Continue a loop

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            for (int i = 0; i < 10; i++) 
            {
                if (i == 4) 
                {
                    continue;
                }

                Console.WriteLine(i);
            }      
        }
    }
}
```

Output:

```text
0
1
2
3
5
6
7
8
9
```