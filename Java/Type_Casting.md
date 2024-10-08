# Type Casting

## Widening Casting

Code:

```java
public class Main {
    public static void main(String[] args) {
        int myInt = 9;
        double myDouble = myInt; // Automatic casting: int to double
    
        System.out.println(myInt);
        System.out.println(myDouble);
    }
}
```

Output:

```text
9
9.0
```

## Narrowing Casting

Code:

```java
public class Main {
    public static void main(String[] args) {
        double myDouble = 9.78d;
        int myInt = (int) myDouble; // Explicit casting: double to int
    
        System.out.println(myDouble);
        System.out.println(myInt);
    }
}
```

Output:

```text
9.78
9
```