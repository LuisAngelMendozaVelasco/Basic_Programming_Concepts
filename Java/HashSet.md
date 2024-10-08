# HashSet

## Create a HashSet and add items to it


Code:

```java
// A HashSet is a collection of items where every item is unique

// Import the HashSet class
import java.util.HashSet;

public class Main {
    public static void main(String[] args) {
        HashSet<String> cars = new HashSet<String>();

        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("BMW");
        cars.add("Mazda");
        System.out.println(cars);
    }
}
```

Output:

```text
[Volvo, Mazda, Ford, BMW]
```

## Check if an item exists in a HashSet

Code:

```java
// Import the HashSet class
import java.util.HashSet;

public class Main {
    public static void main(String[] args) {
        HashSet<String> cars = new HashSet<String>();
        
        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("BMW");
        cars.add("Mazda");
        System.out.println(cars.contains("Mazda"));
    }
}
```

Output:

```text
true
```

## Remove an item from a HashSet

Code:

```java
// Import the HashSet class
import java.util.HashSet;

public class Main {
    public static void main(String[] args) {
        HashSet<String> cars = new HashSet<String>();
        
        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("BMW");
        cars.add("Mazda");
        cars.remove("Volvo");
        System.out.println(cars);
    }
}
```

Output:

```text
[Mazda, Ford, BMW]
```

## Remove all items from a HashSet

Code:

```java
// Import the HashSet class
import java.util.HashSet;

public class Main {
    public static void main(String[] args) {
        HashSet<String> cars = new HashSet<String>();
        
        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("BMW");
        cars.add("Mazda");
        cars.clear();
        System.out.println(cars);
    }
}
```

Output:

```text
[]
```

## Get the size of a HashSet

Code:

```java
// Import the HashSet class
import java.util.HashSet;

public class Main {
    public static void main(String[] args) {
        HashSet<String> cars = new HashSet<String>();
        
        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("BMW");
        cars.add("Mazda");
        System.out.println(cars.size());
    }
}
```

Output:

```text
4
```

## Loop through a HashSet

Code:

```java
// Import the HashSet class
import java.util.HashSet;

public class Main {
    public static void main(String[] args) {
        HashSet<String> cars = new HashSet<String>();

        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("BMW");
        cars.add("Mazda");
        
        for(String i : cars) {
            System.out.println(i);
        }
    }
}
```

Output:

```text
Volvo
Mazda
Ford
BMW
```

## Create a HashSet that should store Integer values

Code:

```java
// Import the HashSet class
import java.util.HashSet;

public class Main {
    public static void main(String[] args) {
        // Create a HashSet object called numbers
        HashSet<Integer> numbers = new HashSet<Integer>();
    
        // Add values to the set
        numbers.add(4);
        numbers.add(7);
        numbers.add(8);
    
        // Show which numbers between 1 and 10 are in the set
        for(int i = 1; i <= 10; i++) {
            if(numbers.contains(i)) {
                System.out.println(i + " was found in the set.");
            } 
            else {
                System.out.println(i + " was not found in the set.");
            }
        }
    }
}
```

Output:

```text
1 was not found in the set.
2 was not found in the set.
3 was not found in the set.
4 was found in the set.
5 was not found in the set.
6 was not found in the set.
7 was found in the set.
8 was found in the set.
9 was not found in the set.
10 was not found in the set.
```