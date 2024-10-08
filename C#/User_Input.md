# User Input

## Get user input text

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            // Type your username and press enter
            Console.WriteLine("Enter username:");

            // Create a string variable and get user input from the keyboard and store it in the variable
            string? userName = Console.ReadLine();

            // Print the value of the variable (userName), which will display the input value
            Console.WriteLine("\nUsername is: " + userName);
        }
    }
}
```

Output:

```text
Enter username:
Luis

Username is: Luis
```

## Get user input with numbers

Code:

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Enter your age: ");

            int age = Convert.ToInt32(Console.ReadLine());

            Console.WriteLine("\nYour age is: " + age);   
        }
    }
}
```

Output:

```text
Enter your age: 
29

Your age is: 29
```