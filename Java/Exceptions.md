# Exceptions

## The try...catch statement

Code:

```java
public class Main {
    public static void main(String[] args) {
        try {
            int[] myNumbers = {1, 2, 3};
            
            System.out.println(myNumbers[10]);
        } 
        catch(Exception e) {
            System.out.println(e);
        }
    }
}
```

Output:

```text
java.lang.ArrayIndexOutOfBoundsException: Index 10 out of bounds for length 3
```

## The finally statement

Code:

```java
public class Main {
    public static void main(String[] args) {
        try {
            int[] myNumbers = {1, 2, 3};

            System.out.println(myNumbers[10]);
        } 
        catch(Exception e) {
            System.out.println(e);
        } 
        finally {
            System.out.println("The 'try catch' is finished.");
        }
    }
}
```

Output:

```text
java.lang.ArrayIndexOutOfBoundsException: Index 10 out of bounds for length 3
The 'try catch' is finished.
```

## The throw statement

Code:

```java
/*
The throw statement allows you to create a custom error.
The throw statement is used together with an exception type. There are many exception types available in Java: ArithmeticException, 
FileNotFoundException, ArrayIndexOutOfBoundsException, SecurityException, etc.
*/

public class Main {
    static void checkAge(int age) { 
        if(age < 18) {
            throw new ArithmeticException("Access denied - You must be at least 18 years old."); 
        } 
        else {
            System.out.println("Access granted - You are old enough!"); 
        }
    } 
     
    public static void main(String[] args) { 
        checkAge(15); 
    } 
}
```

Output:

```text
Exception in thread "main" java.lang.ArithmeticException: Access denied - You must be at least 18 years old.
```