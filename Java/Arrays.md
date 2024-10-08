# Arrays

## Create and access an array

Code:

```java
public class Main {
    public static void main(String[] args) {
        String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
        
        System.out.println(cars[0]);
    }
}
```

Output:

```text
Volvo
```

## Change an array element

Code:

```java
public class Main {
    public static void main(String[] args) {
        String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
        
        cars[0] = "Opel";
        System.out.println(cars[0]);
    }
}
```

Output:

```text
Opel
```

## Find the length of an array

Code:

```java
public class Main {
    public static void main(String[] args) {
        String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};

        System.out.println(cars.length);
    }
}
```

Output:

```text
4
```

## Access an array

Code:

```java
public class Main {
    public static void main(String[] args) {
        String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
        
        cars[0] = "Opel";
        System.out.println(cars[0]);
    }
}
```

Output:

```text
Opel
```

## Loop through an array

Code:

```java
public class Main {
    public static void main(String[] args) {
        String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};

        for(int i = 0; i < cars.length; i++) {
            System.out.println(cars[i]);
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

## Loop through an array with for-each

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

## Multidimensional array

Code:

```java
public class Main {
    public static void main(String[] args) {
        int[][] myNumbers = \{\{1, 2, 3, 4\}, 
                             \{5, 6, 7\}\};
        int x = myNumbers[1][2];

        System.out.println(x);  
    }
}
```

Output:

```text
7
```

## Loop through a multidimensional array

Code:

```java
public class Main {
    public static void main(String[] args) {
        int[][] myNumbers = \{\{1, 2, 3, 4\}, \{5, 6, 7\}\};

        for(int i = 0; i < myNumbers.length; ++i) {
            for(int j = 0; j < myNumbers[i].length; ++j) {
                System.out.println(myNumbers[i][j]);
            }
        }
    }
}
```

Output:

```text
1
2
3
4
5
6
7
```