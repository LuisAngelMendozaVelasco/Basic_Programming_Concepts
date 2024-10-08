# Wrapper Classes

## Create an ArrayList that should store numbers (integers)

Code:

```java
/*
Wrapper classes provide a way to use primitive data types (int, boolean, etc..) as objects.
The table below shows the primitive type and the equivalent wrapper class:
    Primitive Data Type	        Wrapper Class
    byte	                    Byte
    short	                    Short
    int	                        Integer
    long	                    Long
    float	                    Float
    double	                    Double
    boolean	                    Boolean
    char	                    Character
Sometimes you must use wrapper classes, for example when working with Collection objects, such as ArrayList, where primitive types cannot be used (the list can only store objects).
*/

import java.util.ArrayList;

public class Main {
    public static void main(String[] args) { 
        ArrayList<Integer> myNumbers = new ArrayList<Integer>();

        myNumbers.add(10);
        myNumbers.add(15);
        myNumbers.add(20);
        myNumbers.add(25);
        
        for (int i : myNumbers) {
            System.out.println(i);
        }
    } 
}
```

Output:

```text
10
15
20
25
```

## Create wrapper objects

Code:

```java
// To create a wrapper object, use the wrapper class instead of the primitive type. To get the value, you can just print the object.

public class Main {
    public static void main(String[] args) { 
        Integer myInt = 5; 
        Double myDouble = 5.99; 
        Character myChar = 'A'; 

        System.out.println(myInt);
        System.out.println(myDouble);
        System.out.println(myChar);
    }
}
```

Output:

```text
5
5.99
A
```

## Using wrapper methods

Code:

```java
public class Main {
    public static void main(String[] args) { 
        Integer myInt = 5; 
        Double myDouble = 5.99; 
        Character myChar = 'A'; 
        
        System.out.println(myInt.intValue());
        System.out.println(myDouble.doubleValue());
        System.out.println(myChar.charValue());
    }
}
```

Output:

```text
5
5.99
A
```

## Convert wrapper objects to strings

Code:

```java
public class Main {
    public static void main(String[] args) { 
        Integer myInt = 100; 
        String myString = myInt.toString();
        
        System.out.println(myString.length());
    }
}
```

Output:

```text
3
```