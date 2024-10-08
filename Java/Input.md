# Input

## Read user input

Code:

```java
import java.util.Scanner; // Import the Scanner class 

public class Main {
    public static void main(String[] args) {
        Scanner myObj = new Scanner(System.in);
        String userName;
        
        // Enter username and press Enter
        System.out.println("Enter username: "); 
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

## Read user input of various types

Code:

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner myObj = new Scanner(System.in);
    
        // String input
        System.out.println("Enter name: ");
        String name = myObj.nextLine();
    
        // Numerical input
        System.out.println("Enter age: ");
        int age = myObj.nextInt();
        System.out.println("Enter salary: ");
        double salary = myObj.nextDouble();
    
        // Output input by user
        System.out.println("\nName: " + name); 
        System.out.println("Age: " + age); 
        System.out.println("Salary: " + salary); 
    }
}
```

Output:

```text
Enter name: 
Luis
Enter age: 
29
Enter salary: 
5000

Name: Luis
Age: 29
Salary: 5000.0
```