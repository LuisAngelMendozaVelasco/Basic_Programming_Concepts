# Iterator

## Getting an iterator

Code:

```java
// An Iterator is an object that can be used to loop through collections, like ArrayList and HashSet. It is called an "iterator" because "iterating" is the technical term for looping.

import java.util.ArrayList;
import java.util.Iterator;

public class Main {
    public static void main(String[] args) {
        // Make a collection
        ArrayList<String> cars = new ArrayList<String>();

        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("Mazda");
      
        // Get the iterator
        Iterator<String> it = cars.iterator();
      
        // Print the first item
        System.out.println(it.next());
    }
}
```

Output:

```text
Volvo
```

## Looping throug a collection

Code:

```java
import java.util.ArrayList;
import java.util.Iterator;

public class Main {
    public static void main(String[] args) {
        // Make a collection
        ArrayList<String> cars = new ArrayList<String>();

        cars.add("Volvo");
        cars.add("BMW");
        cars.add("Ford");
        cars.add("Mazda");
      
        // Get the iterator
        Iterator<String> it = cars.iterator();
        
        // Loop through a collection
        while(it.hasNext()) {
            System.out.println(it.next());
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

## Removing items from a collection

Code:

```java
import java.util.ArrayList;
import java.util.Iterator;

public class Main {
    public static void main(String[] args) {
        ArrayList<Integer> numbers = new ArrayList<Integer>();

        numbers.add(12);
        numbers.add(8);
        numbers.add(2);
        numbers.add(23);
        
        Iterator<Integer> it = numbers.iterator();

        while(it.hasNext()) {
            Integer i = it.next();

            if(i < 10) {
                it.remove();
            }
        }
        
        System.out.println(numbers);
    }
}
```

Output:

```text
[12, 23]
```