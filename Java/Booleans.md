# Booleans

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

## Find out if an expression is true or false

Code:

```java
public class Main {
    public static void main(String[] args) {
        int x = 10;
        int y = 9;
        
        System.out.println(x > y); // Returns true, because 10 is higher than 9  
    }
}
```

Output:

```text
true
```

## Use the "equal to" operator to evaluate a boolean expression

Code:

```java
public class Main {
    public static void main(String[] args) {
        int x = 10;
        
        System.out.println(x == 10); // Returns true, because the value of x is equal to 10
    }
}
```

Output:

```text
true
```