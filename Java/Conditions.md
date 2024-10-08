# Conditions

## The if statement

Code:

```java
public class Main {
    public static void main(String[] args) {
        if(20 > 18) {
            System.out.println("20 is greater than 18!"); // obviously
        }  
    }
}
```

Output:

```text
20 is greater than 18!
```

## The else statement

Code:

```java
public class Main {
    public static void main(String[] args) {
        int time = 20;
        
        if(time < 18) {
            System.out.println("Good day!");
        } 
        else {
            System.out.println("Good evening!");
        }  
    }
}
```

Output:

```text
Good evening!
```

## The else if statement

Code:

```java
public class Main {
    public static void main(String[] args) {
        int time = 22;
        
        if(time < 10) {
            System.out.println("Good morning!");
        } 
        else if(time < 20) {
            System.out.println("Good day!");
        }  
        else {
            System.out.println("Good evening!");
        }
    }
}
```

Output:

```text
Good evening!
```