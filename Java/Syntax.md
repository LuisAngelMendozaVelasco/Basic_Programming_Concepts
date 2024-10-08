# Syntax

## Create a simple "Hello World" program

Code:

```java
/*
Every line of code that runs in Java must be inside a class.
A class should always start with an uppercase first letter.
Note: Java is case-sensitive: "MyClass" and "myclass" has different meaning.
The name of the java file must match the class name. When saving the file, save it using the class name and add ".java" to the end of the filename.
*/

public class Main {
    /*
    The main() method is required and you will see it in every Java program.
    Any code inside the main() method will be executed.
    Just remember that every Java program has a class name which must match the filename, and that every program must contain the main() method.
    */
    public static void main(String[] args) { // The curly braces {} marks the beginning and the end of a block of code.
        /*
        Inside the main() method, we can use the println() method to print a line of text to the screen.
        System is a built-in Java class that contains useful members, such as out, which is short for "output". 
        The println() method, short for "print line", is used to print a value to the screen (or a file).
        */
        System.out.println("Hello World!"); // Each code statement must end with a semicolon (;).
    }
}
```

Output:

```text
Hello World!
```