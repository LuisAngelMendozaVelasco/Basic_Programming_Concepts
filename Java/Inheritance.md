# Inheritance

## Inheritance (extends)

Code:

```java
class Vehicle {
    protected String brand = "Ford";

    public void honk() {
        System.out.println("Tuut, tuut!");
    }
}
  
class Main extends Vehicle {
    private String modelName = "Mustang";
    
    public static void main(String[] args) {
        Main myFastCar = new Main();
        
        myFastCar.honk();
        System.out.println(myFastCar.brand + " " + myFastCar.modelName);
    }
}
```

Output:

```text
Tuut, tuut!
Ford Mustang
```

## Polymorphism

Code:

```java
/*
Polymorphism means "many forms", and it occurs when we have many classes that are related to each other by inheritance.
Inheritance lets us inherit attributes and methods from another class. 
Polymorphism uses those methods to perform different tasks. This allows us to perform a single action in different ways.
For example, think of a superclass called Animal that has a method called animalSound(). 
Subclasses of Animals could be Pigs, Cats, Dogs, Birds - And they also have their own implementation of an animal sound (the pig oinks, and the cat meows, etc.).
*/

class Animal {
    public void animalSound() {
        System.out.println("The animal makes a sound.");
    }
}
  
class Pig extends Animal {
    public void animalSound() {
        System.out.println("The pig says: wee wee.");
    }
}
  
class Dog extends Animal {
    public void animalSound() {
        System.out.println("The dog says: bow wow.");
    }
}
  
class Main {
    public static void main(String[] args) {
        Animal myAnimal = new Animal();
        Animal myPig = new Pig();
        Animal myDog = new Dog();
            
        myAnimal.animalSound();
        myPig.animalSound();
        myDog.animalSound();
    }
}
```

Output:

```text
The animal makes a sound.
The pig says: wee wee.
The dog says: bow wow.
```