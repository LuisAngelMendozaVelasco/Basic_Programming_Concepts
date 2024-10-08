# Methods

## Create and call a method

Code:

```java
public class Main {
    static void myMethod() {
        System.out.println("I just got executed!");
    }
    
    public static void main(String[] args) {
        myMethod();
    }
}
```

Output:

```text
I just got executed!
```

## Call a method multiple times

Code:

```java
public class Main {
    static void myMethod() {
        System.out.println("I just got executed!");
    }
    
    public static void main(String[] args) {
        myMethod();
        myMethod();
        myMethod();
    }
}
```

Output:

```text
I just got executed!
I just got executed!
I just got executed!
```

## Method with parameters

Code:

```java
public class Main {
    static void myMethod(String fname) {
        System.out.println(fname + " Refsnes");
    }
    
    public static void main(String[] args) {
        myMethod("Liam");
        myMethod("Jenny");
        myMethod("Anja");
    }
}
```

Output:

```text
Liam Refsnes
Jenny Refsnes
Anja Refsnes
```

## Method with multiple parameters

Code:

```java
public class Main {
    static void myMethod(String fname, int age) {
        System.out.println(fname + " is " + age);
    }
    
    public static void main(String[] args) {
        myMethod("Liam", 5);
        myMethod("Jenny", 8);
        myMethod("Anja", 31);
    }
}
```

Output:

```text
Liam is 5
Jenny is 8
Anja is 31
```

## Return value

Code:

```java
public class Main {
    static int myMethod(int x) {
        return 5 + x;
    }
    
    public static void main(String[] args) {
        System.out.println(myMethod(3));
    }
}
```

Output:

```text
8
```

## A method with if...else

Code:

```java
public class Main {
    // Create a checkAge() method with an integer parameter called age
    static void checkAge(int age) {
        // If age is less than 18, print "access denied"
        if(age < 18) {
            System.out.println("Access denied - You are not old enough!"); 
        } 
        // If age is greater than, or equal to, 18, print "access granted"
        else {
            System.out.println("Access granted - You are old enough!"); 
        } 
    } 

    public static void main(String[] args) { 
        checkAge(20); // Call the checkAge method and pass along an age of 20
    } 
}
```

Output:

```text
Access granted - You are old enough!
```

## Method overloading

Code:

```java
public class Main {
    static int plusMethod(int x, int y) {
        return x + y;
    }
    
    static double plusMethod(double x, double y) {
        return x + y;
    }
    
    public static void main(String[] args) {
        int myNum1 = plusMethod(8, 5);
        double myNum2 = plusMethod(4.3, 6.26);

        System.out.println("int: " + myNum1);
        System.out.println("double: " + myNum2);
    } 
}
```

Output:

```text
int: 13
double: 10.559999999999999
```

## Recursion

Code:

```java
/*
10 + sum(9)
10 + ( 9 + sum(8) )
10 + ( 9 + ( 8 + sum(7) ) )
...
10 + 9 + 8 + 7 + 6 + 5 + 4 + 3 + 2 + 1 + sum(0)
10 + 9 + 8 + 7 + 6 + 5 + 4 + 3 + 2 + 1 + 0
Since the function does not call itself when k is 0, the program stops there and returns the result.
*/

public class Main {
    public static void main(String[] args) {
        int result = sum(10);

        System.out.println(result);
    }

    public static int sum(int k) {
        if(k > 0) {
            return k + sum(k - 1);
        } 
        else {
            return 0;
        }
    }
}
```

Output:

```text
55
```

## Recursive function with a halting condition

Code:

```java
/*
Just as loops can run into the problem of infinite looping, recursive functions can run into the problem of infinite recursion. 
Infinite recursion is when the function never stops calling itself. 
Every recursive function should have a halting condition, which is the condition where the function stops calling itself. 
In this example, the function adds a range of numbers between a start and an end. The halting condition for this recursive function is when end is not greater than start.
*/

public class Main {
    public static void main(String[] args) {
        int result = sum(5, 10);

        System.out.println(result);
    }
    
    public static int sum(int start, int end) {
        if(end > start) {
            return end + sum(start, end - 1);
        } 
        else {
            return end;
        }
    }
}
```

Output:

```text
45
```