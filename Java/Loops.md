# Loops

## While loop

Code:

```java
public class Main {
    public static void main(String[] args) {
        int i = 0;

        while(i < 5) {
            System.out.println(i);
            i++;
        }  
    }
}
```

Output:

```text
0
1
2
3
4
```

## Do while loop

Code:

```java
public class Main {
    public static void main(String[] args) {
        int i = 0;
        
        do {
            System.out.println(i);
            i++;
        }
        while(i < 5);  
    }
}
```

Output:

```text
0
1
2
3
4
```

## For loop

Code:

```java
public class Main {
    public static void main(String[] args) {
        for(int i = 0; i < 5; i++) {
            System.out.println(i);
        }  
    }
}
```

Output:

```text
0
1
2
3
4
```

## For-each loop

Code:

```java
public class Main {
    public static void main(String[] args) {
        String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
        
        for(String i : cars) {
            System.out.println(i);
        }    
    }
}
```

Output:

```text
Volvo
BMW
Ford
Mazda
```

## Break a loop

Code:

```java
public class Main {
    public static void main(String[] args) {
        for(int i = 0; i < 10; i++) {
            if(i == 4) {
                break;
            }
            
            System.out.println(i);
        }  
    }
}
```

Output:

```text
0
1
2
3
```

## Continue a loop

Code:

```java
public class Main {
    public static void main(String[] args) {
        for(int i = 0; i < 10; i++) {
            if(i == 4) {
                continue;
            }

            System.out.println(i);
        }  
    }
}
```

Output:

```text
0
1
2
3
5
6
7
8
9
```