# Variables

## Create a string variable

Code:

```java
public class Main {
    public static void main(String[] args) {
        String name = "Luis";  
          
        System.out.println(name);
    }
}
```

Output:

```text
Luis
```

## Create an integer variable

Code:

```java
public class Main {
    public static void main(String[] args) {
        int myNum = 15;

        System.out.println(myNum);
    }    
}
```

Output:

```text
15
```

## Create a variable without assigning the value, and assign the value later

Code:

```java
public class Main {
    public static void main(String[] args) {
        int myNum;

        myNum = 15;
        System.out.println(myNum);
    }
}
```

Output:

```text
15
```

## Overwrite an existing variable value

Code:

```java
public class Main {
    public static void main(String[] args) {
        int myNum = 15;

        myNum = 20;  // myNum is now 20
        System.out.println(myNum);
    }
}
```

Output:

```text
20
```

## Create a final variable (unchangeable and read-only)

Code:

```java
public class Main {
    public static void main(String[] args) {
        final int myNum = 15;

        myNum = 20; // will generate an error
        System.out.println(myNum);
    }
}
```

Output:

```text
error: cannot assign a value to final variable myNum
```

## Combine text and a variable on display

Code:

```java
public class Main {
    public static void main(String[] args) {
        String name = "Luis";

        System.out.println("Hello " + name + "!");
    }
}
```

Output:

```text
Hello Luis!
```

## Add a variable to another variable

Code:

```java
public class Main {
    public static void main(String[] args) {
        String firstName = "Luis ";
        String lastName = "Mendoza";
        String fullName = firstName + lastName;
        
        System.out.println(fullName);  
    }
}
```

Output:

```text
Luis Mendoza
```

## Declare many variables of the same type with a comma-separated list

Code:

```java
public class Main {
    public static void main(String[] args) {
        int x = 5, y = 6, z = 50;

        System.out.println(x + y + z);
    }
}
```

Output:

```text
61
```