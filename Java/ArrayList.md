# ArrayList

## Create an ArrayList

Code:

```java
/*
The difference between a built-in array and an ArrayList in Java, is that the size of an array cannot be modified (if you want to add or remove elements to/from an array, 
you have to create a new one). While elements can be added and removed from an ArrayList whenever you want.
*/

import java.util.ArrayList;

public class Main {
    public static void main(String[] args) { 
        ArrayList<String> cars = new ArrayList<String>(); // Create an ArrayList object

        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("Mazda");
        System.out.println(cars);
    } 
}
```

Output:

```text
[Volvo, BMW, Ford, Mazda]
```

## Access an item in an ArrayList

Code:

```java
import java.util.ArrayList;

public class Main {
    public static void main(String[] args) { 
        ArrayList<String> cars = new ArrayList<String>();
        
        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("Mazda");
        System.out.println(cars.get(0));
    } 
}
```

Output:

```text
Volvo
```

## Remove an item from an ArrayList

Code:

```java
import java.util.ArrayList;

public class Main {
    public static void main(String[] args) { 
        ArrayList<String> cars = new ArrayList<String>();

        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("Mazda");
        cars.remove(0);
        System.out.println(cars);
    } 
}
```

Output:

```text
[BMW, Ford, Mazda]
```

## Remove all items from an ArrayList

Code:

```java
import java.util.ArrayList;

public class Main {
    public static void main(String[] args) { 
        ArrayList<String> cars = new ArrayList<String>();
        
        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
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

## Get the size of an ArrayList

Code:

```java
import java.util.ArrayList;

public class Main {
    public static void main(String[] args) { 
        ArrayList<String> cars = new ArrayList<String>();
        
        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("Mazda");
        System.out.println(cars.size());
    } 
}
```

Output:

```text
4
```

## Loop through an ArrayList

Code:

```java
import java.util.ArrayList;

public class Main {
    public static void main(String[] args) { 
        ArrayList<String> cars = new ArrayList<String>();
        
        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("Mazda");
        
        for (int i = 0; i < cars.size(); i++) {
            System.out.println(cars.get(i));
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

## Loop through an ArrayList with for-each

Code:

```java
import java.util.ArrayList;

public class Main {
    public static void main(String[] args) { 
        ArrayList<String> cars = new ArrayList<String>();

        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
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
BMW
Ford
Mazda
```

## Create an ArrayList that should store numbers (integers)

Code:

```java
import java.util.ArrayList;

public class Main {
    public static void main(String[] args) { 
        ArrayList<Integer> myNumbers = new ArrayList<Integer>();
        
        myNumbers.add(10);
        myNumbers.add(15);
        myNumbers.add(20);
        myNumbers.add(25);

        for (int i : myNumbers) {
            System.out.println(i);
        }
    } 
}
```

Output:

```text
10
15
20
25
```