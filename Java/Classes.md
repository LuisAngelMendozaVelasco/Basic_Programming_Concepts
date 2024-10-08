# Classes

## Create a class and an object of a class

Code:

```java
public class Main {
    int x = 5;

    public static void main(String[] args) {
        Main myObj = new Main();

        System.out.println(myObj.x);
    }
}
```

Output:

```text
5
```

## Create multiple objects of a class

Code:

```java
public class Main {
    int x = 5;

    public static void main(String[] args) {
        Main myObj1 = new Main();
        Main myObj2 = new Main();

        System.out.println(myObj1.x);
        System.out.println(myObj2.x);
    }
}
```

Output:

```text
5
5
```

## Accessing class attributes (variables)

Code:

```java
public class Main {
    int x = 5;

    public static void main(String[] args) {
        Main myObj = new Main();

        System.out.println(myObj.x);
    }
}
```

Output:

```text
5
```

## Modify attributes

Code:

```java
public class Main {
    int x;

    public static void main(String[] args) {
        Main myObj = new Main();

        myObj.x = 40;
        System.out.println(myObj.x);
    }
}
```

Output:

```text
40
```

## Override existing attribute values

Code:

```java
public class Main {
    int x = 10;

    public static void main(String[] args) {
        Main myObj = new Main();

        myObj.x = 25; // x is now 25
        System.out.println(myObj.x);
    }
}
```

Output:

```text
25
```

## Multiple attributes

Code:

```java
public class Main {
    String fname = "Luis";
    String lname = "Mendoza";
    int age = 29;
  
    public static void main(String[] args) {
        Main myObj = new Main();

        System.out.println("Name: " + myObj.fname + " " + myObj.lname);
        System.out.println("Age: " + myObj.age);
    }
}
```

Output:

```text
Name: Luis Mendoza
Age: 29
```

## Create a class method

Code:

```java
public class Main {
    static void myMethod() {
        System.out.println("Hello World!");
    }
    
    public static void main(String[] args) {
        myMethod();
    }
}
```

Output:

```text
Hello World!
```

## Method with parameters

Code:

```java
public class Main {
    static void myMethod(int x) {
        System.out.println(x);
    }
    
    public static void main(String[] args) {
        myMethod(10);
    }
}
```

Output:

```text
10
```

## Access class methods with an object

Code:

```java
public class Main {
    // Create a fullThrottle() method
    public void fullThrottle() {
        System.out.println("The car is going as fast as it can!");
    }

    // Create a speed() method and add a parameter
    public void speed(int maxSpeed) {
        System.out.println("Max speed is: " + maxSpeed);
    }

    // Inside main, call the methods on the myCar object
    public static void main(String[] args) {
        Main myCar = new Main();    // Create a myCar object

        myCar.fullThrottle();       // Call the fullThrottle() method
        myCar.speed(200);           // Call the speed() method
    }
}
```

Output:

```text
The car is going as fast as it can!
Max speed is: 200
```

## Create a class constructor

Code:

```java
public class Main {
    int x;

    // Create a class constructor for the Main class
    public Main() {
        x = 5;
    }
  
    public static void main(String[] args) {
        Main myObj = new Main();
        
        System.out.println(myObj.x);
    }
}
```

Output:

```text
5
```

## Constructor with parameters

Code:

```java
public class Main {
    int modelYear;
    String modelName;
  
    public Main(int year, String name) {
        modelYear = year;
        modelName = name;
    }
  
    public static void main(String[] args) {
        Main myCar = new Main(1969, "Mustang");

        System.out.println(myCar.modelYear + " " + myCar.modelName);
    }
}
```

Output:

```text
1969 Mustang
```