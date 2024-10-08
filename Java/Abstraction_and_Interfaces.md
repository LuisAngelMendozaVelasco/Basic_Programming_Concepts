# Abstraction & Interfaces

## Java abstract classes and methods

Code:

```java
// Abstract class
abstract class Animal {
    // Abstract method (does not have a body)
    public abstract void animalSound();

    // Regular method
    public void sleep() {
        System.out.println("Zzz...");
    }
}

// Subclass (inherit from Animal)
class Pig extends Animal {
    public void animalSound() {
        // The body of animalSound() is provided here
        System.out.println("The pig says: wee wee.");
    }
}

public class Main {
    public static void main(String[] args) {
        Pig myPig = new Pig(); // Create a Pig object
        
        myPig.animalSound();
        myPig.sleep();
    }
}
```

Output:

```text
The pig says: wee wee.
Zzz...
```

## Java interface (implements)

Code:

```java
/*
Another way to achieve abstraction in Java, is with interfaces.
An interface is a completely "abstract class" that is used to group related methods with empty bodies.
To access the interface methods, the interface must be "implemented" (kinda like inherited) by another class with the implements keyword (instead of extends). 
The body of the interface method is provided by the "implement" class.
*/

interface Animal {
    // Interface methods (does not have a body)
    public void animalSound(); 
    public void sleep();
}
  
class Pig implements Animal {
    public void animalSound() {
        System.out.println("The pig says: wee wee.");
    }

    public void sleep() {
        System.out.println("Zzz...");
    }
}

public class Main {
    public static void main(String[] args) {
        Pig myPig = new Pig();

        myPig.animalSound();
        myPig.sleep();
    }
}
```

Output:

```text
The pig says: wee wee.
Zzz...
```

## Multiple interfaces

Code:

```java
// To implement multiple interfaces, separate them with a comma.

interface FirstInterface {
    public void myMethod(); // Interface method
}
  
interface SecondInterface {
    public void myOtherMethod(); // Interface method
}
  
// DemoClass "implements" FirstInterface and SecondInterface
class DemoClass implements FirstInterface, SecondInterface {
    public void myMethod() {
        System.out.println("Some text..");
    }

    public void myOtherMethod() {
        System.out.println("Some other text...");
    }
}

public class Main {
    public static void main(String[] args) {
        DemoClass myObj = new DemoClass();

        myObj.myMethod();
        myObj.myOtherMethod();
    }
}
```

Output:

```text
Some text..
Some other text...
```