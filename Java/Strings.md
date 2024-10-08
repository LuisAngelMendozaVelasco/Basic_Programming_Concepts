# Strings

## Create a string

Code:

```java
public class Main {
    public static void main(String[] args) {
        String greeting = "Hello";

        System.out.println(greeting);
    }
}
```

Output:

```text
Hello!
```

## Quotes inside a string

Code:

```java
public class Main {
    public static void main(String[] args) {
        String txt1 = "It's alright!";
        String txt2 = "That's great!";
        
        System.out.println(txt1);
        System.out.println(txt2);
    }
}
```

Output:

```text
It's alright!
That's great!
```

## Find the length of a string

Code:

```java
public class Main {
    public static void main(String[] args) {
        String txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

        System.out.println("The length of the txt string is: " + txt.length());
    }
}
```

Output:

```text
The length of the txt string is: 26
```

## Using methods to convert strings to uppercase and lowercase

Code:

```java
public class Main {
    public static void main(String[] args) {
        String txt = "Hello World!";

        System.out.println(txt.toUpperCase());
        System.out.println(txt.toLowerCase());
    }
}
```

Output:

```text
HELLO WORLD!
hello world!
```

## Finding a string in a string

Code:

```java
public class Main {
    public static void main(String[] args) {
        String txt = "Please locate where 'locate' occurs!";

        System.out.println(txt.indexOf("locate"));
    }
}
```

Output:

```text
7
```

## String concatenation

Code:

```java
public class Main {
    public static void main(String args[]) {
        String firstName = "Luis";
        String lastName = "Mendoza";

        System.out.println(firstName + " " + lastName);
    }
}
```

Output:

```text
Luis Mendoza
```

## If you add a number and a string, the result will be a string concatenation

Code:

```java
public class Main {
    public static void main(String[] args) {
        String x = "10";
        int y = 20;
        String z = x + y;
        
        System.out.println(z);
    }
}
```

Output:

```text
1020
```