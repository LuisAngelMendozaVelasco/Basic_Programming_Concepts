# Functions

## Create and call a function

Code:

```cpp
#include <iostream>
using namespace std;

void myFunction() {
    cout << "I just got executed!" << endl;
}

int main() {
    myFunction();

    return 0;
}
```

Output:

```text
I just got executed!
```

## Call a function multiple times

Code:

```cpp
#include <iostream>
using namespace std;

void myFunction() {
    cout << "I just got executed!\n";
}

int main() {
    myFunction();
    myFunction();
    myFunction();

    return 0;
}
```

Output:

```text
I just got executed!
I just got executed!
I just got executed!
```

## Function declaration and definition

Code:

```cpp
#include <iostream>
using namespace std;

// Function declaration
void myFunction();

// The main method
int main() {
    myFunction();  // call the function

    return 0;
}

// Function definition
void myFunction() {
    cout << "I just got executed!" << endl;
}
```

Output:

```text
I just got executed!
```

## Parameters and arguments

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

void myFunction(string fname) {
    cout << fname << " Refsnes\n";
}

int main() {
    myFunction("Liam");
    myFunction("Jenny");
    myFunction("Anja");

    return 0;
}
```

Output:

```text
Liam Refsnes
Jenny Refsnes
Anja Refsnes
```

## Default parameter value

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

void myFunction(string country = "Norway") {
    cout << country << "\n";
}

int main() {
    myFunction("Sweden");
    myFunction("India");
    myFunction();
    myFunction("USA");

    return 0;
}
```

Output:

```text
Sweden
India
Norway
USA
```

## Multiple parameters

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

void myFunction(string fname, int age) {
    cout << fname << " Refsnes, " << age << " years old. \n";
}

int main() {
    myFunction("Liam", 3);
    myFunction("Jenny", 14);
    myFunction("Anja", 30);

    return 0;
}
```

Output:

```text
Liam Refsnes, 3 years old. 
Jenny Refsnes, 14 years old. 
Anja Refsnes, 30 years old. 
```

## Return value

Code:

```cpp
#include <iostream>
using namespace std;

int myFunction(int x) {
    return 5 + x;
}

int main() {
    cout << myFunction(3) << endl;

    return 0;
}
```

Output:

```text
8
```

## Return the sum of two parameters

Code:

```cpp
#include <iostream>
using namespace std;

int myFunction(int x, int y) {
    return x + y;
}

int main() {
    cout << myFunction(5, 3) << endl;

    return 0;
}
```

Output:

```text
8
```

## Pass by reference

Code:

```cpp
#include <iostream>
using namespace std;

void swapNums(int &x, int &y) {
    int z = x;

    x = y;
    y = z;
}

int main() {
    int firstNum = 10;
    int secondNum = 20;

    cout << "Before swap: " << "\n";
    cout << firstNum << "\n" << secondNum << "\n";

    swapNums(firstNum, secondNum);

    cout << "\nAfter swap: " << "\n";
    cout << firstNum << "\n" << secondNum << "\n";

    return 0;
}
```

Output:

```text
Before swap: 
10
20

After swap: 
20
10
```

## Pass an array to a function

Code:

```cpp
#include <iostream> 
using namespace std;  

void myFunction(int myNumbers[5]) {
    for(int i = 0; i < 5; i++) {  
        cout << myNumbers[i] << "\n";    
    } 
}

int main() {  
    int myNumbers[5] = {10, 20, 30, 40, 50};  
    
    myFunction(myNumbers);

    return 0;
}  
```

Output:

```text
10
20
30
40
50
```

## Function overloading

Code:

```cpp
#include <iostream>
using namespace std;

//With function overloading, multiple functions can have the same name with different parameters
int plusFunc(int x, int y) {
    return x + y;
}

double plusFunc(double x, double y) {
    return x + y;
}

int main() {
    int myNum1 = plusFunc(8, 5);
    double myNum2 = plusFunc(4.3, 6.26);

    cout << "Int: " << myNum1 << "\n";
    cout << "Double: " << myNum2 << endl;

    return 0;
}
```

Output:

```text
Int: 13
Double: 10.56
```

## Recursion

Code:

```cpp
#include <iostream>
using namespace std;

// Recursion is the technique of making a function call itself. 
int sum(int k) {
    if(k > 0) {
        return k + sum(k - 1);
    } 
    else {
        return 0;
    }
}

int main() {
    int result = sum(10);

    cout << result << endl;

    return 0;
}
```

Output:

```text
55
```