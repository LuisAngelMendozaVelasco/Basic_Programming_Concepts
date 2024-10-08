# Syntax

## Create a simple "Hello World" program

Code:

```csharp
/*
Note: Every C# statement ends with a semicolon ;.
Note: C# is case-sensitive: "MyClass" and "myclass" has different meaning.
Note: Unlike Java, the name of the C# file does not have to match the class name, but they often do (for better organization).
*/

using System; // using System means that we can use classes from the System namespace

namespace MyApplication // namespace is used to organize your code, and it is a container for classes and other namespaces.
{ // The curly braces {} marks the beginning and the end of a block of code.

    /* 
    class is a container for data and methods, which brings functionality to your program. 
    Every line of code that runs in C# must be inside a class. In our example, we named the class Program.
    */
    class Program 
    {
        // Another thing that always appear in a C# program, is the Main method. Any code inside its curly brackets {} will be executed.
        static void Main(string[] args)
        {
            /* 
            Console is a class of the System namespace, which has a WriteLine() method that is used to output/print text. In our example it will output "Hello World!".  
            If you omit the using System line, you would have to write System.Console.WriteLine() to print/output text.
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