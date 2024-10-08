# Classes

## Create a class and an object of a class

Code:

```csharp
using System;

namespace MyApplication
{
    class Car
    {
        string color = "red";

        static void Main(string[] args)
        {
            Car myObj = new Car(); // To create an object of Car, specify the class name, followed by the object name, and use the keyword new

            Console.WriteLine(myObj.color);  
        }
    }
}
```

Output:

```text
red
```

## Create multiple objects of a class

Code:

```csharp
using System;

namespace MyApplication
{
    class Car
    {
        string color = "red";

        static void Main(string[] args)
        {
            Car myObj1 = new Car();
            Car myObj2 = new Car();

            Console.WriteLine(myObj1.color);
            Console.WriteLine(myObj2.color);  
        }
    }
}
```

Output:

```text
red
red
```

## Use multiple classes for better organization

Code:

```csharp
using System;

namespace MyApplication
{
    class Car
    {
        public string color = "red";
    }
}
```

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            Car myObj = new Car();
            
            Console.WriteLine(myObj.color);  
        }
    }
}
```

Output:

```text
red
```

## Access fields and methods

Code:

```csharp
using System;

namespace MyApplication
{
    class Car
    {
        public string? model;
        public string? color;
        public int year;

        public void fullThrottle()
        {
            Console.WriteLine("The car is going as fast as it can!"); 
        }
    }
}
```

```csharp
sing System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            Car Ford = new Car();

            Ford.model = "Mustang";
            Ford.color = "red";
            Ford.year = 1969;
            Console.WriteLine(Ford.model);
            Console.WriteLine(Ford.color);
            Console.WriteLine(Ford.year);
            Ford.fullThrottle();

            Console.Write($"{Environment.NewLine}");
    
            Car Opel = new Car();

            Opel.model = "Astra";
            Opel.color = "white";
            Opel.year = 2005;
    
            Console.WriteLine(Opel.model);
            Console.WriteLine(Opel.color);
            Console.WriteLine(Opel.year);
            Opel.fullThrottle();  
        }
    }
}
```

Output:

```text
red
```

## Create a class constructor

Code:

```csharp
using System;

namespace MyApplication
{
    // Create a Car class
    class Car
    {
        public string model;  // Create a field

        // Create a class constructor for the Car class
        public Car()
        {
            model = "Mustang"; // Set the initial value for model
        }

        static void Main(string[] args)
        {
            Car Ford = new Car();  // Create an object of the Car Class (this will call the constructor)

            Console.WriteLine(Ford.model);  // Print the value of model  
        }
    }
}
```

Output:

```text
Mustang
```

## Constructor with parameters

Code:

```csharp
using System;

namespace MyApplication
{
    class Car
    {
        public string model;
        public string color;
        public int year;
    ​
        // Create a class constructor with multiple parameters
        public Car(string modelName, string modelColor, int modelYear)
        {
            model = modelName;
            color = modelColor;
            year = modelYear;
        }
    ​
        static void Main(string[] args)
        {
            Car Ford = new Car("Mustang", "Red", 1969);
            Console.WriteLine(Ford.color + " " + Ford.year + " " + Ford.model);
        }
    }
}
```

Output:

```text
Red 1969 Mustang
```

## Private modifier

Code:

```csharp
using System;

namespace MyApplication
{
    class Car
    {
        private string model = "Mustang"; // The code is only accessible within the same class

        static void Main(string[] args)
        {
            Car myObj = new Car();

            Console.WriteLine(myObj.model);
        }
    }
}
```

Output:

```text
Mustang
```

## Public modifier

Code:

```csharp
using System;

namespace MyApplication
{
    class Car
    {
        public string model = "Mustang"; //The code is accessible for all classes
    }
}
```

```csharp
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            Car myObj = new Car();
            
            Console.WriteLine(myObj.model);
        }
    }
}
```

Output:

```text
Mustang
```

## Properties (get and set)

Code:

```csharp
/*
The Name property is associated with the name field. It is a good practice to use the same name for both the property and the private field, but with an uppercase first letter.
The get method returns the value of the variable name.
The set method assigns a value to the name variable. The value keyword represents the value we assign to the property.
*/

using System;

namespace MyApplication
{
    class Person
    {
        private string? name;  // field

        public string? Name    // property
        {
            get{return name;}
            set{name = value;}
        }  
    }
}
```

```csharp
/*
The meaning of Encapsulation, is to make sure that "sensitive" data is hidden from users. To achieve this, you must:
* declare fields/variables as private.
* provide public get and set methods, through properties, to access and update the value of a private field.
A property is like a combination of a variable and a method, and it has two methods: a get and a set method.
*/

using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            Person myObj = new Person();

            myObj.Name = "Liam";
            Console.WriteLine(myObj.Name);
        }
    }
}

```

Output:

```text
Liam
```

## Automatic (short-hand) properties

Code:

```csharp
/*
C# also provides a way to use short-hand / automatic properties, where you do not have to define the field for the property, 
and you only have to write get; and set; inside the property.
*/

using System;

namespace MyApplication
{
    class Person
    {
        public string? Name // property
        {
            get; 
            set;
        }  
    }
}
```

```csharp

namespace MyApplication
{
    class Program
    {  
        static void Main(string[] args)
        {
            Person myObj = new Person();

            myObj.Name = "Liam";
            Console.WriteLine(myObj.Name);  
        }
    }
}
```

Output:

```text
Liam
```

## Inheritance

Code:

```csharp
using System;

namespace MyApplication
{
    class Vehicle  // Base class
    {
        public string brand = "Ford";  // Vehicle field
        
        public void honk()             // Vehicle method 
        {
            Console.WriteLine("Tuut, tuut!");
        }
    }
}
```

```csharp
using System;

namespace MyApplication
{
    class Car : Vehicle  // Derived class
    {
        public string modelName = "Mustang";  // Car field
    }
}
```

```csharp
using System;

namespace MyApplication
{
    class Program
    { 
        static void Main(string[] args)
        {
            // Create a myCar object
            Car myCar = new Car();

            // Call the honk() method (From the Vehicle class) on the myCar object
            myCar.honk();

            // Display the value of the brand field (from the Vehicle class) and the value of the modelName from the Car class
            Console.WriteLine(myCar.brand + " " + myCar.modelName);  
        }
    }
}
```

Output:

```text
Tuut, tuut!
Ford Mustang
```

## Polymorphism

Code:

```csharp
// Polymorphism means "many forms", and it occurs when we have many classes that are related to each other by inheritance.

using System;

namespace MyApplication
{
    class Animal  // Base class (parent) 
    {
        public virtual void animalSound()
        {
            Console.WriteLine("The animal makes a sound");
        }
    }

    class Pig : Animal  // Derived class (child) 
    {
        public override void animalSound()
        {
            Console.WriteLine("The pig says: wee wee");
        }
    }

    class Dog : Animal  // Derived class (child) 
    {
        public override void animalSound()
        {
            Console.WriteLine("The dog says: bow wow");
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            Animal myAnimal = new Animal();  // Create a Animal object
            Animal myPig = new Pig();  // Create a Pig object
            Animal myDog = new Dog();  // Create a Dog object
            
            myAnimal.animalSound();
            myPig.animalSound();
            myDog.animalSound();  
        }
    }
}
```

Output:

```text
The animal makes a sound
The pig says: wee wee
The dog says: bow wow
```

## Abstraction

Code:

```csharp
/*
Data abstraction is the process of hiding certain details and showing only essential information to the user.
Abstraction can be achieved with either abstract classes or interfaces.
The abstract keyword is used for classes and methods:
* Abstract class: is a restricted class that cannot be used to create objects (to access it, it must be inherited from another class).
* Abstract method: can only be used in an abstract class, and it does not have a body. The body is provided by the derived class (inherited from).
An abstract class can have both abstract and regular methods
*/

using System;

namespace MyApplication
{
    // Abstract class
    abstract class Animal
    {
        // Abstract method (does not have a body)
        public abstract void animalSound();

        // Regular method
        public void sleep()
        {
            Console.WriteLine("Zzz");
        }
    }
    
    // Derived class (inherit from Animal)
    class Pig : Animal
    {
        public override void animalSound()
        {
            // The body of animalSound() is provided here
            Console.WriteLine("The pig says: wee wee");
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            Pig myPig = new Pig();  // Create a Pig object

            myPig.animalSound();
            myPig.sleep();  
        }
    }
}
```

Output:

```text
The pig says: wee wee
Zzz
```

## Interface

Code:

```csharp
/*
Another way to achieve abstraction in C#, is with interfaces.
An interface is a completely "abstract class", which can only contain abstract methods and properties (with empty bodies).
By default, members of an interface are abstract and public.
*/

/*
Notes on Interfaces:
* Like abstract classes, interfaces cannot be used to create objects (in the example above, it is not possible to create an "IAnimal" object in the Program class).
* Interface methods do not have a body - the body is provided by the "implement" class.
* On implementation of an interface, you must override all of its methods.
* Interfaces can contain properties and methods, but not fields/variables.
* Interface members are by default abstract and public.
* An interface cannot contain a constructor (as it cannot be used to create objects).

Why And When To Use Interfaces?
1) To achieve security - hide certain details and only show the important details of an object (interface).
2) C# does not support "multiple inheritance" (a class can only inherit from one base class). 
However, it can be achieved with interfaces, because the class can implement multiple interfaces. 
Note: To implement multiple interfaces, separate them with a comma.
*/

using System;

namespace MyApplication
{
    // Interface
    interface IAnimal 
    {
        void animalSound(); // interface method (does not have a body)
    }

    // Pig "implements" the IAnimal interface
    class Pig : IAnimal 
    {
        public void animalSound() 
        {
            // The body of animalSound() is provided here
            Console.WriteLine("The pig says: wee wee");
        }
    }

    class Program 
    {
        static void Main(string[] args) 
        {
            Pig myPig = new Pig();  // Create a Pig object
            
            myPig.animalSound();  
        }
    }
}   
```

Output:

```text
The pig says: wee wee
```

## Multiple interfaces

Code:

```csharp
using System;

namespace MyApplication
{
    interface IFirstInterface
    {
        void myMethod(); // interface method
    }

    interface ISecondInterface
    {
        void myOtherMethod(); // interface method
    }

    // Implement multiple interfaces
    class DemoClass : IFirstInterface, ISecondInterface
    {
        public void myMethod()
        {
            Console.WriteLine("Some text..");
        }
        public void myOtherMethod()
        {
            Console.WriteLine("Some other text...");
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            DemoClass myObj = new DemoClass();

            myObj.myMethod();
            myObj.myOtherMethod();  
        }
    }
}
```

Output:

```text
Some text..
Some other text...
```

## Enums

Code:

```csharp
/*
An enum is a special "class" that represents a group of constants (unchangeable/read-only variables).
To create an enum, use the enum keyword (instead of class or interface), and separate the enum items with a comma.
Enum is short for "enumerations", which means "specifically listed".

Use enums when you have values that you know aren't going to change, like month days, days, colors, deck of cards, etc.
*/

using System;

namespace MyApplication
{
    enum Level
    {
        Low,
        Medium,
        High
    }

    class Program
    {
        static void Main(string[] args)
        {
            Level myVar = Level.Medium;

            Console.WriteLine(myVar);  
        }
    }
}
```

Output:

```text
Medium
```

## Working with files

Code:

```csharp
using System;
using System.IO;  // include the System.IO namespace

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            string writeText = "Hello World!";  // Create a text string

            File.WriteAllText("filename.txt", writeText);  // Create a file and write the contents of writeText to it

            string readText = File.ReadAllText("filename.txt"); // Read the contents of the file

            Console.WriteLine(readText); // Output the content

            File.Delete("filename.txt"); // Delete the file  
        }
    }
}
```

Output:

```text
Hello World!
```