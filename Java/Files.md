# Files

## Create a file

Code:

```java
/*
The File class has many useful methods for creating and getting information about files. For example:
Method	            Type	        Description
canRead()	        Boolean	        Tests whether the file is readable or not
canWrite()	        Boolean	        Tests whether the file is writable or not
createNewFile()	    Boolean	        Creates an empty file
delete()	        Boolean	        Deletes a file
exists()	        Boolean	        Tests whether the file exists
getName()	        String	        Returns the name of the file
getAbsolutePath()	String	        Returns the absolute pathname of the file
length()	        Long	        Returns the size of the file in bytes
list()	            String[]	    Returns an array of the files in the directory
mkdir()	            Boolean	        Creates a directory
*/

import java.io.File; 
import java.io.IOException;

public class Main {
    public static void main(String[] args) {  
        try {  
            File myObj = new File("filename.txt");  
            if(myObj.createNewFile()) {  
                System.out.println("File created: " + myObj.getName());  
            } 
            else {  
                System.out.println("File already exists!");  
            }  
            myObj.delete();
        } 
        catch(IOException e) {
            System.out.println("An error occurred!");
            e.printStackTrace(); // Prints this throwable and its backtrace to the standard error stream.
        }  
    }  
}
```

Output:

```text
File created: filename.txt
```

## Write to a file

Code:

```java
/*
We use the FileWriter class together with its write() method to write some text to a previous created file. 
Note that when you are done writing to the file, you should close it with the close() method.
*/

import java.io.FileWriter;
import java.io.IOException;
import java.io.File;

public class Main {
    public static void main(String[] args) {  
        try {  
            FileWriter myWriter = new FileWriter("filename.txt");

            myWriter.write("Files in Java might be tricky, but it is fun enough!");
            myWriter.close();
            System.out.println("Successfully wrote to the file.");
            File myObj = new File("filename.txt"); 
            myObj.delete();

        } 
        catch(IOException e) {
            System.out.println("An error occurred.");
            e.printStackTrace();
        } 
    } 
}
```

Output:

```text
Successfully wrote to the file.
```

## Read a file

Code:

```java
import java.io.File;
import java.io.FileNotFoundException;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {  
        try {
            File myObj = new File("filename.txt");
            Scanner myReader = new Scanner(myObj);  

            while(myReader.hasNextLine()) {
                String data = myReader.nextLine();
                System.out.println(data);
            }
            myReader.close();
        } 
        catch(FileNotFoundException e) {
            System.out.println("An error occurred.");
            e.printStackTrace();
        } 
    }  
}
```

Output:

```text
An error occurred.
java.io.FileNotFoundException: filename.txt (No such file or directory)
```

## Get file information

Code:

```java
import java.io.File; 
import java.io.IOException;

public class Main {
    public static void main(String[] args) {  
        File myObj = new File("filename.txt"); 
        try {  
            myObj.createNewFile();
        } 
        catch(IOException e) {
            e.printStackTrace(); // Prints this throwable and its backtrace to the standard error stream.
        }  

        if(myObj.exists()) {
            System.out.println("File name: " + myObj.getName()); 
            System.out.println("Absolute path: " + myObj.getAbsolutePath()); 
            System.out.println("Writeable: " + myObj.canWrite()); 
            System.out.println("Readable: " + myObj.canRead()); 
            System.out.println("File size in bytes: " + myObj.length());
            myObj.delete();
        } 
        else {
            System.out.println("The file does not exist.");
        }
    } 
}
```

Output:

```text
File name: filename.txt
Absolute path: /home/luis-mendoza/Documents/GitHub/Java_Examples/Files/filename.txt
Writeable: true
Readable: true
File size in bytes: 0
```

## Delete a file

Code:

```java
import java.io.File;
import java.io.IOException; 

public class Main {
    public static void main(String[] args) { 
        File myObj = new File("filename.txt"); 
        
        try {  
            myObj.createNewFile();
        } 
        catch(IOException e) {
            e.printStackTrace(); // Prints this throwable and its backtrace to the standard error stream
        }  

        if(myObj.delete()) { // To delete a file in Java, use the delete() method
            System.out.println("Deleted the file: " + myObj.getName());
        } 
        else {
            System.out.println("Failed to delete the file.");
        } 
    } 
}
```

Output:

```text
Deleted the file: filename.txt
```