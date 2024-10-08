# Modifiers

## Public class

Code:

```java
/*
The public keyword is an access modifier, meaning that it is used to set the access level for classes, attributes, methods and constructors.
We divide modifiers into two groups:
* Access Modifiers - controls the access level
* Non-Access Modifiers - do not control access level, but provides other functionality
*/

public class Main { // The class is accessible by any other class
    public static void main(String[] args) { 
        System.out.println("Hello World!");
    }
}
```

Output:

```text
Hello World!
```

## Default class

Code:

```java
class Main { // The class is only accessible by classes in the same package. This is used when you don't specify a modifier.
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

Output:

```text
Hello World!
```

## Public attributes

Code:

```java
// public: The code is accessible for all classes

public class Person {
    public String fname = "Luis";
    public String lname = "Mendoza";
    public String email = "luis@mendoza.com";
    public int age = 29;
}
```

```java
public class Main {
    public static void main(String[] args) {
        Person myObj = new Person(); 
        
        System.out.println("Name: " + myObj.fname + " " + myObj.lname);
        System.out.println("Email: " + myObj.email);
        System.out.println("Age: " + myObj.age);
    }
}
```

Output:

```text
Name: Luis Mendoza
Email: luis@mendoza.com
Age: 29
```

## Private attributes

Code:

```java
public class Main {
    // private	The code is only accessible within the declared class
    private String fname = "Luis";
    private String lname = "Mendoza";
    private String email = "luis@mendoza.com";
    private int age = 29;
    
    public static void main(String[] args) {
        Main myObj = new Main();

        System.out.println("Name: " + myObj.fname + " " + myObj.lname);
        System.out.println("Email: " + myObj.email);
        System.out.println("Age: " + myObj.age);
    }
}
```

Output:

```text
Name: Luis Mendoza
Email: luis@mendoza.com
Age: 24
```

## Default attributes

Code:

```java
public class Main {
    // default	The code is only accessible in the same package. This is used when you don't specify a modifier.
    String fname = "Luis";
    String lname = "Mendoza";
    String email = "luis@mendoza.com";
    int age = 29;
    
    public static void main(String[] args) {
        Main myObj = new Main();

        System.out.println("Name: " + myObj.fname + " " + myObj.lname);
        System.out.println("Email: " + myObj.email);
        System.out.println("Age: " + myObj.age);
    }
}
```

Output:

```text
Name: Luis Mendoza
Email: luis@mendoza.com
Age: 29
```

## Protected attributes

Code:

```java
class Person {
    // protected	The code is accessible in the same package and subclasses.
    protected String fname = "Luis";
    protected String lname = "Mendoza";
    protected String email = "luis@mendoza.com";
    protected int age = 29;
}
  
class Main extends Person {
    private int graduationYear = 2018;

    public static void main(String[] args) {
        Main myObj = new Main();

        System.out.println("Name: " + myObj.fname + " " + myObj.lname);
        System.out.println("Email: " + myObj.email);
        System.out.println("Age: " + myObj.age);
        System.out.println("Graduation Year: " + myObj.graduationYear);
    }
}
```

Output:

```text
Name: Luis Mendoza
Email: luis@mendoza.com
Age: 29
Graduation Year: 2018
```

## Final class

Code:

```java
final class Main {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

Output:

```text
Hello World!
```

## Abstract class with abstract methods

Code:

```java
// An abstract method belongs to an abstract class, and it does not have a body. The body is provided by the subclass.

abstract class Person {
    public String fname = "Luis";
    public String lname = "Mendoza";
    public String email = "luis@mendoza.com";
    public int age = 29;

    public abstract void study(); // Abstract method 
}
```

```java
// Subclass (inherit from Person)

class Student extends Person {
    public int graduationYear = 2018;

    public void study() {
        System.out.println("Studying all day long!");
    }
}
```

```java
public class Main {
    public static void main(String[] args) {
        // Create an object of the Student class (which inherits attributes and methods from Person)
        Student myObj = new Student(); 
        
        System.out.println("Name: " + myObj.fname + " " + myObj.lname);
        System.out.println("Email: " + myObj.email);
        System.out.println("Age: " + myObj.age);
        System.out.println("Graduation Year: " + myObj.graduationYear);
        myObj.study(); // Call abstract method
    }
}
```

Output:

```text
Name: Luis Mendoza
Email: luis@mendoza.com
Age: 29
Graduation Year: 2018
Studying all day long!
```