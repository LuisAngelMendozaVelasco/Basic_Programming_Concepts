# Classes

## Create an object of a class and access class attributes

Code:

```cpp
#include <iostream>
#include <string> 
using namespace std;

class MyClass {          // The class
    public:              // Access specifier
        int myNum;       // Attribute (int variable)
        string myString; // Attribute (string variable)
};

int main() {
    MyClass myObj;  // Create an object of MyClass

    // Access attributes and set values
    myObj.myNum = 15;
    myObj.myString = "Some text";

    // Print values
    cout << myObj.myNum << "\n"; 
    cout << myObj.myString << endl; 

    return 0;
}
```

Output:

```text
15
Some text
```

## Create multiple objects

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

class Car {
    public:
        string brand;
        string model;
        int year;
};

int main() {
    Car carObj1;
    carObj1.brand = "BMW";
    carObj1.model = "X5";
    carObj1.year = 1999;

    Car carObj2;
    carObj2.brand = "Ford";
    carObj2.model = "Mustang";
    carObj2.year = 1969;

    cout << carObj1.brand << " " << carObj1.model << " " << carObj1.year << "\n";
    cout << carObj2.brand << " " << carObj2.model << " " << carObj2.year << "\n";

    return 0;
}
```

Output:

```text
BMW X5 1999
Ford Mustang 1969
```

## Create class methods

Code:

```cpp
#include <iostream>
using namespace std;

class MyClass {         // The class
    public:               // Access specifier
        void myMethod() {   // Method/function
            cout << "Hello World!" << endl;
        }
};

int main() {
    MyClass myObj;     // Create an object of MyClass
    
    myObj.myMethod();  // Call the method

    return 0;
}
```

Output:

```text
Hello World!
```

## Define a class method outside the class definition

Code:

```cpp
#include <iostream>
using namespace std;

class MyClass {             // The class
    public:                 // Access specifier
        void myMethod();    // Method/function declaration
};

// Method/function definition outside the class
void MyClass::myMethod() {
    cout << "Hello World!" << endl;
}

int main() {
    MyClass myObj;     // Create an object of MyClass

    myObj.myMethod();  // Call the method

    return 0;
}
```

Output:

```text
Hello World!
```

## Add parameters to a class method

Code:

```cpp
#include <iostream>
using namespace std;

class Car {
    public:
        int speed(int maxSpeed);
};

int Car::speed(int maxSpeed) {
    return maxSpeed;
}

int main() {
    Car myObj;

    cout << myObj.speed(200) << endl;

    return 0;
}
```

Output:

```text
200
```

## Create a constructor

Code:

```cpp
#include <iostream>
using namespace std;

/*
A constructor in C++ is a special method that is automatically called when an object of a class is created.
To create a constructor, use the same name as the class, followed by parentheses ().
*/
class MyClass {         // The class
    public:             // Access specifier
        MyClass() {     // Constructor
            cout << "Hello World!" << endl;
        }
};

int main() {
    MyClass myObj;    // Create an object of MyClass (this will call the constructor)

    return 0;
}
```

Output:

```text
Hello World!
```

## Constructor parameters

Code:

```cpp
#include <iostream>
using namespace std;

class Car {        // The class
    public:          // Access specifier
        string brand;  // Attribute
        string model;  // Attribute
        int year;      // Attribute
        Car(string x, string y, int z) {  // Constructor with parameters
            brand = x;
            model = y;
            year = z;
        }
};

int main() {
    // Create Car objects and call the constructor with different values
    Car carObj1("BMW", "X5", 1999);
    Car carObj2("Ford", "Mustang", 1969);

    // Print values
    cout << carObj1.brand << " " << carObj1.model << " " << carObj1.year << "\n";
    cout << carObj2.brand << " " << carObj2.model << " " << carObj2.year << "\n";

    return 0;
}
```

Output:

```text
BMW X5 1999
Ford Mustang 1969
```

## Constructor defined outside the class

Code:

```cpp
#include <iostream>
using namespace std;

class Car {             // The class
    public:             // Access specifier
        string brand;   // Attribute
        string model;   // Attribute
        int year;       // Attribute
        Car(string x, string y, int z); // Constructor declaration
};

// Constructor definition outside the class
Car::Car(string x, string y, int z) {
    brand = x;
    model = y;
    year = z;
}

int main() {
    // Create Car objects and call the constructor with different values
    Car carObj1("BMW", "X5", 1999);
    Car carObj2("Ford", "Mustang", 1969);

    // Print values
    cout << carObj1.brand << " " << carObj1.model << " " << carObj1.year << "\n";
    cout << carObj2.brand << " " << carObj2.model << " " << carObj2.year << "\n";

    return 0;
}
```

Output:

```text
BMW X5 1999
Ford Mustang 1969
```

## Public and private specifiers

Code:

```cpp
#include <iostream>
using namespace std;

class MyClass {
    public:     // Public access specifier
        int x;  // Public attribute
    private:    // Private access specifier
        int y;  // Private attribute
};

int main() {
    MyClass myObj;

    myObj.x = 25;   // Allowed (x is public)
    //myObj.y = 50; // Not allowed (y is private)

    cout << myObj.x << endl;

    return 0;
}
```

Output:

```text
25
```

## Encapsulation - hide sensitive data from users

Code:

```cpp
#include <iostream>
using namespace std;

/*
The meaning of Encapsulation, is to make sure that "sensitive" data is hidden from users. To achieve this, you must declare class variables/attributes as private 
(cannot be accessed from outside the class). If you want others to read or modify the value of a private member, you can provide public get and set methods.

The salary attribute is private, which have restricted access.
The public setSalary() method takes a parameter (s) and assigns it to the salary attribute (salary = s).
The public getSalary() method returns the value of the private salary attribute.
Inside main(), we create an object of the Employee class. Now we can use the setSalary() method to set the value of the private attribute to 50000. 
Then we call the getSalary() method on the object to return the value.

Why Encapsulation?
It is considered good practice to declare your class attributes as private (as often as you can). Encapsulation ensures better control of your data, because you (or others) 
can change one part of the code without affecting other parts. Increased security of data.
*/

class Employee {
    private:
        int salary;
    public:
        void setSalary(int s) {
            salary = s;
        }
        int getSalary() {
            return salary;
        }
};

int main() {
    Employee myObj;

    myObj.setSalary(50000);
    cout << myObj.getSalary() << endl;

    return 0;
}
```

Output:

```text
50000
```

## Inheritance - inherit attributes and methods from one class to another

Code:

```cpp
/*
Inheritance
In C++, it is possible to inherit attributes and methods from one class to another. We group the "inheritance concept" into two categories:
- Derived class (child) - the class that inherits from another class.
- Base class (parent) - the class being inherited from.
To inherit from a class, use the : symbol.
*/

#include <iostream>
#include <string>
using namespace std;

// Base class
class Vehicle {
    public: 
        string brand = "Ford";
        void honk() {
            cout << "Tuut, tuut! \n" ;
        }
};

// Derived class
class Car: public Vehicle {
    public: 
        string model = "Mustang";
};

int main() {
    Car myCar;

    myCar.honk();
    cout << myCar.brand + " " + myCar.model << endl;

    return 0;
}
```

Output:

```text
Tuut, tuut! 
Ford Mustang
```

## Multilevel inheritance

Code:

```cpp
#include <iostream>
using namespace std;

// Parent class
class MyClass {
    public: 
        void myFunction() {
            cout << "Some content in parent class." << endl;
        }
};

// Child class
class MyChild: public MyClass {};

// Grandchild class 
class MyGrandChild: public MyChild {};

int main() {
    MyGrandChild myObj;
    
    myObj.myFunction();

    return 0;
}
```

Output:

```text
Some content in parent class.
```

## Multiple inheritance

Code:

```cpp
#include <iostream>
using namespace std;

// Base class
class MyClass {
    public:
        void myFunction() {
            cout << "Some content in parent class.\n" ;
        }
};

// Another base class
class MyOtherClass {
    public:
        void myOtherFunction() {
            cout << "Some content in another class.\n" ;
        }
};

// Derived class
class MyChildClass: public MyClass, public MyOtherClass {};

int main() {
    MyChildClass myObj;

    myObj.myFunction();
    myObj.myOtherFunction();

    return 0;
}
```

Output:

```text
Some content in parent class.
Some content in another class.
```

## Polymorphism - perform a single action in different ways

Code:

```cpp
/*
Polymorphism means "many forms", and it occurs when we have many classes that are related to each other by inheritance.
Like we specified in the previous chapter; Inheritance lets us inherit attributes and methods from another class. 
Polymorphism uses those methods to perform different tasks. This allows us to perform a single action in different ways.
For example, think of a base class called Animal that has a method called animalSound(). 
Derived classes of Animals could be Pigs, Cats, Dogs, Birds - And they also have their own implementation of an animal sound (the pig oinks, and the cat meows, etc.).
*/

#include <iostream>
#include <string>
using namespace std;

// Base class
class Animal {
    public:
        void animalSound() {
            cout << "The animal makes a sound \n" ;
        }
};

// Derived class
class Pig : public Animal {
    public:
        void animalSound() {
            cout << "The pig says: wee wee \n" ;
        }
};

// Derived class
class Dog : public Animal {
    public:
        void animalSound() {
            cout << "The dog says: bow wow \n" ;
        }
};

int main() {
    Animal myAnimal;
    Pig myPig;
    Dog myDog;

    myAnimal.animalSound();
    myPig.animalSound();
    myDog.animalSound();

    return 0;
}
```

Output:

```text
The animal makes a sound
The pig says: wee wee
The dog says: bow wow
```

## Exceptions - Handle errors

Code:

```cpp
/*
When executing C++ code, different errors can occur: coding errors made by the programmer, errors due to wrong input, or other unforeseeable things.
When an error occurs, C++ will normally stop and generate an error message. The technical term for this is: C++ will throw an exception (throw an error).

Exception handling in C++ consist of three keywords: try, throw and catch:
The try statement allows you to define a block of code to be tested for errors while it is being executed.
The throw keyword throws an exception when a problem is detected, which lets us create a custom error.
The catch statement allows you to define a block of code to be executed, if an error occurs in the try block.
The try and catch keywords come in pairs.
*/

#include <iostream>
using namespace std;

int main() {
    try {
        int age = 15;

        if(age >= 18) {
            cout << "Access granted - you are old enough." << endl;
        } 
        else {
            throw(age);
        }
    }
    catch(int myNum) {
        cout << "Access denied - You must be at least 18 years old.\n";
        cout << "Age is: " << myNum << endl;  
    }

    return 0;
}
```

Output:

```text
Access denied - You must be at least 18 years old.
Age is: 15
```