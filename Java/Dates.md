# Dates

## Display current date

Code:

```java
import java.time.LocalDate;  // Import the LocalDate class

public class Main {
    public static void main(String[] args) {  
        LocalDate myObj = LocalDate.now();  // Create a date object
        
        System.out.println(myObj);  // Display the current date
    }  
}
```

Output:

```text
2023-12-20
```

## Display current time

Code:

```java
import java.time.LocalTime;  // Import the LocalTime class

public class Main {
    public static void main(String[] args) {  
        LocalTime myObj = LocalTime.now();

        System.out.println(myObj);
    } 
}
```

Output:

```text
14:58:05.824755
```

## Display current date and time

Code:

```java
import java.time.LocalDateTime;  // Import the LocalDateTime class

public class Main {
    public static void main(String[] args) {  
        LocalDateTime myObj = LocalDateTime.now();

        System.out.println(myObj);
    }
}
```

Output:

```text
2023-12-20T14:58:05.824755
```

## Formatting date and time

Code:

```java
import java.time.LocalDateTime;  // Import the LocalDateTime class
import java.time.format.DateTimeFormatter;  // Import the DateTimeFormatter class

public class Main {
    public static void main(String[] args) {  
        LocalDateTime myDateObj = LocalDateTime.now();  

        System.out.println("Before formatting: " + myDateObj);  

        DateTimeFormatter myFormatObj = DateTimeFormatter.ofPattern("dd-MM-yyyy HH:mm:ss");  
        String formattedDate = myDateObj.format(myFormatObj);  

        System.out.println("After formatting: " + formattedDate);  
    }  
}
```

Output:

```text
Before formatting: 2023-12-20T14:58:05.824755
After formatting: 2023-12-20 14:58:05
```