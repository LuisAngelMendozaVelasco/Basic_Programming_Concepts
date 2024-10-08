# Data Types

## A demonstration of different data types in Java

Code:

```java
public class Main {
    public static void main(String[] args) {
        int myNum = 5;               // integer (whole number)
        float myFloatNum = 5.99f;    // floating point number
        char myLetter = 'D';         // character
        boolean myBool = true;       // boolean
        String myText = "Hello";     // String  

        System.out.println(myNum);
        System.out.println(myFloatNum);
        System.out.println(myLetter);
        System.out.println(myBool);
        System.out.println(myText);
    }
}
```

Output:

```text
5
5.99
D
true
Hello
```

## Create a byte type

Code:

```java
public class Main {
    public static void main(String[] args) {
        byte myNum = 100; // Stores whole numbers from -128 to 127

        System.out.println(myNum);  
    }
}
```

Output:

```text
100
```

## Create a short type

Code:

```java
public class Main {
    public static void main(String[] args) {
        short myNum = 5000; // Stores whole numbers from -32,768 to 32,767

        System.out.println(myNum);  
    }
}
```

Output:

```text
5000
```

## Create an int type

Code:

```java
public class Main {
    public static void main(String[] args) {
        int myNum = 100000; // Stores whole numbers from -2,147,483,648 to 2,147,483,647

        System.out.println(myNum);  
    }
}
```

Output:

```text
100000
```

## Create a long type

Code:

```java
public class Main {
    public static void main(String[] args) {
        long myNum = 15000000000L; //Stores whole numbers from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807

        System.out.println(myNum);  
    }
}
```

Output:

```text
15000000000
```

## Create a float type

Code:

```java
public class Main {
    public static void main(String[] args) {
        float myNum = 5.75f; //Stores fractional numbers. Sufficient for storing 6 to 7 decimal digits

        System.out.println(myNum);  
    }
}
```

Output:

```text
5.75
```

## Create a double type

Code:

```java
public class Main {
    public static void main(String[] args) {
        double myNum = 19.99d; //Stores fractional numbers. Sufficient for storing 15 decimal digits

        System.out.println(myNum);  
    }
}
```

Output:

```text
19.99
```

## Create a boolean type

Code:

```java
public class Main {
    public static void main(String[] args) {
        boolean isJavaFun = true;
        boolean isFishTasty = false;    

        System.out.println(isJavaFun);
        System.out.println(isFishTasty);
    }
}
```

Output:

```text
true
false
```

## Create a char type

Code:

```java
public class Main {
    public static void main(String[] args) {
        char myGrade = 'B';

        System.out.println(myGrade);
    }
}
```

Output:

```text
B
```

## Create a String type

Code:

```java
public class Main {
    public static void main(String[] args) {
        String greeting = "Hello World!";

        System.out.println(greeting);
    }
}
```

Output:

```text
Hello World!
```