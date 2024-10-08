# Exceptions

## The try...catch statement

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            try
            {
                int[] myNumbers = {1, 2, 3};

                Console.WriteLine(myNumbers[10]);
            }
            catch(Exception)
            {
                Console.WriteLine("Something went wrong!");
            }  
        }
    }
}
```

Output:

```text
Something went wrong!
```

## The finally statement

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            try
            {
                int[] myNumbers = {1, 2, 3};

                Console.WriteLine(myNumbers[10]);
            }
            catch(Exception)
            {
                Console.WriteLine("Something went wrong!");
            }  
            finally
            {
                Console.WriteLine("The 'try catch' is finished!");
            }    
        }
    }
}
```

Output:

```text
Something went wrong!
The 'try catch' is finished!
```