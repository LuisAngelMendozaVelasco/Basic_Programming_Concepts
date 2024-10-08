# Packages

## Import a class from the Java API

Code:

```java
/*
A package in Java is used to group related classes. Think of it as a folder in a file directory. We use packages to avoid name conflicts, and to write a better maintainable code. 
Packages are divided into two categories:
- Built-in Packages (packages from the Java API)
- User-defined Packages (create your own packages)
*/

import java.util.Scanner; // Import the Scanner class 

public class Main {
    public static void main(String[] args) {
        Scanner myObj = new Scanner(System.in);
        String userName;
        
        // Enter username and press Enter
        System.out.println("Enter username:"); 
        userName = myObj.nextLine();   
        System.out.println("\nUsername is: " + userName);        
    }
}
```

Output:

```text
Enter username:
Luis

Username is: Luis
```

## Import a package from the Java API

Code:

```java
import java.util.*; // Import the java.util package 

public class Main {
    public static void main(String[] args) {
        Scanner myObj = new Scanner(System.in);
        String userName;
        
        // Enter username and press Enter
        System.out.println("Enter username:"); 
        userName = myObj.nextLine();   
           
        System.out.println("\nUsername is: " + userName);        
    }
}
```

Output:

```text
Enter username:
Luis

Username is: Luis
```

## Create a package

Code:

```java
/*
To create your own package, you need to understand that Java uses a file system directory to store them. Just like folders on your computer:
Example
└── root
  └── mypack
    └── MyPackageClass.java
To create a package, use the package keyword
*/

/*
Save the file as MyPackageClass.java, and compile it:
- C:\Users\Your Name>javac MyPackageClass.java
Then compile the package:
- C:\Users\Your Name>javac -d . MyPackageClass.java
This forces the compiler to create the "mypack" package.
The -d keyword specifies the destination for where to save the class file. You can use any directory name, like c:/user (windows), or, 
if you want to keep the package within the same directory, you can use the dot sign ".".
Note: The package name should be written in lower case to avoid conflict with class names.
*/

package mypack;

public class MyPackageClass {
    public static void main(String[] args) { 
        System.out.println("This is my package!"); 
    } 
}
```

Output:

```text
This is my package!
```