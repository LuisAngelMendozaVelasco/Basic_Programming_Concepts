# Structures

## Access Structure Members

Code:

```cpp
#include <iostream>
using namespace std;

// Create a structure variable called myStructure
struct {
    int myNum;
    string myString;
} myStructure;

int main() {
    // Assign values to members of myStructure
    myStructure.myNum = 1;
    myStructure.myString = "Hello World!";

    // Print members of myStructure
    cout << myStructure.myNum << "\n";
    cout << myStructure.myString << "\n";

    return 0;
}
```

Output:

```text
1
Hello World!
```

## One Structure in Multiple Variables

Code:

```cpp
#include <iostream>
using namespace std;

struct {
    string brand;
    string model;
    int year;
} myCar1, myCar2; // We can add variables by separating them with a comma here

int main() {
    // Put data into the first structure
    myCar1.brand = "BMW";
    myCar1.model = "X5";
    myCar1.year = 1999;

    // Put data into the second structure
    myCar2.brand = "Ford";
    myCar2.model = "Mustang";
    myCar2.year = 1969;

    // Print the structure members
    cout << myCar1.brand << " " << myCar1.model << " " << myCar1.year << "\n";
    cout << myCar2.brand << " " << myCar2.model << " " << myCar2.year << "\n";

    return 0;
}
```

Output:

```text
BMW X5 1999
Ford Mustang 1969
```

## Named Structures

Code:

```cpp
#include <iostream>
using namespace std;

// Declare a structure named "car"
struct car {
    string brand;
    string model;
    int year;
};

int main() {
    // Create a car structure and store it in myCar1;
    car myCar1;
    myCar1.brand = "BMW";
    myCar1.model = "X5";
    myCar1.year = 1999;

    // Create another car structure and store it in myCar2;
    car myCar2;
    myCar2.brand = "Ford";
    myCar2.model = "Mustang";
    myCar2.year = 1969;

    // Print the structure members
    cout << myCar1.brand << " " << myCar1.model << " " << myCar1.year << "\n";
    cout << myCar2.brand << " " << myCar2.model << " " << myCar2.year << "\n";

    return 0;
}
```

Output:

```text
BMW X5 1999
Ford Mustang 1969
```