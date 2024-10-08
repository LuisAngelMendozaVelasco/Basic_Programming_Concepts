# HashMap

## Create a HashMap

Code:

```java
/*
A HashMap stores items in "key/value" pairs, and you can access them by an index of another type (e.g. a String).
One object is used as a key (index) to another object (value). It can store different types: String keys and Integer values, or the same type, like: String keys and String values.
*/

import java.util.HashMap;

public class Main {
    public static void main(String[] args) {
        HashMap<String, String> capitalCities = new HashMap<String, String>();

        capitalCities.put("England", "London");
        capitalCities.put("Germany", "Berlin");
        capitalCities.put("Norway", "Oslo");
        capitalCities.put("USA", "Washington DC");
        System.out.println(capitalCities); 
    }
}
```

Output:

```text
{USA=Washington DC, Norway=Oslo, England=London, Germany=Berlin}
```

## Access an item in a HashMap

Code:

```java
import java.util.HashMap;

public class Main {
    public static void main(String[] args) {
        HashMap<String, String> capitalCities = new HashMap<String, String>();
        
        capitalCities.put("England", "London");
        capitalCities.put("Germany", "Berlin");
        capitalCities.put("Norway", "Oslo");
        capitalCities.put("USA", "Washington DC");
        System.out.println(capitalCities.get("England"));
    }
}
```

Output:

```text
London
```

## Remove an item from a HashMap

Code:

```java
import java.util.HashMap;

public class Main {
    public static void main(String[] args) {
        HashMap<String, String> capitalCities = new HashMap<String, String>();

        capitalCities.put("England", "London");
        capitalCities.put("Germany", "Berlin");
        capitalCities.put("Norway", "Oslo");
        capitalCities.put("USA", "Washington DC");
        capitalCities.remove("England");
        System.out.println(capitalCities); 
    }
}
```

Output:

```text
{USA=Washington DC, Norway=Oslo, Germany=Berlin}
```

## Remove all items from a HashMap

Code:

```java
import java.util.HashMap;

public class Main {
    public static void main(String[] args) {
        HashMap<String, String> capitalCities = new HashMap<String, String>();

        capitalCities.put("England", "London");
        capitalCities.put("Germany", "Berlin");
        capitalCities.put("Norway", "Oslo");
        capitalCities.put("USA", "Washington DC");
        capitalCities.clear();
        System.out.println(capitalCities); 
    }
}
```

Output:

```text
{}
```

## Get the size of a HashMap

Code:

```java
import java.util.HashMap;

public class Main {
    public static void main(String[] args) {
        HashMap<String, String> capitalCities = new HashMap<String, String>();
        
        capitalCities.put("England", "London");
        capitalCities.put("Germany", "Berlin");
        capitalCities.put("Norway", "Oslo");
        capitalCities.put("USA", "Washington DC");
        System.out.println(capitalCities.size());
    }
}
```

Output:

```text
4
```

## Loop through a HashMap

Code:

```java
import java.util.HashMap;

public class Main {
    public static void main(String[] args) {
        HashMap<String, String> capitalCities = new HashMap<String, String>();

        capitalCities.put("England", "London");
        capitalCities.put("Germany", "Berlin");
        capitalCities.put("Norway", "Oslo");
        capitalCities.put("USA", "Washington DC");
        
        for (String i : capitalCities.keySet()) {
            System.out.println("key: " + i + ", value: " + capitalCities.get(i));
        }
    }
}
```

Output:

```text
key: USA, value: Washington DC
key: Norway, value: Oslo
key: England, value: London
key: Germany, value: Berlin
```

## Create a HashMap that should store String keys and Integer values

Code:

```java
// Import the HashMap class
import java.util.HashMap;

public class Main {
    public static void main(String[] args) {
        // Create a HashMap object called people
        HashMap<String, Integer> people = new HashMap<String, Integer>();
    
        // Add keys and values (Name, Age)
        people.put("John", 32);
        people.put("Steve", 30);
        people.put("Angie", 33);

        for (String i : people.keySet()) {
            System.out.println("Name: " + i + ", Age: " + people.get(i));
        }
    }
}
```

Output:

```text
Name: Angie Age: 33
Name: Steve Age: 30
Name: John Age: 32
```