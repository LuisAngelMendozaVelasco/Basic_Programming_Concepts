# Threads

## Running a thread by extending the thread class

Code:

```java
/*
Threads allows a program to operate more efficiently by doing multiple things at the same time.
Threads can be used to perform complicated tasks in the background without interrupting the main program.
It can be created by extending the Thread class and overriding its run() method.
*/

public class Main extends Thread{
    public static void main(String[] args) {
        Main thread = new Main();

        thread.start(); // Causes this thread to begin execution; the Java Virtual Machine calls the run method of this thread.
        System.out.println("This code is outside of the thread.");
    }

    public void run() {
        System.out.println("This code is running in a thread.");
    }
}
```

Output:

```text
This code is outside of the thread.
This code is running in a thread.
```

## Running a thread by implementing the Runnable interface

Code:

```java
public class Main implements Runnable {
    public static void main(String[] args) {
        Main obj = new Main();
        Thread thread = new Thread(obj);
        
        thread.start();
        System.out.println("This code is outside of the thread.");
    }

    public void run() {
        System.out.println("This code is running in a thread.");
    }
}
```

Output:

```text
This code is outside of the thread.
This code is running in a thread.
```

## Concurrency problems

Code:

```java
/*
Because threads run at the same time as other parts of the program, there is no way to know in which order the code will run. 
When the threads and main program are reading and writing the same variables, the values are unpredictable. 
The problems that result from this are called concurrency problems.
*/

public class Main extends Thread {
    public static int amount = 0;

    public static void main(String[] args) {
        Main thread = new Main();

        thread.start();
        System.out.println(amount);
        amount++;
        System.out.println(amount);
    }
  
    public void run() {
        amount++;
    }
}
```

Output:

```text
0
2
```

## Avoid concurrency problems

Code:

```java
/*
To avoid concurrency problems, it is best to share as few attributes between threads as possible. 
If attributes need to be shared, one possible solution is to use the isAlive() method of the thread to check whether the thread has 
finished running before using any attributes that the thread can change.
*/

public class Main extends Thread {
    public static int amount = 0;

    public static void main(String[] args) {
        Main thread = new Main();

        thread.start();

        // Wait for the thread to finish
        while(thread.isAlive()) {
            System.out.println("Waiting...");
        }

        // Update amount and print its value
        System.out.println("Main: " + amount);
        amount++;
        System.out.println("Main: " + amount);
    }

    public void run() {
        amount++;
    }
}
```

Output:

```text
Waiting...
Main: 1
Main: 2
```